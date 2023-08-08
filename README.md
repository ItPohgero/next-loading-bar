\# Next Loading Bar

Next Loading Bar is a component that displays a loading bar during navigation between routes in a Next.js application.

\## Installation

You can install the package using npm:

\`\`\`bash
npm install next-loading-bar
\`\`\`

\## Usage

Import the \`NextLoadingBar\` component and use it in your application:

\`\`\`jsx
import NextLoadingBar from 'next-loading-bar';

// ...

<NextLoadingBar />
\`\`\`

\## Props

\| Prop \| Type \| Default \| Description \|
\|-------------------\|----------------------------------------\|-------------\|--------------------------------------------------------------------------------------------------------\|
\| \`position\` \| \`'top' \| 'bottom'\` \| \`'top'\` \| The position of the loading bar. \|
\| \`color\` \| \`string\` \| \`'#29D'\` \| The color of the loading bar. \|
\| \`startPosition\` \| \`number\` \| \`0.3'\` \| The start position of the loading bar. \|
\| \`stopDelayMs\` \| \`number\` \| \`200\` \| The stop delay in milliseconds. \|
\| \`height\` \| \`number\` \| \`3\` \| The height of the loading bar. \|
\| \`showOnShallow\` \| \`boolean\` \| \`true\` \| Whether to show the loading bar on shallow routes. \|
\| \`options\` \| \`Partial<NProgress.NProgressOptions>\` \| \`null\` \| Other NProgress configuration options to pass to NProgress. \|
\| \`nonce\` \| \`string\` \| \`undefined\` \| The nonce attribute to use for the \`style\` tag. \|
\| \`transformCSS\` \| \`(css: string) => JSX.Element\` \| See below \| Use your custom CSS tag instead of the default one. \|

The \`transformCSS\` prop allows you to provide a custom CSS tag.

\`\`\`jsx
// Example usage of transformCSS
<NextLoadingBar
transformCSS={(css) => <style nonce={nonce}>{css}</style>}
/>
\`\`\`

\## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
