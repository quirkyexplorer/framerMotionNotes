# Framer Motion Properties Reference

A comprehensive table of Framer Motion properties organized into categories.

## 1. Animation Properties

| **Property**    | **Type**                | **Description**                                                                                       | **Example**                                           |
|------------------|-------------------------|-------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| `animate`        | `string \| object`      | Defines the target visual state(s) for the component.                                                 | `<motion.div animate={{ opacity: 1 }} />`            |
| `initial`        | `string \| object`      | Sets the initial state before animation begins.                                                       | `<motion.div initial={{ opacity: 0 }} />`            |
| `exit`           | `string \| object`      | Defines the exit animation state for a component being removed.                                       | `<motion.div exit={{ opacity: 0 }} />`               |
| `transition`     | `object`               | Configures the timing and easing of an animation.                                                     | `<motion.div animate={{ x: 100 }} transition={{ duration: 1 }} />` |
| `whileHover`     | `object`               | Defines an animation that runs while the component is hovered over.                                   | `<motion.div whileHover={{ scale: 1.2 }} />`         |
| `whileTap`       | `object`               | Defines an animation that runs while the component is being tapped.                                   | `<motion.div whileTap={{ scale: 0.9 }} />`           |
| `whileDrag`      | `object`               | Defines an animation that runs while the component is being dragged.                                  | `<motion.div whileDrag={{ scale: 0.8 }} />`          |

---

## 2. Gestures Properties

| **Property**    | **Type**                | **Description**                                                                                       | **Example**                                           |
|------------------|-------------------------|-------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| `drag`           | `boolean`              | Enables dragging for the component.                                                                  | `<motion.div drag />`                                 |
| `dragConstraints`| `object`               | Restricts drag movement to specific boundaries.                                                      | `<motion.div drag dragConstraints={{ top: 0, left: 0 }} />` |
| `dragElastic`    | `number` \| `boolean`  | Determines how elastic the drag movement feels.                                                      | `<motion.div drag dragElastic={0.5} />`              |
| `dragMomentum`   | `boolean`              | Enables or disables drag momentum.                                                                   | `<motion.div drag dragMomentum={false} />`           |
| `onDragStart`    | `(event, info) => void`| Callback function triggered at the start of a drag.                                                  | `<motion.div drag onDragStart={() => console.log('Started!')} />` |
| `onDragEnd`      | `(event, info) => void`| Callback function triggered at the end of a drag.                                                    | `<motion.div drag onDragEnd={() => console.log('Ended!')} />` |

---

## 3. Layout Properties

| **Property**    | **Type**                | **Description**                                                                                       | **Example**                                           |
|------------------|-------------------------|-------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| `layout`         | `boolean`              | Enables layout animations when the component's size or position changes.                              | `<motion.div layout />`                               |
| `layoutId`       | `string`               | Links components for shared layout transitions.                                                      | `<motion.div layoutId="box" />`                      |
| `onLayoutAnimationStart` | `() => void`   | Callback when a layout animation starts.                                                             | `<motion.div layout onLayoutAnimationStart={() => {}} />` |
| `onLayoutAnimationComplete` | `() => void` | Callback when a layout animation completes.                                                          | `<motion.div layout onLayoutAnimationComplete={() => {}} />` |

---

## 4. Utilities

| **Property**    | **Type**                | **Description**                                                                                       | **Example**                                           |
|------------------|-------------------------|-------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| `variants`       | `object`               | Predefined animation states that can be referenced by `animate`, `initial`, and `exit`.               | `<motion.div variants={{ open: { opacity: 1 } }} />` |
| `custom`         | `any`                  | Passes custom data to animations, often used with variants.                                           | `<motion.div custom={index} animate="open" />`       |
| `style`          | `object`               | Inline styles for the motion component.                                                              | `<motion.div style={{ backgroundColor: 'red' }} />`  |
| `id`             | `string`               | Identifier for uniquely targeting motion elements.                                                   | `<motion.div id="motionBox" />`                      |

---

## 5. Keyframe Animations

| **Property**    | **Type**                | **Description**                                                                                       | **Example**                                           |
|------------------|-------------------------|-------------------------------------------------------------------------------------------------------|-------------------------------------------------------|
| `keyframes`      | `array`                | Defines multiple values for an animation to transition through.                                       | `<motion.div animate={{ x: [0, 50, 100] }} />`        |
| `repeat`         | `number`               | Number of times an animation should repeat.                                                          | `<motion.div animate={{ x: 100 }} transition={{ repeat: 2 }} />` |
| `repeatType`     | `string`               | Defines how the animation repeats (`loop`, `reverse`, `mirror`).                                      | `<motion.div transition={{ repeatType: 'reverse' }} />` |

---

## Notes

- Replace `motion.div` with any valid HTML tag, such as `motion.button` or `motion.svg`, to animate other elements.
- Combine properties for complex animations.

For more details, refer to the [Framer Motion documentation](https://www.framer.com/motion/).
