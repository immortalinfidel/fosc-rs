# Forecast Oscillator (FOSC)
 ```
use fosc_rs::FOSC;
use ta_common::traits::Indicator;


let mut fosc = FOSC::new(5);
assert_eq!(fosc.next(81.59), None);
assert_eq!(fosc.next(81.06), None);
assert_eq!(fosc.next(82.87), None);
assert_eq!(fosc.next(83.00), None);
assert_eq!(fosc.next(83.61), None);
assert_eq!(fosc.next(83.15), Some(-1.2868310282621687));
assert_eq!(fosc.next(82.84), Some(-1.6586190246257615));
assert_eq!(fosc.next(83.99), Some(1.0346469817835624));
assert_eq!(fosc.next(84.55), Some(1.0277942046126718));
assert_eq!(fosc.next(84.36), Some(-0.0995732574679644));
assert_eq!(fosc.next(85.53), Some(0.5997895475271895));
assert_eq!(fosc.next(86.54), Some(0.6482551421308311));
assert_eq!(fosc.next(86.89), Some(0.08286339049376355));
assert_eq!(fosc.next(87.77), Some(0.157229121567756));
assert_eq!(fosc.next(87.29), Some(-1.5832283193950765));






```