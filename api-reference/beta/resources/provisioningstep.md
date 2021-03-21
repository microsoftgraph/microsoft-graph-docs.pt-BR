---
title: Tipo de recurso provisioningStep
description: 'Descreve as etapas tomadas para executar uma ação. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6baf1656cb470cfc8dc01908f5a398ac5d421eb1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960338"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="fb4a3-103">Tipo de recurso provisioningStep</span><span class="sxs-lookup"><span data-stu-id="fb4a3-103">provisioningStep resource type</span></span>

<span data-ttu-id="fb4a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb4a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb4a3-105">Descreve as etapas tomadas para executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="fb4a3-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="fb4a3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb4a3-106">Properties</span></span>

| <span data-ttu-id="fb4a3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb4a3-107">Property</span></span>     | <span data-ttu-id="fb4a3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb4a3-108">Type</span></span>        | <span data-ttu-id="fb4a3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb4a3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb4a3-110">description</span><span class="sxs-lookup"><span data-stu-id="fb4a3-110">description</span></span>|<span data-ttu-id="fb4a3-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4a3-111">String</span></span>|<span data-ttu-id="fb4a3-112">Resumo do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="fb4a3-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="fb4a3-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="fb4a3-113">details</span></span>|[<span data-ttu-id="fb4a3-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="fb4a3-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="fb4a3-115">Detalhes do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="fb4a3-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="fb4a3-116">nome</span><span class="sxs-lookup"><span data-stu-id="fb4a3-116">name</span></span>|<span data-ttu-id="fb4a3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb4a3-117">String</span></span>|<span data-ttu-id="fb4a3-118">Nome da etapa.</span><span class="sxs-lookup"><span data-stu-id="fb4a3-118">Name of the step.</span></span>|
|<span data-ttu-id="fb4a3-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="fb4a3-119">provisioningStepType</span></span>|<span data-ttu-id="fb4a3-120">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="fb4a3-120">provisioningStepType</span></span>| <span data-ttu-id="fb4a3-121">Tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="fb4a3-121">Type of step.</span></span> <span data-ttu-id="fb4a3-122">Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="fb4a3-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="fb4a3-123">status</span><span class="sxs-lookup"><span data-stu-id="fb4a3-123">status</span></span>|<span data-ttu-id="fb4a3-124">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="fb4a3-124">provisioningResult</span></span>| <span data-ttu-id="fb4a3-125">Status da etapa.</span><span class="sxs-lookup"><span data-stu-id="fb4a3-125">Status of the step.</span></span> <span data-ttu-id="fb4a3-126">Os valores possíveis são: `success` , , , , `warning`  `failure` `skipped` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="fb4a3-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb4a3-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb4a3-127">JSON representation</span></span>

<span data-ttu-id="fb4a3-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb4a3-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


