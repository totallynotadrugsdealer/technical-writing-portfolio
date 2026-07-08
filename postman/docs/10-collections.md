A **Postman Collection** is one of the fundamental elements in Postman, used to save, organize, and share API requests. Collections help you group related requests together, collaborate with teammates, and streamline your API development workflows.

## What is a Collection?

A collection is a set of requests sent to API endpoints [^1]. It can also include:

- Saved responses from requests
- Each endpoint's authorization type, parameters, and headers
- Request bodies, tests, and settings [^1]

## What You Can Do with Collections

- **Create collections** from scratch or from Postman's predefined templates, to save frequently used requests or group requests for a specific purpose like testing or simulating workflows [^2]
- **Add API requests** — collections can contain HTTP requests, or you can create a multi-protocol collection with GraphQL, gRPC, and other request types [^2]
- **Organize requests** using folders and subfolders, drag-and-drop reordering, or alphabetical sorting [^3]
- **Collaborate** by sharing collections, watching for changes, tagging collections, and adding comments [^2]
- **View activity** on the collection's Overview tab, which shows a changelog, associated environments, monitors, and mocks [^2]

## Managing Collections

You can manage collections directly in the Postman sidebar by clicking **Items > Collections** [^3]. Key management actions include:

- Adding folders and subfolders to group requests
- Deleting collections (with the option to recover them from Trash)
- Reverting a collection to an earlier state using the changelog
- Bulk selecting multiple collections with **⌘** or **Ctrl** + click [^3]

## Collection Format

Postman Collections are based on an open source *collection format* that is both machine and human readable [^2]. This format can be used to generate client and server SDKs, documentation, and mock servers.

## Programmatic Management

You can also manage collections programmatically using the [Postman API](https://api.postman.com/). This allows you to add, delete, or update collections, transfer items between collections, manage forks and pull requests, and even import OpenAPI definitions to create collections [^4].

In summary, collections are the core organizational unit in Postman, enabling you to structure your API requests, collaborate with your team, and integrate with broader development workflows.

[^1]: https://learning.postman.com/docs/getting-started/basics/postman-elements
[^2]: https://learning.postman.com/docs/use/use-collections/overview
[^3]: https://learning.postman.com/docs/use/use-collections/manage-collections
[^4]: https://learning.postman.com/docs/reference/postman-api/intro-api
