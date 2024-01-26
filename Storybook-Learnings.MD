# Storybook Quickstart

## When storybook is right

Storybook is highly beneficial for frontend developers focused on building and refining UI components. It provides an isolated environment for developing and testing components, ensuring they function correctly across different states and scenarios without needing to embed them in your main application initially.
This isolation simplifies debugging and enhances component reusability.

Storybook also aids in creating a living documentation of components, making it easier for teams to understand and reuse code. It's especially useful in projects where visual consistency and component-driven development are critical, such as in large-scale applications or design systems.

> If the UI is not component driven, storybook can still be used, but the setup of stories might require more effort. More setup and scaffolding might be required to get the components to render in isolation.

## Common Scenarios

### Network request dependencies

Network requests can be mocked using (but not limit to) MSW or MirageJS. This allows the component to be rendered in isolation without needing to make a network request.

> It's important to setup correctly. These setups should happen within the [preview file](preview.js).

### Any other dependencies

Any other dependencies, such as context, wrappers (like containers), can be done using decorators. See [decorators](https://storybook.js.org/docs/writing-stories/decorators) for more information.
