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
 ![image](https://github.com/MartiVilas/JavaScript-Personalization/assets/150129703/722a628e-62fb-46f3-92fb-395c77d151b0)

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

![image](https://github.com/MartiVilas/JavaScript-Personalization/assets/150129703/ba0a077c-b331-4a40-9914-d211ea9189ef)
