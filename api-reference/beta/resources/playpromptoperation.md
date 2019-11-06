---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 84b54fbce830f5b505decee7e2d25618700728b3
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006575"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="36d44-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="36d44-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36d44-104">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="36d44-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="36d44-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36d44-105">Properties</span></span>

| <span data-ttu-id="36d44-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36d44-106">Property</span></span>            | <span data-ttu-id="36d44-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="36d44-107">Type</span></span>                        | <span data-ttu-id="36d44-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="36d44-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="36d44-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="36d44-109">clientContext</span></span>       | <span data-ttu-id="36d44-110">String</span><span class="sxs-lookup"><span data-stu-id="36d44-110">String</span></span>                      | <span data-ttu-id="36d44-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="36d44-111">Unique Client Context string.</span></span> <span data-ttu-id="36d44-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="36d44-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="36d44-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="36d44-113">completionReason</span></span>    | <span data-ttu-id="36d44-114">String</span><span class="sxs-lookup"><span data-stu-id="36d44-114">String</span></span>                      | <span data-ttu-id="36d44-115">Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="36d44-115">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="36d44-116">id</span><span class="sxs-lookup"><span data-stu-id="36d44-116">id</span></span>                  | <span data-ttu-id="36d44-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36d44-117">String</span></span>                      | <span data-ttu-id="36d44-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36d44-118">Read-only.</span></span>                                                                         |
| <span data-ttu-id="36d44-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="36d44-119">resultInfo</span></span>          | [<span data-ttu-id="36d44-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="36d44-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="36d44-121">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="36d44-121">The result information.</span></span> <span data-ttu-id="36d44-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="36d44-122">Read-only.</span></span>                                |
| <span data-ttu-id="36d44-123">status</span><span class="sxs-lookup"><span data-stu-id="36d44-123">status</span></span>              | <span data-ttu-id="36d44-124">String</span><span class="sxs-lookup"><span data-stu-id="36d44-124">String</span></span>                      | <span data-ttu-id="36d44-125">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="36d44-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="36d44-126">Relações</span><span class="sxs-lookup"><span data-stu-id="36d44-126">Relationships</span></span>
<span data-ttu-id="36d44-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="36d44-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36d44-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36d44-128">JSON representation</span></span>

<span data-ttu-id="36d44-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36d44-129">The following is a JSON representation of the resource.</span></span>

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
