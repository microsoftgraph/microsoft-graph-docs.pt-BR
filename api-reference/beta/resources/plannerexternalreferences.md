---
title: tipo de recurso plannerExternalReferences
description: O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa. Este é um tipo aberto. Ele faz parte do objeto de detalhes da tarefa. O valor no par propriedade-valor é o objeto externalReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6684757b9eb8b1d05a738b5aed887a05e8f32cb3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344505"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="c08f8-106">tipo de recurso plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="c08f8-106">plannerExternalReferences resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c08f8-107">O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="c08f8-107">The **plannerExternalReferences** resource represents the collection of references on a task.</span></span> <span data-ttu-id="c08f8-108">Este é um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="c08f8-108">This is an Open Type.</span></span> <span data-ttu-id="c08f8-109">Ele faz parte do objeto de [detalhes da tarefa](plannertaskdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="c08f8-109">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="c08f8-110">O valor no par propriedade-valor é o objeto [externalReference](plannerexternalreference.md) .</span><span class="sxs-lookup"><span data-stu-id="c08f8-110">The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="c08f8-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c08f8-111">Properties</span></span>
<span data-ttu-id="c08f8-112">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c08f8-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="c08f8-113">Nesse caso, o cliente deve fornecer **URLs válidas** com base nos protocolos **http/https** como propriedades e seus valores devem ser os objetos [externalReference](plannerexternalreference.md) .</span><span class="sxs-lookup"><span data-stu-id="c08f8-113">In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects.</span></span> <span data-ttu-id="c08f8-114">Com base em OData, os nomes de propriedade em tipos abertos não podem conter `.`os `:`seguintes `%` caracteres:, e, portanto, precisam ser codificados.</span><span class="sxs-lookup"><span data-stu-id="c08f8-114">Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded.</span></span> <span data-ttu-id="c08f8-115">O exemplo é mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="c08f8-115">Example is shown below.</span></span> <span data-ttu-id="c08f8-116">Para remover uma referência, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="c08f8-116">To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c08f8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c08f8-117">JSON representation</span></span>

<span data-ttu-id="c08f8-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c08f8-118">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="c08f8-119">Como</span><span class="sxs-lookup"><span data-stu-id="c08f8-119">// Example</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
