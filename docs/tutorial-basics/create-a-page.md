---
sidebar_position: 1
---

# Create a Page

## Page Details



- `src/components/research.js`
- `src/pages/footer.js`

## Create your first React Page

Create a file at `src/components/my-react-page_name.js`:

```jsx title="src/pages/my-react-page.js"
import React from 'react';
import Layout from '@theme/Layout';

export default function MyReactPage() {
  return (
    <Layout>
      <h1>My React page</h1>
      <p>This is a React page</p>
    </Layout>
  );
}
```

A new page is now available at [http://localhost:3000/my-react-page_name](http://localhost:3000/my-react-page).
