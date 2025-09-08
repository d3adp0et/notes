# PNPT Study Plan - 12 Week Grind

## The Schedule (4-5 hrs/day, 5 days/week)

### Weeks 1-2: Getting Your Bearings
**What you're doing:** Basic stuff + OSINT

Study:
- Knock out the rest of PEH modules (networking, Linux/Windows basics, tool intro)
- Go through the OSINT Fundamentals course

Lab work:
- Hit up 2-3 OSINT challenges. TraceLabs CTF archives are solid, OSINTCurio.us blog has good stuff too
- Pop some easy boxes on HTB or THM - nothing crazy, just get comfortable

Documentation:
- Start taking screenshots of everything. Write up what you did, even if it's messy

---

### Weeks 3-4: Breaking Into Stuff
**What you're doing:** Finding vulns → exploiting them → writing it up

Study:
- PEH web app hacking, scanning techniques, exploitation basics

Lab work:
- 2-3 HTB boxes per week (easy/medium difficulty)
- Grab some VulnHub machines that look like real external services
- Get comfortable with Nmap, Gobuster, Burp Suite - use them on everything

Documentation:
- Write a mini report for each box. What was broken, why it matters, how to fix it

---

### Weeks 5-7: AD Hell (But Good Hell)
**What you're doing:** Learning to wreck Active Directory environments

Study:
- Finish all the PEH AD modules
- Read The Pentester's Playbook (TCM's book - it's actually pretty good)

Lab work:
- Spin up your own AD lab. One DC, couple of clients. Break it, fix it, break it again
- Learn to love these tools: Responder, CrackMapExec, BloodHound, Mimikatz, all the Impacket stuff
- If you've got the cash, HTB Pro Labs (Offshore or RastaLabs) are worth it. VHL works too

Documentation:
- Map out your attack paths. Draw diagrams if it helps

---

### Weeks 8-9: Pretend It's Real
**What you're doing:** Full pentest from start to finish

Pick a big lab environment and go through the whole process:
1. Recon (even if you're just pretending it's a real company)
2. Get initial foothold from external
3. Move laterally, get Domain Admin
4. Set up persistence if you're feeling fancy

Write a complete report using TCM's template. Make it look professional.

---

### Weeks 10-11: Making It Pretty
**What you're doing:** Getting your report game tight

- Run another full mock engagement on a different lab
- Find some real pentest reports online (redacted ones) and see how yours stacks up
- Practice explaining your findings out loud. Seriously, talk to your rubber duck about RCE

---

### Week 12: Final Prep
**What you're doing:** Getting exam-ready

- Review all your notes and cheatsheets
- Warm up with 2-3 medium boxes
- Make sure your report template is dialed in
- Check that your screenshot process is smooth

---

## Daily Grind

Here's how to spend those 4-5 hours:
- **1 hour:** Reading/watching course content (or reviewing if you're ahead)
- **2-3 hours:** Actually hacking stuff
- **30-60 mins:** Writing up what you found

Don't skip the writeup part. You'll hate yourself during the exam if you do.

---

## The Actual Roadmap

### Step 1: Foundations (You Probably Know This Already)

The basics - networking, Linux/Windows, common tools. PEH covers all this. Don't skip the labs even if you think you know it. There's always something new.

### Step 2: OSINT (Don't Sleep on This)

Learn to stalk companies properly (legally). Use theHarvester, Amass, Hunter.io, LinkedIn, breach databases. Practice on real companies BUT DON'T TOUCH THEIR SYSTEMS. Just collect public info.

You should be able to build a target profile before you even run nmap.

### Step 3: External Attacks

Figure out scoping and rules of engagement - the exam tests this.

Practice on:
- HTB boxes (start easy, work up to medium)
- Old VulnHub machines
- Anything that looks like a real external network

Take notes on everything. Future you will thank present you.

### Step 4: Active Directory (This Is Where People Fail)

Build a lab:
- One DC
- 2+ Windows boxes
- Make it vulnerable (weak passwords, kerberoastable accounts, etc.)

The attack chain you need to master:
1. Get in (phishing sim, password spray, whatever)
2. Escalate privileges locally
3. Move laterally (pass-the-hash, kerberos tickets, etc.)
4. Own the domain
5. Maintain access

Tools you MUST know cold:
- Impacket suite (especially secretsdump, psexec, wmiexec)
- Mimikatz (or at least know when to use it)
- BloodHound/SharpHound
- Responder
- CrackMapExec

HTB Pro Labs are expensive but worth it. VHL is cheaper and still good.

### Step 5: Report Writing (This Matters More Than You Think)

TCM gives you a template. USE IT.

For every box/lab:
- Executive summary (explain it like the CEO needs to understand)
- Technical details with screenshots
- Real-world impact
- How to fix it (be specific)

Find real pentest reports online and copy their style (not their content).

### Step 6: Full Mock Runs

Do the whole thing:
- Fake OSINT on a fake company
- External enumeration
- Pop a box
- Pivot inside
- Own AD
- Write the report
- Present findings (even if just to your cat)

This is what the exam actually tests - being a consultant, not just a script kiddie.

---

## Resources That Don't Suck

**For AD Practice:**
- HTB Pro Labs (Offshore, RastaLabs) - pricey but legit
- Virtual Hacking Labs - decent and cheaper
- Your own lab - free but takes setup time

**For General Practice:**
- HTB regular boxes
- VulnHub (download and run locally)
- THM if you need more hand-holding

**For OSINT:**
- TraceLabs old CTFs
- OSINTCurio.us challenges
- Google dorking playground

**For Reports:**
- TCM's template (use this for the exam)
- Any redacted pentest report you can find
- Your own notes from every box

---

## Real Talk

The PNPT is a 5-day exam plus 2 days for the report. It's not about being elite - it's about being methodical and professional.

Things that actually matter:
- AD knowledge (like 40% of the exam)
- Report quality (they actually read this)
- Time management (5 days goes fast)
- Screenshots of EVERYTHING
- Explaining business impact, not just "I got root"

Things people mess up:
- Rushing through OSINT
- Not practicing report writing until the end
- Forgetting to screenshot their process
- Writing reports like a techie instead of a consultant

---

## Final Thoughts

This cert is about proving you can do a real pentest, not just hack boxes. The technical stuff is maybe 60% of it. The other 40% is communication, documentation, and thinking like a business consultant who happens to hack things.

Stick to the schedule, practice the reports, and you'll be fine. The exam is tough but fair. If you can compromise an AD environment and write about it clearly, you'll pass.

Good luck. Now stop reading and go hack something.
