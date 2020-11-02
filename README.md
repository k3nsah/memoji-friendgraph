# Memoji Friendgraph

The idea was to create a simple, undirected, graph of some of my friends in the CS, ITI, and Engineering communities. I wanted a way to visually represent my semi-professional `network` of people in the form of a fun project. You can view a [live demo](https://www.kelcimensah.dev/projects/friendgraph) here to see how it looks!

![Kelci's Memoji Friendgraph](https://github.com/k3nsah/memoji-friendgraph/blob/main/friendgraph%20screenshot.png)

## Setup
This project uses the [Vis.js](https://visjs.org/) javascript library to build the interactive graph and Apple's trademark [Memoji](https://support.apple.com/en-us/HT208986) stickers as personalized image nodes to represent each person:

#### 1. create a directory - all of your files will need to be in the same directory (folder)
#### 2. create an `index.html` file
> This file is the boilerplate which will be used to display the javascript graph. 
#### 3. place the following script in the `<head>` tag
> ``` <script src="https://cdnjs.cloudflare.com/ajax/libs/vis/4.19.1/vis.min.js"></script> ```
> 
> This references [Vis.js](https://visjs.org/), which is what we're using.
#### 4. create `friendgraph.js` (in this repository, its labeled `memoji_friendgraph.js`)
#### 5. adjust edges of graph in the code
> The connected line between two nodes, or memoji people in this case, is called an `edge`. You can edit the connection lines by reordering the destination points in the following section:
>
```javascript 
edges: [
  //person 1 == 1
  {from: 1, to: 2},
  {from: 1, to: 3},
  {from: 1, to: 4},
  {from: 1, to: 5}
]
```
> person 1 is connected to person 2, 3, 4, and 5. Simultaneously, person 2, 3, 4, and 5 are also all connected to person 1 in an `undirected` connection.

#### 6. add css to `index.html`
> Add CSS to your graph to style it. Here's something you might want to add:
> * use `border: 1px solid #c4c4c4` since the graph automatically comes without a border, so you can't tell where your transparent canvas ends.

## Future Updates
- [ ] convert nodes to become clickable
- [ ] reorganize order of edges for neatness

## Resources
* [Vis.js](https://visjs.org/) JavaScript Library
* [Apple's Memoji](https://apps.apple.com/us/story/id1445637997) Stickers
