---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 43f36c1843a8f9e92081015dd349ee48a1f768ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037343"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="d7f1d-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="d7f1d-103">playPromptOperation resource type</span></span>

<span data-ttu-id="d7f1d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7f1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7f1d-105">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="d7f1d-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="d7f1d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7f1d-106">Properties</span></span>

| <span data-ttu-id="d7f1d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7f1d-107">Property</span></span>            | <span data-ttu-id="d7f1d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7f1d-108">Type</span></span>                        | <span data-ttu-id="d7f1d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7f1d-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="d7f1d-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="d7f1d-110">clientContext</span></span>       | <span data-ttu-id="d7f1d-111">String</span><span class="sxs-lookup"><span data-stu-id="d7f1d-111">String</span></span>                      | <span data-ttu-id="d7f1d-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="d7f1d-112">Unique Client Context string.</span></span> <span data-ttu-id="d7f1d-113">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="d7f1d-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="d7f1d-114">id</span><span class="sxs-lookup"><span data-stu-id="d7f1d-114">id</span></span>                  | <span data-ttu-id="d7f1d-115">String</span><span class="sxs-lookup"><span data-stu-id="d7f1d-115">String</span></span>                      | <span data-ttu-id="d7f1d-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7f1d-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="d7f1d-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d7f1d-117">resultInfo</span></span>          | [<span data-ttu-id="d7f1d-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d7f1d-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d7f1d-119">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="d7f1d-119">The result information.</span></span> <span data-ttu-id="d7f1d-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7f1d-120">Read-only.</span></span>                                |
| <span data-ttu-id="d7f1d-121">status</span><span class="sxs-lookup"><span data-stu-id="d7f1d-121">status</span></span>              | <span data-ttu-id="d7f1d-122">String</span><span class="sxs-lookup"><span data-stu-id="d7f1d-122">String</span></span>                      | <span data-ttu-id="d7f1d-123">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d7f1d-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="d7f1d-124">Relações</span><span class="sxs-lookup"><span data-stu-id="d7f1d-124">Relationships</span></span>
<span data-ttu-id="d7f1d-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7f1d-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7f1d-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7f1d-126">JSON representation</span></span>

<span data-ttu-id="d7f1d-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7f1d-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

