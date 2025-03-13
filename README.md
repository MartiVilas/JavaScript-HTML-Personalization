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

  "Generar tabla en el DOM a partir de un objeto": {
          "prefix": "tablaDom",
          "body": [
            "/**",
            " * Genera una tabla HTML en el DOM a partir de un objeto dado.",
            " *",
            " * @param {string} id - ID del contenedor donde se insertará la tabla.",
            " * @param {Object} objeto - Objeto cuyos atributos y valores se mostrarán en la tabla.",
            " * @param {Object} [opciones={}] - Opciones de personalización.",
            " * @param {boolean} [opciones.incluirFunciones=false] - Si es `true`, incluirá métodos del objeto.",
            " * @param {string} [opciones.claseTabla=\"tabla-estilo\"] - Clase CSS para la tabla.",
            " */",
            "function tablaDom(id, objeto, opciones = {}) {",
            "  const contenedor = document.getElementById(id);",
            "  if (!contenedor) {",
            "    console.error(`No se encontró ningún elemento con id \"${id}\"`);",
            "    return;",
            "  }",
            "  const { incluirFunciones = false, claseTabla = \"tabla-estilo\" } = opciones;",
            "  const tabla = document.createElement(\"table\");",
            "  tabla.className = claseTabla;",
            "  tabla.style.borderCollapse = \"collapse\";",
            "  tabla.style.width = \"100%\";",
            "  tabla.style.textAlign = \"left\";",
            "  const filaAtributos = document.createElement(\"tr\");",
            "  const filaValores = document.createElement(\"tr\");",
            "  const claves = Object.keys(objeto).filter(clave => incluirFunciones || typeof objeto[clave] !== \"function\");",
            "  for (const clave of claves) {",
            "    const th = document.createElement(\"th\");",
            "    th.textContent = clave;",
            "    th.style.border = \"1px solid #ccc\";",
            "    th.style.padding = \"8px\";",
            "    filaAtributos.appendChild(th);",
            "    const td = document.createElement(\"td\");",
            "    td.style.border = \"1px solid #ccc\";",
            "    td.style.padding = \"8px\";",
            "    td.appendChild(formatearValor(objeto[clave]));",
            "    filaValores.appendChild(td);",
            "  }",
            "  tabla.appendChild(filaAtributos);",
            "  tabla.appendChild(filaValores);",
            "  contenedor.appendChild(tabla);",
            "}",
            "",
            "/**",
            " * Formatea un valor para ser insertado en la tabla, manejando objetos y arrays.",
            " *",
            " * @param {*} valor - Valor a formatear.",
            " * @returns {HTMLElement} - Elemento HTML con el valor formateado.",
            " */",
            "function formatearValor(valor) {",
            "  if (Array.isArray(valor)) {",
            "    const ul = document.createElement(\"ul\");",
            "    valor.forEach(item => {",
            "      const li = document.createElement(\"li\");",
            "      li.appendChild(formatearValor(item));",
            "      ul.appendChild(li);",
            "    });",
            "    return ul;",
            "  } else if (typeof valor === \"object\" && valor !== null) {",
            "    return document.createTextNode(JSON.stringify(valor, null, 2));",
            "  } else {",
            "    return document.createTextNode(valor);",
            "  }",
            "}"
          ],
          "description": "Genera una tabla HTML en el DOM a partir de un objeto."
        }


```
