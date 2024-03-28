<script lang="ts">
  import Code from "./code.svelte";
  import Markdown from "./markdown.svelte";
  import Notes from "./notes.svelte";
  import Slide from "./slide.svelte";
</script>

<Slide>Horizontal Slide</Slide>

<Slide>
  <Slide>Vertical Slide 1</Slide>
  <Slide>Vertical Slide 2</Slide>
</Slide>

<Slide animate>
  <ul>
    <li>React</li>
    <li>Solid</li>
    <li>Svelte</li>
    <li>Vue</li>
  </ul>
</Slide>

<Slide animate>
  <ul>
    <li>Svelte ❤️</li>
    <li>React</li>
    <li>Solid</li>
    <li>Vue</li>
  </ul>
</Slide>

<Slide animate>
  <Code id="code" lines>
    {`
			function love() {}
	 `}
  </Code>
</Slide>

<Slide animate>
  <Code id="code" lines="2|1-3">
    {`
			function love() {
				console.log('Svelte')
			}
	 `}
  </Code>
</Slide>

<Markdown>
  {`
		## Markdown ❤️
		You can use **HTML** or **Markdown** for slides.
	`}
</Markdown>

<Markdown name="example.md" external />

<Slide animate>
  <p>This contains speaker notes</p>
  <p>Press S to see it</p>
  <ul>
    <li>Svelte ❤️</li>
    <li>React</li>
    <li>Solid</li>
    <li>Vue</li>
  </ul>
  <Notes>
    <ul>
      <li><b>This is a speaker note</b></li>
      <li><b>Avoid eye contact.</b></li>
    </ul>
  </Notes>
</Slide>
