# Zykov

**A graph-oriented language for semantic curatorial publishing on the web.**

Zykov is a programming language for constructing semantic graphs, narrative structures, curatorial archives, interconnected blogs, and exploratory hypertextual spaces through algebraic graph expressions.

Its companion compiler, **Zygrafi**, transforms `.zyk` scripts into interactive semantic publications with:
- graph visualization,
- room navigation,
- topic filters,
- interconnected entries,
- hypertext references,
- editorial layouts,
- and curatorial reading interfaces.

---

# Philosophy

Zykov treats graphs not only as data structures, but as navigable narrative spaces.

A graph in Zykov can simultaneously become:
- a semantic archive,
- an interconnected diary,
- a curatorial exhibition,
- a conceptual atlas,
- a semantic notebook,
- or a digital publication.

The language is inspired by:
- algebraic graph theory,
- semantic hypertext,
- curatorial design,
- ergodic literature,
- experimental interfaces,
- and graph-based visual exploration.

---

# Installation

## Requirements

- Node.js 18+
- npm
- Visual Studio Code (optional, for syntax highlighting)

---

## Install globally

From the root folder:

```bash
./setup.sh
```

This installs:
- `zygrafi`
- `zykov`
- VS Code syntax highlighting
- demo builds

---

# Try this

Create a file called `hello-world.zyk`:

```zyk
Title = "Hello Zygrafi"

Background = "#dfe7e1"

Categories = {
  day1 -> "#4db6ac",
  semantic -> "#ce93d8"
}

NodesColor = {
  entries -> "#34495e",
  general -> "#5d6d7e"
}

EdgesColor = "#7ac9a2"

Layout = "forceAtlas"

A :: day1
B :: semantic
C

Room = A * (B + C)

roomData "Main Room" = {
  Title: "Hello Zygrafi",
  Text: "A semantic graph publication generated with Zykov."
}

entry A = {
  Title:"First Entry",
  Text:"This is a semantic publication node."
}

entry B = {
  Title:"Semantic Publishing",
  Text:"Zykov transforms graph structures into navigable curatorial spaces."
}

gallery = {
  Room -> "Main Room"
}
```

Then compile:

```bash
zygrafi publish hello-world.zyk
```


---

# Example Projects

Included examples:
- `hello.zyk`
- `living-gallery.zyk`
- `wipeout_soundtrack.zyk`
- `note-lab-example.zyk`

---

# Galleries

Here are some galleries to explore:
1. [Computers, Anthropology and Sneakers: A Map Gallery](https://stackblitz.com/edit/stackblitz-starters-xlrqanaa?embed=1&file=index.html&hideExplorer=1&view=preview)
2. [Wipeout: Music, Lore and Tracks](https://stackblitz.com/edit/stackblitz-starters-udiv5vcl?embed=1&file=index.html&hideExplorer=1&view=preview)
3. [A modo de Blog Semántico (Abril 2026)](https://stackblitz.com/edit/stackblitz-starters-bcspbqee?embed=1&file=index.html&hideExplorer=1&view=preview)
---

# Available layouts

```zyk
Layout = "circular"
Layout = "grid"
Layout = "force"
Layout = "forceAtlas"
Layout = "random"
Layout = "concentric"
Layout = "radial"
Layout = "arc"
```

Layouts in Zykov are not only geometric arrangements:
they are reading strategies for semantic navigation.

---

# VS Code Syntax Highlighting

The project includes:
- `.zyk` syntax support
- the `Zykov Exhibit` theme

To manually install the extension:

```bash
./scripts/install-vscode-extension.sh
```

Then:
1. restart VS Code,
2. open a `.zyk` file,
3. select:
   `Preferences → Color Theme → Zykov Exhibit`

---

# License

Zykov is licensed under the GNU AGPL-3.0.

This guarantees that:
- derivative systems remain open,
- network-based deployments preserve attribution,
- and semantic publication ecosystems derived from Zykov remain part of the open commons.

---

# Credits

Zykov language developed by Alfonso Bustamante.

Based on the paper:

> *A Zykov Algebra Approach to Clique Propagation*  
> Discrete Mathematics, Algorithms and Applications  
> World Scientific, May 2025.

Repository:
https://github.com/Anekemuthep/Zykov

Website:
https://alfonsobustamante.com/

Published article:
https://www.worldscientific.com/doi/10.1142/S1793830925500806
