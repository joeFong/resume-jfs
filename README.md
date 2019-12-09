# resume-jf

A Svelte webcomponent to easily create a new beautiful resume and embed it on your website or print it as a pdf.

### Basic Usage
Go to my website https://joefong.xyz to see what the 'resumeObj' object looks like.
```sh
<script>
    import ClassicTheme from './ClassicTheme.svelte';
</script>
<ClassicTheme {...resume}/>
```
### Static
Include script in head or body
```sh
<script src="/path/to/file/resume-jfs/build/bundle.js"></script>
```
### CDN
Include script in head or body
```sh
<script src="https://cdn.jsdelivr.net/npm/resume-jf@1.0.0/dist/resume-jfs.js"></script>
```
### Installation
Install the dependencies and devDependencies and start the server.

```sh
$ npm i resume-jfs
```

### Attributes
- `theme` - only has 'classic' theme for now.
- `resume` - a JSON object passed in as a spread prop. 

### Todos

 - Write Tests
 - Add Themes
 - A form to generate resume for users that don't want to deal with JSON 

License
----

ISC
**Free Software, Hell Yeah!**
