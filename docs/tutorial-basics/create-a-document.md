---
sidebar_position: 2
---

# Create a Document

Documents are **groups of pages** connected through:

- a **sidebar**
- **previous/next navigation**
- **versioning**

## Create your first Doc

Create a Markdown file at `documentation/docs_name.md`:

```md title="documentation/docs_name.md"
# Hello

This is my **first Practicant document**!
```

A new document is now available at [http://localhost:3000/documentation/docs_name](http://localhost:3000/documentation/docs_name).

## Configure the Sidebar

Practicant automatically **creates a sidebar** from the `documentation` folder.

Add metadata to customize the sidebar label and position:

```md title="documentation/docs_name.md" {1-4}
---
sidebar_label: 'Documentation_Details'
sidebar_position: 3
---

# Hello

This is my **first Practicant document**!
```

It is also possible to create your sidebar explicitly in `sidebars.js`:

```js title="sidebars.js"
module.exports = {
  tutorialSidebar: [
    'intro',
    // highlight-next-line
    'hello',
    {
      type: 'category',
      label: 'Tutorial',
      items: ['tutorial-basics/create-a-document'],
    },
  ],
};
```
