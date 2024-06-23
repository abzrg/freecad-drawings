# Model 1

On object can be created in a number of different ways.
For any new object we need to examine it and decide which techniques we're going to use.
This involves breaking down the object into its individual parts.
To examine its best to look at it in each profiles of front side and top.


**workflow**:

1. create new document and save it with a name.
2. select the part design. there are two important tabs on the left:
  - model: each time a body or sketch or operation is added, they are shown in that tab
  - tasks: which guides you through part design process.
3. create a body.
4. create a sketch.
5. select the plane to start sketching in 2D plane.
  - xy: top view
  - xz: front
  - yz: right

...

**dress up actions**: fillet, chamfer. these actions should be done last of all just to finish off
  object.

**Model tab**:
- bold body the is the active body
- grayed out items are not visible.
- toggle visibility with space key.
- the green arrow on an item shows the *tip*, which is the very last action.

**Tasks tab**:
- solver message: this will change constantly when we place a geometry onto the screen.
  - the number of constraints are show. It can be in under, fully, or over constrained state. by
    clicking on the number one can see where the under or over constrained occurs. In the case of
    over constrained sketch one can click on the number and press 'DEL' key to remove the extra
    constraints and starts at a under constraints condition again.
- edit controls:
  - auto constraints ✓
  - avoid redundant auto constraints ✓

**right click**: cancels the selected tool and goes into the normal selection mode

**Constraints** can be *deleted* by first selecting them and then pressing 'DEL' key. Another ways is to
  select the constraints and go to the tasks tab, and under constraints and hit 'DEL' key.

view > toggle axis cross: depends on the first sketch's position.


**features**: with the desired sketch selected:
- Additive features
  - pad: adds materials similar to extrude in other CAD softwares
- Subtractive features
  - pocket: removes

To select a face to sketch on, click *once* on that face. Then proceed to create a sketch in tasks
tab.
- double click will select the whole body.

To have 4 circles have the same diameter/radius:
- select all four and apply the diameter constraint.
- constraint one circle's diameter and then select the other circles and use the equality
  constraints.

To bring or reference to external points (on other geometries/sketches), we use the 'external
geometry' button. (shortcut: gx)

We want the least number of *datum constraints* (those with data and measurement added to them: like
diameter constraints) in our sketch.

One can hide distance constraints by clicking on them and un-tick the constraints in the constraints
section in the tasks tab.

In the case of *pocket* feature, **To first** means: The pocket will extrude up to the first face of
the support in the extrusion direction

To **export** as stl, we select the tip action and, from file menu select the export entry.
We can export the previous actions and export the work until those actions as stl.
