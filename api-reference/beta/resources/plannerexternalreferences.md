---
title: tipo de recurso plannerExternalReferences
description: O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa. Este é um tipo aberto. Ele faz parte do objeto de detalhes da tarefa. O valor no par propriedade-valor é o objeto externalReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 65eb2deb04f44bd08be14cf1c0c6d61807552efa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966011"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="7e371-106">tipo de recurso plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="7e371-106">plannerExternalReferences resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e371-107">O recurso **plannerExternalReferences** representa a coleção de referências em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="7e371-107">The **plannerExternalReferences** resource represents the collection of references on a task.</span></span> <span data-ttu-id="7e371-108">Este é um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="7e371-108">This is an Open Type.</span></span> <span data-ttu-id="7e371-109">Ele faz parte do objeto de [detalhes da tarefa](plannertaskdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="7e371-109">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="7e371-110">O valor no par propriedade-valor é o objeto [externalReference](plannerexternalreference.md) .</span><span class="sxs-lookup"><span data-stu-id="7e371-110">The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="7e371-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e371-111">Properties</span></span>
<span data-ttu-id="7e371-112">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7e371-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="7e371-113">Nesse caso, o cliente deve fornecer **URLs válidas** com base nos protocolos **http/https** como propriedades e seus valores devem ser os objetos [externalReference](plannerexternalreference.md) .</span><span class="sxs-lookup"><span data-stu-id="7e371-113">In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects.</span></span> <span data-ttu-id="7e371-114">Com base em OData, os nomes de propriedade em tipos abertos não podem conter `.`os `:`seguintes `%` caracteres:, e, portanto, precisam ser codificados.</span><span class="sxs-lookup"><span data-stu-id="7e371-114">Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`  so they need to be encoded.</span></span> <span data-ttu-id="7e371-115">O exemplo é mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="7e371-115">Example is shown below.</span></span> <span data-ttu-id="7e371-116">Para remover uma referência, defina o valor da propriedade como `null`.</span><span class="sxs-lookup"><span data-stu-id="7e371-116">To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e371-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e371-117">JSON representation</span></span>

<span data-ttu-id="7e371-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7e371-118">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="7e371-119">Como</span><span class="sxs-lookup"><span data-stu-id="7e371-119">// Example</span></span>

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
