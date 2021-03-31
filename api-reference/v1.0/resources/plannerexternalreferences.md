---
title: Tipo de recurso plannerExternalReferences
description: O **recurso plannerExternalReferences** representa a coleção de referências em uma tarefa. Este é um Tipo Aberto. Ele faz parte do objeto de detalhes da tarefa. O valor no par de valores de propriedade é o objeto externalReference.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d4580d2e54b1f9b913b7dab5c283e9af7391b964
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473392"
---
# <a name="plannerexternalreferences-resource-type"></a><span data-ttu-id="1f4b6-106">Tipo de recurso plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="1f4b6-106">plannerExternalReferences resource type</span></span>

<span data-ttu-id="1f4b6-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f4b6-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f4b6-108">O **recurso plannerExternalReferences** representa a coleção de referências em uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="1f4b6-108">The **plannerExternalReferences** resource represents the collection of references on a task.</span></span> <span data-ttu-id="1f4b6-109">Este é um Tipo Aberto.</span><span class="sxs-lookup"><span data-stu-id="1f4b6-109">This is an Open Type.</span></span> <span data-ttu-id="1f4b6-110">Ele faz parte do objeto [de detalhes da](plannertaskdetails.md) tarefa.</span><span class="sxs-lookup"><span data-stu-id="1f4b6-110">It is part of the [task details](plannertaskdetails.md) object.</span></span> <span data-ttu-id="1f4b6-111">O valor no par de valores de propriedade é o [objeto externalReference.](plannerexternalreference.md)</span><span class="sxs-lookup"><span data-stu-id="1f4b6-111">The value in the property-value pair is the [externalReference](plannerexternalreference.md) object.</span></span>


## <a name="properties"></a><span data-ttu-id="1f4b6-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f4b6-112">Properties</span></span>
<span data-ttu-id="1f4b6-113">As propriedades de um Tipo Aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1f4b6-113">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="1f4b6-114">Nesse caso, o cliente deve fornecer **URLs válidas** com base nos protocolos **HTTP/HTTPS** como propriedades e seus valores devem ser [os objetos externalReference.](plannerexternalreference.md)</span><span class="sxs-lookup"><span data-stu-id="1f4b6-114">In this case, the client must provide **valid URLs** based on the **HTTP/HTTPS** protocols as properties and their values must be the [externalReference](plannerexternalreference.md) objects.</span></span> <span data-ttu-id="1f4b6-115">Com base em OData, os nomes de propriedades em Tipos Abertos não podem conter os seguintes caracteres: , , , , portanto, eles precisam `.` `:` ser `%` `@` `#` codificados.</span><span class="sxs-lookup"><span data-stu-id="1f4b6-115">Based on OData, property names in Open Types cannot contain the following characters: `.`, `:`, `%`, `@`, `#` so they need to be encoded.</span></span> <span data-ttu-id="1f4b6-116">Exemplo é mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="1f4b6-116">Example is shown below.</span></span> <span data-ttu-id="1f4b6-117">Para remover uma referência, de definir o valor da propriedade como `null` .</span><span class="sxs-lookup"><span data-stu-id="1f4b6-117">To remove a reference, set the value of the property to `null`.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f4b6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f4b6-118">JSON representation</span></span>

<span data-ttu-id="1f4b6-119">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1f4b6-119">Here is a JSON representation of the resource</span></span>

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

## <a name="example"></a><span data-ttu-id="1f4b6-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f4b6-120">Example</span></span>

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

