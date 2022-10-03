# tdei-docs

To add a new markdown file do the following.

1. Create a markdown file and add the following on the top as mentioned in the example-1.md file.

layout: default
title: <title>


2. Go to sidebar.html in _includes folder. Add the following code in any of the category to add the new link. Replace file name and link name

```
 <li>
          <a
            href="/tdei-docs/<file-name>"
            class="d-inline-flex align-items-center rounded"
            ><link name></a
          >
        </li>
```

3. To create new category, Go to sidebar.html in _includes folder, add the following code a line above last </ul> and replace the links names and file names

```
<li class="mb-1">
      <button
        class="btn d-inline-flex align-items-center rounded collapsed"
        data-bs-toggle="collapse"
        data-bs-target="#getting-started-collapse"
        aria-expanded="false"
      >
        Getting started
      </button>

      <ul class="list-unstyled fw-normal pb-1 small">
        <li>
          <a
            href="/tdei-docs/example-1"
            class="d-inline-flex align-items-center rounded"
            >Introduction</a
          >
        </li>
        <li>
          <a
            href="/tdei-docs/example-2"
            class="d-inline-flex align-items-center rounded"
            >Download</a
          >
        </li>
      </ul>
    </li>
```
