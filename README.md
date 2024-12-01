# Framer Motion Properties Guide

A comprehensive guide to Framer Motion properties with clear descriptions and examples.

---

## Animation Properties

| <span style="color:blue">**Property**</span> | <span style="color:green">**Type**</span> | <span style="color:purple">**Description**</span> | <span style="color:orange">**Example**</span> |
|---------------------------------------------|------------------------------------------|--------------------------------------------------|-----------------------------------------------|
| `initial`                                   | Object                                   | Initial state before animation                  | `initial={{ opacity: 0 }}`                    |
| `animate`                                   | Object                                   | Target state for animations                     | `animate={{ opacity: 1 }}`                    |
| `exit`                                      | Object                                   | Animation when component is removed            | `exit={{ opacity: 0 }}`                       |
| `transition`                                | Object                                   | Controls animation timing and type             | `transition={{ duration: 0.5, type: "spring" }}` |

---

## Interaction Animations

| <span style="color:blue">**Property**</span> | <span style="color:green">**Type**</span> | <span style="color:purple">**Description**</span> | <span style="color:orange">**Example**</span> |
|---------------------------------------------|------------------------------------------|--------------------------------------------------|-----------------------------------------------|
| `whileHover`                                | Object                                   | Animations during hover state                   | `whileHover={{ scale: 1.1 }}`                 |
| `whileTap`                                  | Object                                   | Animations during press/tap                     | `whileTap={{ scale: 0.9 }}`                   |
| `whileDrag`                                 | Object                                   | Animations while dragging                       | `whileDrag={{ scale: 1.2 }}`                  |

---

## Gesture Properties

| <span style="color:blue">**Property**</span> | <span style="color:green">**Type**</span> | <span style="color:purple">**Description**</span> | <span style="color:orange">**Example**</span> |
|---------------------------------------------|------------------------------------------|--------------------------------------------------|-----------------------------------------------|
| `drag`                                      | Boolean/String                          | Enables dragging                                | `drag={true}` or `drag="x"`                   |
| `dragConstraints`                           | Object                                   | Limits drag movement                            | `dragConstraints={{ left: 0, right: 300 }}`   |
| `dragElastic`                               | Number                                   | Bounce-back effect during dragging             | `dragElastic={0.7}`                           |
| `dragMomentum`                              | Boolean                                  | Enables momentum after dragging                | `dragMomentum={true}`                         |

---

## Variant-Based Animations

| <span style="color:blue">**Property**</span> | <span style="color:green">**Type**</span> | <span style="color:purple">**Description**</span> | <span style="color:orange">**Example**</span> |
|---------------------------------------------|------------------------------------------|--------------------------------------------------|-----------------------------------------------|
| `variants`                                  | Object                                   | Predefined animation states                     | `variants={containerVariants}`                |
| `initial` (variant)                         | String                                   | Initial variant state                           | `initial="hidden"`                             |
| `animate` (variant)                         | String                                   | Current variant state                           | `animate="visible"`                            |
| `exit` (variant)                            | String                                   | Exit variant state                              | `exit="exit"`                                  |

---

## Transition Properties

| <span style="color:blue">**Property**</span> | <span style="color:green">**Type**</span> | <span style="color:purple">**Description**</span> | <span style="color:orange">**Example**</span> |
|---------------------------------------------|------------------------------------------|--------------------------------------------------|-----------------------------------------------|
| `type`                                      | String                                   | Animation type                                  | `type: "tween"` or `type: "spring"`           |
| `duration`                                  | Number                                   | Animation duration in seconds                  | `duration: 0.5`                               |
| `delay`                                     | Number                                   | Delay before animation starts                  | `delay: 0.2`                                  |
| `ease`                                      | String/Function                          | Easing function                                 | `ease: "easeInOut"`                            |
| `staggerChildren`                           | Number                                   | Delay between child animations                 | `staggerChildren: 0.1`                         |

---

## Layout Properties

| <span style="color:blue">**Property**</span> | <span style="color:green">**Type**</span> | <span style="color:purple">**Description**</span> | <span style="color:orange">**Example**</span> |
|---------------------------------------------|------------------------------------------|--------------------------------------------------|-----------------------------------------------|
| `layout`                                    | Boolean/String                          | Enables layout animations                       | `layout={true}`                                |
| `layoutId`                                  | String                                   | Shared layout between components               | `layoutId="unique-identifier"`                |
| `layoutTransition`                          | Object                                   | Customizes layout animation                    | `layoutTransition={{ type: "spring" }}`       |

---

## Scroll-Triggered Animations

| <span style="color:blue">**Property**</span> | <span style="color:green">**Type**</span> | <span style="color:purple">**Description**</span> | <span style="color:orange">**Example**</span> |
|---------------------------------------------|------------------------------------------|--------------------------------------------------|-----------------------------------------------|
| `viewport`                                  | Object                                   | Trigger animations on scroll                    | `viewport={{ once: true }}`                   |
| `whileInView`                               | Object                                   | Animations when in viewport                     | `whileInView={{ opacity: 1 }}`                |

---

## Event Handlers

| <span style="color:blue">**Property**</span> | <span style="color:green">**Type**</span> | <span style="color:purple">**Description**</span> | <span style="color:orange">**Example**</span> |
|---------------------------------------------|------------------------------------------|--------------------------------------------------|-----------------------------------------------|
| `onHoverStart`                              | Function                                 | Callback on hover start                         | `onHoverStart={() => console.log('Hover started')}` |
| `onHoverEnd`                                | Function                                 | Callback on hover end                           | `onHoverEnd={() => console.log('Hover ended')}` |
| `onTap`                                     | Function                                 | Callback on tap/click                           | `onTap={() => console.log('Tapped')}`          |
| `onDragStart`                               | Function                                 | Callback when dragging starts                  | `onDragStart={() => console.log('Drag started')}` |

---

