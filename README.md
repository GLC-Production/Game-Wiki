# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Write new Category

To create a category (folder) in `docs/`:

1. Make a folder under `docs/`, for example `docs/my-category/`.
2. Add a `_category_.json` file inside the folder to configure label/order and an optional generated index:

```json
{
	"label": "My Category",
	"position": 2,
	"link": {
		"type": "generated-index",
		"description": "Overview of My Category"
	}
}
```
3. Put your docs in that folder. Each file can include `sidebar_position` to control ordering within the category.

Preview with `yarn start` and verify the sidebar reflects the new category and pages.

For more details, see the official Docusaurus docs: https://docusaurus.io/docs/sidebar
