<span data-ttu-id="8be1c-p102">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **URLs válidas** baseadas nos protocolos **HTTP/HTTPS** como propriedades e seus valores devem ser os objetos [externalReference](plannerexternalreference.md). Com base no OData, os nomes de propriedade em Tipos Abertos não podem conter os seguintes caracteres: `.`, `:` e `%`, portanto, eles precisam ser codificados. Um exemplo é mostrado abaixo. Para remover uma referência, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="8be1c-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects. Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded. Example is shown below. To remove a reference, set the value of the property to `null`.</span></span>
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **URLs válidas** baseadas nos protocolos **HTTP/HTTPS** como propriedades e seus valores devem ser os objetos [externalReference](plannerexternalreference.md). Com base no OData, os nomes de propriedade em Tipos Abertos não podem conter os seguintes caracteres: `.`, `:` e `%`, portanto, eles precisam ser codificados. Um exemplo é mostrado abaixo. Para remover uma referência, defina o valor da propriedade como `null`.

## <span data-ttu-id="8be1c-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8be1c-112">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="8be1c-113">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8be1c-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReferences"
}-->


```json
{
  "String-value":
  {
    "alias": "String-value",
    "lastModifiedBy": "String-value",
    "lastModifiedDateTime": "String(timestamp)",
    "previewPriority": "String-value",
    "type": "String-value"
  }
}
```

<span data-ttu-id="8be1c-114">// Exemplo</span><span class="sxs-lookup"><span data-stu-id="8be1c-114">// Example</span></span>

```json
{
  "https%3A//contoso%2Esharepoint%2Ecom/teams/agile/documents/AnnualReport%2Epptx":
  {
    "@odata.type": "microsoft.graph.externalReference", // required in PATCH requests to edit the references on a task
    "alias": "Agile Team Annual Report",
    "lastModifiedBy": {
      "user": {
        "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
      }
    },
    "lastModifiedDateTime": "2015-09-21T17:45:12.039Z",
    "previewPriority": "0009005756397228702",
    "type": "PowerPoint"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->