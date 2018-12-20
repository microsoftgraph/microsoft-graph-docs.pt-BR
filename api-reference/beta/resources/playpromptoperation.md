---
title: tipo de recurso de playPromptOperation
description: A operação playPrompt para obter o resultado da ação playPrompt.
author: VinodRavichandran
ms.openlocfilehash: d63b8f6cfa96706104cd7baaa08475974b12ca13
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380949"
---
# <a name="playpromptoperation-resource-type"></a><span data-ttu-id="a8dc1-103">tipo de recurso de playPromptOperation</span><span class="sxs-lookup"><span data-stu-id="a8dc1-103">playPromptOperation resource type</span></span>

> <span data-ttu-id="a8dc1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8dc1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8dc1-106">A operação playPrompt para obter o resultado da ação playPrompt.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-106">The playPrompt operation to obtain the result of the playPrompt action.</span></span>

## <a name="properties"></a><span data-ttu-id="a8dc1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8dc1-107">Properties</span></span>

| <span data-ttu-id="a8dc1-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="a8dc1-108">Property</span></span>            | <span data-ttu-id="a8dc1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8dc1-109">Type</span></span>                        | <span data-ttu-id="a8dc1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8dc1-110">Description</span></span>|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| <span data-ttu-id="a8dc1-111">clientContext</span><span class="sxs-lookup"><span data-stu-id="a8dc1-111">clientContext</span></span>       | <span data-ttu-id="a8dc1-112">String</span><span class="sxs-lookup"><span data-stu-id="a8dc1-112">String</span></span>                      | <span data-ttu-id="a8dc1-113">O contexto de cliente.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-113">The client context.</span></span>                                                                |
| <span data-ttu-id="a8dc1-114">completionReason</span><span class="sxs-lookup"><span data-stu-id="a8dc1-114">completionReason</span></span>    | <span data-ttu-id="a8dc1-115">String</span><span class="sxs-lookup"><span data-stu-id="a8dc1-115">String</span></span>                      | <span data-ttu-id="a8dc1-116">Os valores possíveis são: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-116">Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`.</span></span> |
| <span data-ttu-id="a8dc1-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8dc1-117">createdDateTime</span></span>     | <span data-ttu-id="a8dc1-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8dc1-118">DateTimeOffset</span></span>              | <span data-ttu-id="a8dc1-119">A hora de início da operação.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-119">The start time of the operation.</span></span>                                                   |
| <span data-ttu-id="a8dc1-120">id</span><span class="sxs-lookup"><span data-stu-id="a8dc1-120">id</span></span>                  | <span data-ttu-id="a8dc1-121">String</span><span class="sxs-lookup"><span data-stu-id="a8dc1-121">String</span></span>                      | <span data-ttu-id="a8dc1-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-122">Read-only.</span></span>                                                                         |
| <span data-ttu-id="a8dc1-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="a8dc1-123">lastActionDateTime</span></span>  | <span data-ttu-id="a8dc1-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8dc1-124">DateTimeOffset</span></span>              | <span data-ttu-id="a8dc1-125">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-125">The time of the last action of the operation.</span></span>                                      |
| <span data-ttu-id="a8dc1-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a8dc1-126">resultInfo</span></span>          | [<span data-ttu-id="a8dc1-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="a8dc1-127">resultInfo</span></span>](resultInfo.md) | <span data-ttu-id="a8dc1-128">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-128">The result information.</span></span> <span data-ttu-id="a8dc1-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-129">Read-only.</span></span> <span data-ttu-id="a8dc1-130">Servidor foi gerado.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-130">Server generated.</span></span>                               |
| <span data-ttu-id="a8dc1-131">status</span><span class="sxs-lookup"><span data-stu-id="a8dc1-131">status</span></span>              | <span data-ttu-id="a8dc1-132">String</span><span class="sxs-lookup"><span data-stu-id="a8dc1-132">String</span></span>                      | <span data-ttu-id="a8dc1-133">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span>               |

## <a name="relationships"></a><span data-ttu-id="a8dc1-134">Relações</span><span class="sxs-lookup"><span data-stu-id="a8dc1-134">Relationships</span></span>
<span data-ttu-id="a8dc1-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8dc1-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8dc1-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8dc1-136">JSON representation</span></span>

<span data-ttu-id="a8dc1-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8dc1-137">The following is a JSON representation of the resource.</span></span>

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
