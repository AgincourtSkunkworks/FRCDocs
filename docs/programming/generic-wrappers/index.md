# Generic Wrappers

In FRC, we often need to interact with different electrical components to make the robot work, such as motor controllers and joysticks (or other input devices). We may also switch between different variants of these components relatively often. To both make the process of switching easier & faster (which is important in competition), and reduce the amount of different libraries we need to remember how to use, we can create generic wrappers for these components.

The idea is to create a class with generic functions that cover the functionality we need access to, and map these functions to the different library-specific functions that we need to call to make that component work. Then, we would specify which type of component we are using in a configuration file, and the wrapper would automatically use the correct implementations for that component. If needed, additional specifics like library enums can also be generalized and mapped to the correct values.

This does come with the difficulty of ensuring that there is feature parity between the different libraries, so if one library we have support for has a feature but another doesn't, we may not be able to use that feature in our generic. However, by doing this, we ensure the code remains consistent and flexible, which is vital in fast-paced, high-stress environments like competitions.
