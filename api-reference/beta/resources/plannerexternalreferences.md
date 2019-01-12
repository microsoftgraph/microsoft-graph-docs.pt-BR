---
title: Tipo de recurso plannerExternalReferences
description: O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa. Este é um Tipo Aberto. Ele faz parte do objeto task details. O valor no par propriedade-valor é o objeto externalReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ddd3b3d4887aa5794dee26ea8a5aed4a7c2895e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935371"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="a0997-106">Tipo de recurso plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="a0997-106">plannerExternalReferences resource type</span></span>

> <span data-ttu-id="a0997-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0997-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0997-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0997-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0997-p103">O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa. Este é um Tipo Aberto. Ele faz parte do objeto [task details](plannertaskdetails.md). O valor no par propriedade-valor é o objeto [externalReference](plannerexternalreference.md).</span><span class="sxs-lookup"><span data-stu-id="a0997-p103">The **plannerExternalReferences** resource represents the collection of references on a task. This is an Open Type. It is part of the [task details](plannertaskdetails.md) object. The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="a0997-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0997-113">Properties</span></span>
<span data-ttu-id="a0997-p104">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer **URLs válidas** baseadas nos protocolos **HTTP/HTTPS** como propriedades e seus valores devem ser os objetos [externalReference](plannerexternalreference.md). Com base no OData, os nomes de propriedade em Tipos Abertos não podem conter os seguintes caracteres: `.`, `:` e `%`, portanto, eles precisam ser codificados. Um exemplo é mostrado abaixo. Para remover uma referência, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="a0997-p104">Properties of an Open Type can be defined by the client. In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects. Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded. Example is shown below. To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0997-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0997-119">JSON representation</span></span>

<span data-ttu-id="a0997-120">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a0997-120">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="a0997-121">// Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0997-121">// Example</span></span>

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
