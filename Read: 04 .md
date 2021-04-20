### What is CSS Grid : 

CSS Grid is a 2 dimensional layout system that can
handle both columns and rows. 


### Properties for the Parent : (Grid Container)

1. display
Defines the element as a grid container and establishes a new grid formatting context for its contents.

Values:
grid – generates a block-level grid
inline-grid – generates an inline-level grid

![](https://i.ibb.co/G04YjtT/grid2.png)

2. grid-template-columns
3. grid-template-rows
Defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.

Values:

`<track-size>` – can be a length, a percentage, or a fraction of the free space in the grid (using the fr unit)
`<line-name>` – an arbitrary name of your choosing

![](https://i.ibb.co/m9r1qgj/grid1.png)


## Terminology
1. grid container
2. grid item
3. grid line = The dividing lines that make up the structure of the grid.
4. grid track = column or row
5. grid cell = a single "unit" of the grid.
6. grid area = The total space surrounded by four grid lines. Can contain any number of cells.

## Container properties
`display` -> `grid | inline-grid | subgrid`

`grid-template-columns` / `grid-template-rows` = Defines the columns and rows of the grid with a space-separated list of values.
- `<track-size> ... | <line-name> <track-size> ...`
- can use: `repeat(#, ...)`
- The "fr" unit allows you to set the size of a track as a fraction of the free space of the grid container.

`grid-template-areas` = Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property.
```
.container {
  grid-template-areas: 
  "<grid-area-name> | . | none | ..."
  "...";
}
```

`grid-template` = shorthand for the above
- `none | subgrid | <grid-template-rows> / <grid-template-columns>`
```
.container {
  grid-template:
  [row1-start] "header header header" 25px [row1-end]
  [row2-start] "footer footer footer" 25px [row2-end]
  / auto 50px auto;
}
```
_Note: Since grid-template doesn't reset the implicit grid properties (grid-auto-columns, grid-auto-rows, and grid-auto-flow), 
       which is probably what you want to do in most cases, it's recommended to use the grid property instead of grid-template._

`grid-column-gap` / `grid-row-gap` = Specifies the size of the grid lines.
- `<line-size>`

`grid-gap` = shorthand for the above 
- `<grid-row-gap> <grid-column-gap>`

`justify-items` / `align-items` = Aligns the content inside a grid item along the row/column axis.
- `start | end | center | stretch`

`justify-content` / `align-content` = Set the row/column alignment of the grid within the grid container.

`grid-auto-columns` / `grid-auto-rows` = Specifies the size of any auto-generated grid tracks (aka implicit grid tracks).

`grid-auto-flow` = If you have grid items that you don't explicitly place on the grid, the auto-placement algorithm kicks in to automatically place the items.
- `row | column | row dense | column dense`

`grid` = shorthand for all the grid properties
- `none | <grid-template-rows> / <grid-template-columns> | <grid-auto-flow> [<grid-auto-rows> [/ <grid-auto-columns>]]`

## Item properties
`grid-column-start` / `grid-column-end` / `grid-row-start` / `grid-row-end` = determine item location
- `<number> | <name> | span <number> | span <name> | auto`

`grid-column` / `grid-row` = shorthand for the above
- `<start-line> / <end-line> | <start-line> / span <value>`

`grid-area` = Gives an item a name so that it can be referenced by a template created with the grid-template-areas property. Or shorthand for the above.
- `<name> | <row-start> / <column-start> / <row-end> / <column-end>`

`justify-self` / `align-self` = Aligns the content inside a grid item along the row/column axis.
- `start | end | center | stretch`
