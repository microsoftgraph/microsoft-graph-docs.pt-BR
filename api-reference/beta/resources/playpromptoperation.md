---
title: tipo de recurso de playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515199"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="353e1-103">tipo de recurso de playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="353e1-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="353e1-104">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="353e1-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="353e1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="353e1-105">Properties</span></span>

| <span data-ttu-id="353e1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="353e1-106">Property</span></span>            | <span data-ttu-id="353e1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="353e1-107">Type</span></span>                        | <span data-ttu-id="353e1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="353e1-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="353e1-109">ClientContext</span><span class="sxs-lookup"><span data-stu-id="353e1-109">clientContext</span></span>       | <span data-ttu-id="353e1-110">String</span><span class="sxs-lookup"><span data-stu-id="353e1-110">String</span></span>                      | <span data-ttu-id="353e1-111">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="353e1-111">The client context.</span></span>                                                                |
| <span data-ttu-id="353e1-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="353e1-112">completionReason</span></span>    | <span data-ttu-id="353e1-113">String</span><span class="sxs-lookup"><span data-stu-id="353e1-113">String</span></span>                      | <span data-ttu-id="353e1-114">Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="353e1-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="353e1-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="353e1-115">createdDateTime</span></span>     | <span data-ttu-id="353e1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="353e1-116">DateTimeOffset</span></span>              | <span data-ttu-id="353e1-117">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="353e1-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="353e1-118">id</span><span class="sxs-lookup"><span data-stu-id="353e1-118">id</span></span>                  | <span data-ttu-id="353e1-119">String</span><span class="sxs-lookup"><span data-stu-id="353e1-119">String</span></span>                      | <span data-ttu-id="353e1-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="353e1-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="353e1-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="353e1-121">lastActionDateTime</span></span>  | <span data-ttu-id="353e1-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="353e1-122">DateTimeOffset</span></span>              | <span data-ttu-id="353e1-123">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="353e1-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="353e1-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="353e1-124">resultInfo</span></span>          | [<span data-ttu-id="353e1-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="353e1-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="353e1-126">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="353e1-126">The result information.</span></span> <span data-ttu-id="353e1-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="353e1-127">Read-only.</span></span> <span data-ttu-id="353e1-128">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="353e1-128">Server generated.</span></span>                               |
| <span data-ttu-id="353e1-129">status</span><span class="sxs-lookup"><span data-stu-id="353e1-129">status</span></span>              | <span data-ttu-id="353e1-130">String</span><span class="sxs-lookup"><span data-stu-id="353e1-130">String</span></span>                      | <span data-ttu-id="353e1-131">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="353e1-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="353e1-132">Relações</span><span class="sxs-lookup"><span data-stu-id="353e1-132">Relationships</span></span>
<span data-ttu-id="353e1-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="353e1-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="353e1-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="353e1-134">JSON representation</span></span>

<span data-ttu-id="353e1-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="353e1-135">The following is a JSON representation of the resource.</span></span>

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
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/playpromptoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
