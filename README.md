# PromptMaker

Tool to make contributing to popsauce easy.

Outil permettant de faciliter la création de questions pour popsauce.

## Installation

Extract the zip

To start the program, in the bin folder

On Windows:

```
launcher.bat
```
On Mac/Linux:

In terminal
```
launcher
```

## Usage
![example](https://github.com/esteb4nned/promptmaker/assets/31979112/4af89e8a-7b3c-4c90-b666-f77f8660bdca)
| Parameter       | Description                                                                                |
| :-------------- | :----------------------------------------------------------------------------------------- |
| Filename        | By default file(s) are named from the first answer you typed in the answer area.           |
| Custom filename | In most cases custom filename is unneeded. Example of use case is for prompts asking to complete lyrics or characters from movies/series where you have to set the source as filename. |
| Image selection | Copy and set the image name the same as the generated json.                                |
| Resize          | **\*\*Experimental\*\*** You might be better off using other way to resize your image.     |
| Text content    | For text type prompt (i.e quotes, lyrics)                                                  |
| Answer(s)       | Answer(s) should be typed each on a **separate line**.                                     |
| Short(s)        | Shorthand(s) if added should be **separated by a comma** "**,**"                           |
| Tag editor      | If tags are missing for automated input you can edit them or choose to use manual input.   |

If no image has been selected, the program only generate a json file.

## Example output

Image prompt

```json
{
  "prompt": "What movie is this image from?",
  "text": null,
  "source": [
    "movie name"
  ],
  "shorthand": [],
  "details": "w/e fit your description",
  "submitter": "test",
  "tags": [
    "Mainstream",
    "Easy",
    "Movies"
  ]
}
```

Text prompt
```json
{
  "prompt": "What movie is this quote from?",
  "text": "i.e random quote or song lyrics.",
  "source": [
    "w/e movie name"
  ],
  "shorthand": [],
  "details": "",
  "submitter": "test",
  "tags": [
    "Mainstream",
    "Medium",
    "Movies"
  ]
}
```

## Todo

- resizer (still a work in progress)

## Compiling

To compile the project by yourself you need the dependencies used to be modular. I provide the one i made in the modular folder.

```bash
mvn clean javafx:jlink
```
