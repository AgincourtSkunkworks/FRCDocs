# Bang-Bang Control

--8<-- "incomplete.md"

Bang-Bang control, or on-off control is a very simple control algorithm with two possible states, on or off. It switches between these two states based on a particular condition, usually the error between the desired and actual values.

## Use Cases
Bang-Bang control is a simple but effective control algorithm when used in the right context. It is most suited for applications where the system's behaviour can be easily achieved by switching the system on or off based on certain conditions. Here are some scenarios where Bang-Bang control may be used in FRC:

- Driving a set time at a constant speed
- Spinning the intake motors while a game piece is detected
- Turning on the shooter motors when a game piece is detected in the shooter mechanism

You'll notice that these usecases are all binary in nature, where the system's activation is based on whether a simple condition is met or not. Bang-Bang control will not be able to account for complex scenarios or where external factors may affect the system's behaviour. In those cases, more sophisticated control such as PID should be considered instead.

## Theory
### Principle


### Signals


### Tolerance (Hysteresis)


## Implementation


## Helpful Links
- [Wikipedia](https://en.wikipedia.org/wiki/Bang%E2%80%93bang_control)
