---
title: tipo de recurso playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a6ecdb06c910923d35f9d36590ad09fd7835fccb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563655"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="ae840-103">tipo de recurso playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="ae840-103">playPromptOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae840-104">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="ae840-104">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="ae840-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae840-105">Properties</span></span>

| <span data-ttu-id="ae840-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae840-106">Property</span></span>            | <span data-ttu-id="ae840-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae840-107">Type</span></span>                        | <span data-ttu-id="ae840-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae840-108">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="ae840-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="ae840-109">clientContext</span></span>       | <span data-ttu-id="ae840-110">String</span><span class="sxs-lookup"><span data-stu-id="ae840-110">String</span></span>                      | <span data-ttu-id="ae840-111">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="ae840-111">The client context.</span></span>                                                                |
| <span data-ttu-id="ae840-112">completionReason</span><span class="sxs-lookup"><span data-stu-id="ae840-112">completionReason</span></span>    | <span data-ttu-id="ae840-113">String</span><span class="sxs-lookup"><span data-stu-id="ae840-113">String</span></span>                      | <span data-ttu-id="ae840-114">Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="ae840-114">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="ae840-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae840-115">createdDateTime</span></span>     | <span data-ttu-id="ae840-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae840-116">DateTimeOffset</span></span>              | <span data-ttu-id="ae840-117">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="ae840-117">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="ae840-118">id</span><span class="sxs-lookup"><span data-stu-id="ae840-118">id</span></span>                  | <span data-ttu-id="ae840-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ae840-119">String</span></span>                      | <span data-ttu-id="ae840-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae840-120">Read-only.</span></span>                                                                         |
| <span data-ttu-id="ae840-121">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="ae840-121">lastActionDateTime</span></span>  | <span data-ttu-id="ae840-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae840-122">DateTimeOffset</span></span>              | <span data-ttu-id="ae840-123">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="ae840-123">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="ae840-124">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ae840-124">resultInfo</span></span>          | [<span data-ttu-id="ae840-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="ae840-125">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="ae840-126">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="ae840-126">The result information.</span></span> <span data-ttu-id="ae840-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae840-127">Read-only.</span></span> <span data-ttu-id="ae840-128">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="ae840-128">Server generated.</span></span>                               |
| <span data-ttu-id="ae840-129">status</span><span class="sxs-lookup"><span data-stu-id="ae840-129">status</span></span>              | <span data-ttu-id="ae840-130">String</span><span class="sxs-lookup"><span data-stu-id="ae840-130">String</span></span>                      | <span data-ttu-id="ae840-131">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ae840-131">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="ae840-132">Relações</span><span class="sxs-lookup"><span data-stu-id="ae840-132">Relationships</span></span>
<span data-ttu-id="ae840-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae840-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae840-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae840-134">JSON representation</span></span>

<span data-ttu-id="ae840-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae840-135">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
