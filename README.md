# artsy2

A suggestion of how the artsy folder structure could be

This project does not "run" it's just copy paste of code to showcase structure

## Palette

We want to swift toward a less copy paste approach and have things developed once and reuse them.

#### You may be thinking:

"But why is copy and pasting a bad idea? My code works and I don't need to go around different folders, I can just quickly define things locally"
So why is this a bad idea?

- It does take up extra developer time to create components from scratch when we could just reuse them
- It makes our code more prone to errors since all the component definitions need to be debugged in a case of a bug/error. Maybe we fix the component in one place where it's currently breaking but we forget to fix it in another place?
- Same goes for Design changes. Let's say the Designer decided to change something we then need to go and find every locally defined component and update it, while we could just update it one time if it was defined in a central place of information

In sort: Extra development time, more errors, harder to update designs. Less cohesion between the project.

#### Solution: Atomic Design

We want to define components once and import them to whenever we need to use them.

Using an [Atomic Design] Pattern can help us structure that in an intuitive way instead of defining everything in a flat higherarchy.

### How to think about atoms, molecules and organisms?

If it uses an atom, it's a molecule.

If it uses a molecule, it's an atom.

And so on.

These definitions are just there as a guideline and not supposed to be super strict.

### Design as a Guideline

We also want to follow the same idea as we have on the [Design], in Figma

[Atoms]: Buttons, radios, checkboxes, dropdown menus, input, icons, banners, tiles, pills

[Molecules]: headers, carousels, content, editorial

Atoms and Molecules are the suggested ones, but if we want to take it a step further we can also consider Organisms, Templates and Pages

[organisms]: grids

[Templates]: auctions, fairs, galleries

[Pages]: Home, Fairs, Auctions, Sell With Artsy

[design]: https://www.figma.com/file/m6gDpKHEWDbYJyrwsVZDBr/Artsy-3.0-Design-System?node-id=2%3A614
[atomic design]: https://www.notion.so/artsy/Atomic-Design-Principles-fc6b4d56ff8a4c218b1d46e753bc0e4b?d=472f60caaf43422988d63b0b5f71abf6#96bb4a22c61547e2890d934a82db6c81
[atoms]: https://www.figma.com/file/m6gDpKHEWDbYJyrwsVZDBr/Artsy-3.0-Design-System?node-id=2%3A614
[molecules]: https://www.figma.com/file/m6gDpKHEWDbYJyrwsVZDBr/Artsy-3.0-Design-System?node-id=1004%3A1354
[organisms]: https://www.figma.com/file/m6gDpKHEWDbYJyrwsVZDBr/Artsy-3.0-Design-System?node-id=1305%3A725
[templates]: https://www.figma.com/file/m6gDpKHEWDbYJyrwsVZDBr/Artsy-3.0-Design-System?node-id=1002%3A729
[pages]: https://www.figma.com/file/m6gDpKHEWDbYJyrwsVZDBr/Artsy-3.0-Design-System?node-id=5245%3A2952
