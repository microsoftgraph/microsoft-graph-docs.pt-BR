---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1bc49a3fbf494e378ec695af1f53c0ca4ea313ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521618"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="e6c3a-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="e6c3a-103">playPromptOperation resource type</span></span>

<span data-ttu-id="e6c3a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e6c3a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6c3a-105">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-105">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="e6c3a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6c3a-106">Properties</span></span>

| <span data-ttu-id="e6c3a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6c3a-107">Property</span></span>            | <span data-ttu-id="e6c3a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6c3a-108">Type</span></span>                        | <span data-ttu-id="e6c3a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6c3a-109">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="e6c3a-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="e6c3a-110">clientContext</span></span>       | <span data-ttu-id="e6c3a-111">String</span><span class="sxs-lookup"><span data-stu-id="e6c3a-111">String</span></span>                      | <span data-ttu-id="e6c3a-112">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-112">Unique Client Context string.</span></span> <span data-ttu-id="e6c3a-113">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-113">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="e6c3a-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="e6c3a-114">completionReason</span></span>    | <span data-ttu-id="e6c3a-115">String</span><span class="sxs-lookup"><span data-stu-id="e6c3a-115">String</span></span>                      | <span data-ttu-id="e6c3a-116">Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="e6c3a-117">id</span><span class="sxs-lookup"><span data-stu-id="e6c3a-117">id</span></span>                  | <span data-ttu-id="e6c3a-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6c3a-118">String</span></span>                      | <span data-ttu-id="e6c3a-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-119">Read-only.</span></span>                                                                         |
| <span data-ttu-id="e6c3a-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e6c3a-120">resultInfo</span></span>          | [<span data-ttu-id="e6c3a-121">resultInfo</span><span class="sxs-lookup"><span data-stu-id="e6c3a-121">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="e6c3a-122">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-122">The result information.</span></span> <span data-ttu-id="e6c3a-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-123">Read-only.</span></span>                                |
| <span data-ttu-id="e6c3a-124">status</span><span class="sxs-lookup"><span data-stu-id="e6c3a-124">status</span></span>              | <span data-ttu-id="e6c3a-125">String</span><span class="sxs-lookup"><span data-stu-id="e6c3a-125">String</span></span>                      | <span data-ttu-id="e6c3a-126">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-126">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="e6c3a-127">Relações</span><span class="sxs-lookup"><span data-stu-id="e6c3a-127">Relationships</span></span>
<span data-ttu-id="e6c3a-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6c3a-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6c3a-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6c3a-129">JSON representation</span></span>

<span data-ttu-id="e6c3a-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6c3a-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.playPromptOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "unknown | completedSuccessfully | mediaOperationCanceled",
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
