# <a name="plannerexternalreferences-resource-type"></a>Tipo de recurso plannerExternalReferences

O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa. Este é um Tipo Aberto. Ele faz parte do objeto [task details](plannertaskdetails.md). O valor no par propriedade-valor é o objeto [externalReference](plannerexternalreference.md).


### <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **URLs válidas** baseadas nos protocolos **HTTP/HTTPS** como propriedades e seus valores devem ser os objetos [externalReference](plannerexternalreference.md). Com base no OData, os nomes de propriedade em Tipos Abertos não podem conter os seguintes caracteres: `.`, `:` e `%`, portanto, eles precisam ser codificados. Um exemplo é mostrado abaixo. Para remover uma referência, defina o valor da propriedade como `null`.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

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

// Exemplo

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