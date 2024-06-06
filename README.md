# 📚 VSCode Personalization

## Current bracket guide {}

```json
{ 
    "[xml]": {
        "editor.defaultFormatter": "redhat.vscode-xml"
    },
    "redhat.telemetry.enabled": true,
    "[html]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "[javascript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode"
    },
    "workbench.colorTheme": "Tokyo Night",
    "git.confirmSync": false,
    "editor.bracketPairColorization.independentColorPoolPerBracketType": true,
    "editor.guides.bracketPairs": true,
    "editor.guides.highlightActiveBracketPair": true,
    "editor.guides.highlightActiveIndentation": true,
}
```
 ![image](https://github.com/MartiVilas/JavaScript-Personalization/assets/150129703/722a628e-62fb-46f3-92fb-395c77d151b0)

---

## Current Snippets 

```json
{

    "DOM": {
        "prefix": "DOM",
        "body": [
            "function añadirAlDom(id, resultado) {",
            "\tconst container = document.getElementById(id);",
            "\tlet p = document.createElement('p');",
            "\tcontainer.appendChild(p);",
            "\tp.textContent = resultado;",
            "\tp.setAttribute('class', 'result');",
            "}"
        ],
        "description": "Add an element to the DOM"
    },

    "MapArray": {
        "prefix": "MapArray",
        "body": [
            "array.map(elemento => 'añadir lo que se necesite')"
        ],
        "description": "Map over an array"
    },

    "SetArray": {
        "prefix": "SetArray",
        "body": [
            "let gadgets = new Set(['añadir contenido set']);"
        ],
        "description": "Create a new Set"
    },

    "imprimirObjeto": {
        "prefix": "imprimirObjeto",
        "body": [
            "function imprimirClase(id, objeto) {",
            "\tfor (const atributo in objeto) {",
            "\t\tañadirAlDom(id, `atributo: ${atributo}, valor: ${objeto[atributo]}`);",
            "\t}",
            "}"
        ],
        "description": "Print object attributes"
    }
}

	

```



### 📚 HTML Snippets

```
	"HTML": {
		"prefix": "base",
		"body": [
		  "<!DOCTYPE html>",
		  "<html lang=\"es\">",
		  "<head>",
		  "    <meta charset=\"UTF-8\">",
		  "    <meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">",
		  "    <link rel=\"stylesheet\" href=\"./style.css\">",
		  "    <script src=\"./main.js\" defer></script>",
		  "",
		  "    <title>Titulo</title>",
		  "</head>",
		  "",
		  "<body>",
		  "    ",
		  "    <header>",
		  "",
		  "    </header>",
		  "",
		  "    <main>",
		  "",
		  "",
		  "    </main>",
		  "",
		  "    <footer>",
		  "        ",
		  "    </footer>",
		  "</body>",
		  "</html>"
		],
		"description": ""
	  }
```
![image](https://github.com/MartiVilas/JavaScript-Personalization/assets/150129703/2d0f8345-d140-44ae-9ec9-ce88e72d466b)
![image](https://github.com/MartiVilas/JavaScript-Personalization/assets/150129703/ce4f8b3c-977a-4ef0-8867-55e905607d4f)
