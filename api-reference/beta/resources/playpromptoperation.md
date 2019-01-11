---
title: tipo de recurso de playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: bc18b8f64dedd3fa4d758778bbee37c6bcfd46c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814375"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="6a842-103">tipo de recurso de playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="6a842-103">playPromptOperation resource type</span></span>

> <span data-ttu-id="6a842-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6a842-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a842-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6a842-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a842-106">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="6a842-106">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="6a842-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a842-107">Properties</span></span>

| <span data-ttu-id="6a842-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a842-108">Property</span></span>            | <span data-ttu-id="6a842-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a842-109">Type</span></span>                        | <span data-ttu-id="6a842-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a842-110">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="6a842-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="6a842-111">clientContext</span></span>       | <span data-ttu-id="6a842-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a842-112">String</span></span>                      | <span data-ttu-id="6a842-113">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="6a842-113">The client context.</span></span>                                                                |
| <span data-ttu-id="6a842-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="6a842-114">completionReason</span></span>    | <span data-ttu-id="6a842-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a842-115">String</span></span>                      | <span data-ttu-id="6a842-116">Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="6a842-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="6a842-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a842-117">createdDateTime</span></span>     | <span data-ttu-id="6a842-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a842-118">DateTimeOffset</span></span>              | <span data-ttu-id="6a842-119">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="6a842-119">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="6a842-120">id</span><span class="sxs-lookup"><span data-stu-id="6a842-120">id</span></span>                  | <span data-ttu-id="6a842-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a842-121">String</span></span>                      | <span data-ttu-id="6a842-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a842-122">Read-only.</span></span>                                                                         |
| <span data-ttu-id="6a842-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="6a842-123">lastActionDateTime</span></span>  | <span data-ttu-id="6a842-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a842-124">DateTimeOffset</span></span>              | <span data-ttu-id="6a842-125">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="6a842-125">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="6a842-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6a842-126">resultInfo</span></span>          | [<span data-ttu-id="6a842-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="6a842-127">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="6a842-128">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="6a842-128">The result information.</span></span> <span data-ttu-id="6a842-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a842-129">Read-only.</span></span> <span data-ttu-id="6a842-130">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="6a842-130">Server generated.</span></span>                               |
| <span data-ttu-id="6a842-131">status</span><span class="sxs-lookup"><span data-stu-id="6a842-131">status</span></span>              | <span data-ttu-id="6a842-132">String</span><span class="sxs-lookup"><span data-stu-id="6a842-132">String</span></span>                      | <span data-ttu-id="6a842-133">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="6a842-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="6a842-134">Relações</span><span class="sxs-lookup"><span data-stu-id="6a842-134">Relationships</span></span>
<span data-ttu-id="6a842-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a842-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a842-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a842-136">JSON representation</span></span>

<span data-ttu-id="6a842-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a842-137">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "playPromptOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
