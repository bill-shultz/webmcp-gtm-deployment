# Chrome DevTools — WebMCP Tool Registration

Screenshots confirming WebMCP Tools deployed via Google Tag Manager Custom HTML tags are registering and firing correctly in Chrome, on live sites where I have full backend access and control.

## webmcp-setup-context-gtm-tag.jpg

Shows `navigator.modelContext.registerTool()`: "fixforu_guidelines" firing on [www.fixforu.com](https://www.fixforu.com) — Jackson Enterprises — using Chrome DevTools to confirm the GTM-deployed Setup Context Tag registered successfully in the browser. This tag returns mandatory context and rules about Jackson Enterprises and the website, including accurate business information, the correct company address, service areas, services provided, the correct phone number, and experience.

## webmcp-setup-context-tag.jpg

Shows `navigator.modelContext.registerTool()`: "fixforu_guidelines" firing on [www.fixforu.com](https://www.fixforu.com) — Jackson Enterprises — using Chrome DevTools to confirm the GTM-deployed tag registered successfully in the browser for the purpose of clarifying information about the site to AI Agents.

## webmcp-tool-chrome-ext-1.jpg

Shows `navigator.modelContext.registerTool()`: "checkServiceArea" firing on [www.fixforu.com](https://www.fixforu.com) — Jackson Enterprises — using Chrome DevTools to confirm the GTM-deployed tag registered successfully in the browser. This tag is designed to help AI Agents validate whether Jackson Enterprises services a given geographic area.

## webmcp-tool-chrome-ext-2.jpg

Shows `navigator.modelContext.registerTool()`: "checkServiceArea" firing on [www.fixforu.com](https://www.fixforu.com) — Jackson Enterprises — confirming that "Christiansburg" is a service area for Jackson Enterprises. This also shows how to run the tool by entering the word "christiansburg" into Chrome DevTools.

## webmcp-tool-chrome-ext-3.jpg

Further validation showing `"success": true, "message": "Yes! Christiansburg is a supported service area."`

## webmcp-tool-chrome-ext-4-ny.jpg

Shows `navigator.modelContext.registerTool()`: "checkServiceArea" firing on [www.fixforu.com](https://www.fixforu.com) — Jackson Enterprises — testing whether Jackson Enterprises services "New York." New York is not a service area of Jackson Enterprises. The WebMCP tool is specifically designed to confirm that only certain geographic areas in and around Christiansburg, Virginia are serviced by Jackson Enterprises.

## webmcp-tool-chrome-ext-5-no.jpg

Shows `navigator.modelContext.registerTool()`: "checkServiceArea" firing on [www.fixforu.com](https://www.fixforu.com) — Jackson Enterprises. This test helps the AI Agent understand and communicate that Jackson Enterprises does not provide services to New York. Note the output specifically shows "christiansburg" as "Yes!" and "new york" as "not found." AI Agents learn more about Jackson Enterprises' services and service area using these WebMCP Tools.

## Additional notes

I've also deployed a WebMCP Tool called "verifyPageService" on this site, along with WebMCP Tools on other websites using Google Tag Manager. This is still experimental — I'll continue adding more screenshots and notes as testing continues.
