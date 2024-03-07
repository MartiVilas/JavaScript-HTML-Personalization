# 📚 JavaScript Personalization

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
---

## Current Snippets 

```json
	"DOM": {
		"prefix": "DOM",
		"body": [
			"function añadirAlDom(id,resultado){",
			"\tconst container = document.getElementById(id)",
			"\tlet p = docuement.createElement('p');",
			"\tcontainer.appendChild(p);",
			"\tp.textContent = resultado;",
			"\tp.setAttribute('class', 'result');",
			"}"
		],
		"description": "Log output to console"
	},


	"MapArray":{
		"prefix": "MapArray",
		"body": [
			"array.map(elemento => 'añadir lo que se necesite')",
		],
		"description": "Log output to console"
	},


	"SetArray":{
		"prefix": "SetArray",
		"body": [
			"let gadgets = new Set(['añadir contenido set']);",
		],
		"description": "Log output to console"
	}

```
