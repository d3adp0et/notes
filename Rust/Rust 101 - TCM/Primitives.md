# Primitives (Scalar Types)

- Integer
- Float
- Boolean
- Character

## Integer
unsigned: never negative - u8, u16, u32, u64, u128, usize
signed: can be negative and positive - i8, i16, **i32**, i64, i128, isize

eg: println!("Max size of a u32: {}", u32::MAX);  //the brackets are placeholder


## Floats 
-f32 (a 32-bit floating-point number, which can represent values with a precision of roughly 7 decimal digits.)
-**f64** (a 64-bit floating-point number, which can represent values with a precision of roughly 16 decimal digits.)

## Boolean (bool)
- true/false; 0/1
- comparison: ==; !=; <; >; <=; >= 
- logical: &&; ||; !
- simple if-else:
	
  ```
  let x = 15; 
  if x > 10 { 
    println!("x is greater than 10");
  }
  ```
## Character (char)
- not string