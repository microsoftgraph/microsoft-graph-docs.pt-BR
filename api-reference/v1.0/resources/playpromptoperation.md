---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5adc385c5764371c1e2cab516bc33fd8504aecf5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447084"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="a00f8-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="a00f8-103">playPromptOperation resource type</span></span>

<span data-ttu-id="a00f8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a00f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a00f8-105">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="a00f8-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="a00f8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a00f8-106">Properties</span></span>

| <span data-ttu-id="a00f8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a00f8-107">Property</span></span>            | <span data-ttu-id="a00f8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a00f8-108">Type</span></span>                        | <span data-ttu-id="a00f8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00f8-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="a00f8-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="a00f8-110">clientContext</span></span>       | <span data-ttu-id="a00f8-111">String</span><span class="sxs-lookup"><span data-stu-id="a00f8-111">String</span></span>                      | <span data-ttu-id="a00f8-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="a00f8-112">Unique Client Context string.</span></span> <span data-ttu-id="a00f8-113">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a00f8-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="a00f8-114">id</span><span class="sxs-lookup"><span data-stu-id="a00f8-114">id</span></span>                  | <span data-ttu-id="a00f8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a00f8-115">String</span></span>                      | <span data-ttu-id="a00f8-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a00f8-116">Read-only.</span></span>                                                                         |
| <span data-ttu-id="a00f8-117">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a00f8-117">resultInfo</span></span>          | [<span data-ttu-id="a00f8-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a00f8-118">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="a00f8-119">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="a00f8-119">The result information.</span></span> <span data-ttu-id="a00f8-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a00f8-120">Read-only.</span></span>                                |
| <span data-ttu-id="a00f8-121">status</span><span class="sxs-lookup"><span data-stu-id="a00f8-121">status</span></span>              | <span data-ttu-id="a00f8-122">String</span><span class="sxs-lookup"><span data-stu-id="a00f8-122">String</span></span>                      | <span data-ttu-id="a00f8-123">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a00f8-123">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="a00f8-124">Relações</span><span class="sxs-lookup"><span data-stu-id="a00f8-124">Relationships</span></span>
<span data-ttu-id="a00f8-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a00f8-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a00f8-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a00f8-126">JSON representation</span></span>

<span data-ttu-id="a00f8-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a00f8-127">The following is a JSON representation of the resource.</span></span>

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
