---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3aff109b152be328e6923f6fdb36f116e63a9c16
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913307"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="106a6-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="106a6-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="106a6-104">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="106a6-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="106a6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="106a6-105">Properties</span></span>

| <span data-ttu-id="106a6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="106a6-106">Property</span></span>            | <span data-ttu-id="106a6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="106a6-107">Type</span></span>                        | <span data-ttu-id="106a6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="106a6-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="106a6-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="106a6-109">clientContext</span></span>       | <span data-ttu-id="106a6-110">String</span><span class="sxs-lookup"><span data-stu-id="106a6-110">String</span></span>                      | <span data-ttu-id="106a6-111">Cadeia de caracteres de contexto de cliente exclusivo.</span><span class="sxs-lookup"><span data-stu-id="106a6-111">Unique Client Context string.</span></span> <span data-ttu-id="106a6-112">O limite máximo é de 256 caracteres.</span><span class="sxs-lookup"><span data-stu-id="106a6-112">Max limit is 256 chars.</span></span>                              |
| <span data-ttu-id="106a6-113">completionReason</span><span class="sxs-lookup"><span data-stu-id="106a6-113">completionReason</span></span>    | <span data-ttu-id="106a6-114">String</span><span class="sxs-lookup"><span data-stu-id="106a6-114">String</span></span>                      | <span data-ttu-id="106a6-115">Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="106a6-115">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="106a6-116">id</span><span class="sxs-lookup"><span data-stu-id="106a6-116">id</span></span>                  | <span data-ttu-id="106a6-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="106a6-117">String</span></span>                      | <span data-ttu-id="106a6-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="106a6-118">Read-only.</span></span>                                                                         |
| <span data-ttu-id="106a6-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="106a6-119">resultInfo</span></span>          | [<span data-ttu-id="106a6-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="106a6-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="106a6-121">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="106a6-121">The result information.</span></span> <span data-ttu-id="106a6-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="106a6-122">Read-only.</span></span>                                |
| <span data-ttu-id="106a6-123">status</span><span class="sxs-lookup"><span data-stu-id="106a6-123">status</span></span>              | <span data-ttu-id="106a6-124">String</span><span class="sxs-lookup"><span data-stu-id="106a6-124">String</span></span>                      | <span data-ttu-id="106a6-125">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="106a6-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="106a6-126">Relações</span><span class="sxs-lookup"><span data-stu-id="106a6-126">Relationships</span></span>
<span data-ttu-id="106a6-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="106a6-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="106a6-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="106a6-128">JSON representation</span></span>

<span data-ttu-id="106a6-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="106a6-129">The following is a JSON representation of the resource.</span></span>

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
