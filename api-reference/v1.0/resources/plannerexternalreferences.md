---
title: tipo de recurso plannerExternalReferences
description: O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa. Este é um tipo aberto. Ele faz parte do objeto de detalhes da tarefa. O valor no par propriedade-valor é o objeto externalReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 37511817d32d1979cf30fc12eb7a1560b1870c27
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447119"
---
# <a name="plannerexternalreferences-resource-type"></a>tipo de recurso plannerExternalReferences

Namespace: Microsoft. Graph

O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa. Este é um tipo aberto. Ele faz parte do objeto de [detalhes da tarefa](plannertaskdetails.md) . O valor no par propriedade-valor é o objeto [externalReference](plannerexternalreference.md) .


## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **URLs válidas** com base nos protocolos **http/https** como propriedades e seus valores devem ser os objetos [externalReference](plannerexternalreference.md) . Com base em OData, os nomes de propriedade em tipos abertos não podem conter `.`os `:`seguintes `%` caracteres:, e, portanto, precisam ser codificados. O exemplo é mostrado abaixo. Para remover uma referência, defina o valor da propriedade como `null`.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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

Como

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
