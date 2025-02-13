# web-dev-starter

This is a website demonstrating accessibility.

## Getting Started

To get started, clone this repository and run the following commands:

```bash
npm install
```

This will install the necessary dependencies for the project.

## Development

It is recommended to use the VSCode Live Server extension to run the project
locally. This will allow you to see changes in real-time as you make them. There
is no need to run a build process or refresh the page manually. Additionally,
you do not need to setup a local server to run the project.

## Testing

To run the tests for the project, run the following command:

```bash
npm test
```

The tests should fail as JavaScript was not intended to work with this project.

## Accessibility Lab Answers

#### Color

The background and foreground of the page have issues. I ran the lighthouse scan on the site and it was reported that multiple tags
(too many to list) did not have sufficient contrast. I could not figure out a bunch more than that because chrome dev tools no longer allows you to see the contrast levels upon inspection of the html elements.

#### Keyboard

When navigating with a keyboard, you can actually do quite a lot. You can access all buttons, links, and text inputs fields just using tab, space, enter, and the arrow keys. I am not entirely sure what exactly is missing here, besides the text being way too small.

#### Semantic HTML

You have to change the `<div>` so it's using the `<nav>` tag.

#### Images

Added alt tags to images.

#### Audio

I made the audio downloadable for users whos browsers dont support HTML audio.

#### Forms

I added an aria-label to help identify the input form.

#### Show Comment Button

It already works to highlight it, so I just added a tabIndex to it which allowed me to be able to hit enter and use the button.

#### Table

I added some aria tags as well as identified the columns of the table using the scope="col" attribute.

#### Suggestions

1. Add some sort of language attribute for supporting multiple languages.
2. Use `<h1>` tags for main headings.
