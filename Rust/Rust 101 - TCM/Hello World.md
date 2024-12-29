# Hello World


### Cargo
- cargo is the rust package manager
- syntax: cargo new projet_name
- makes the file with two folders src(main.rs) and target(.toml files)
- RUN: 
	```
	fn main() {
		println!"("Hello, world!");
	}
	```
- syntax: cargo run

## Main Function(fn) & Macros

- main fn
- macros are small functions
- println vs print ; println has breaks after every line while print does not
	- eg.: println!("hello world!")
	       println!("hello world!")
	       /\*[hello world!
		  hello world!]\*/
	- eg.: print!("hello world!")
	       print!("hello world!")
	       //[hello world!hello world!	

### **comments you can see above how to use (both multi-line and single-line)**

## Errors

- 'rustc --explain error_code'
- 
