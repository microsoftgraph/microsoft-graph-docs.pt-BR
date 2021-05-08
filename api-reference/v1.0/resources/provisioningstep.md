---
title: Tipo de recurso provisioningStep
description: 'Descreve as etapas tomadas para executar uma ação. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 695f0c30e802dabb03cb30f0615ee6a59e8cc540
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241478"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="89fee-103">Tipo de recurso provisioningStep</span><span class="sxs-lookup"><span data-stu-id="89fee-103">provisioningStep resource type</span></span>

<span data-ttu-id="89fee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89fee-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89fee-105">Descreve as etapas tomadas para executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="89fee-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="89fee-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89fee-106">Properties</span></span>

| <span data-ttu-id="89fee-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89fee-107">Property</span></span>     | <span data-ttu-id="89fee-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="89fee-108">Type</span></span>        | <span data-ttu-id="89fee-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="89fee-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="89fee-110">description</span><span class="sxs-lookup"><span data-stu-id="89fee-110">description</span></span>|<span data-ttu-id="89fee-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89fee-111">String</span></span>|<span data-ttu-id="89fee-112">Resumo do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="89fee-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="89fee-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="89fee-113">details</span></span>|[<span data-ttu-id="89fee-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="89fee-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="89fee-115">Detalhes do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="89fee-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="89fee-116">nome</span><span class="sxs-lookup"><span data-stu-id="89fee-116">name</span></span>|<span data-ttu-id="89fee-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="89fee-117">String</span></span>|<span data-ttu-id="89fee-118">Nome da etapa.</span><span class="sxs-lookup"><span data-stu-id="89fee-118">Name of the step.</span></span>|
|<span data-ttu-id="89fee-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="89fee-119">provisioningStepType</span></span>|<span data-ttu-id="89fee-120">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="89fee-120">provisioningStepType</span></span>| <span data-ttu-id="89fee-121">Tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="89fee-121">Type of step.</span></span> <span data-ttu-id="89fee-122">Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="89fee-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="89fee-123">status</span><span class="sxs-lookup"><span data-stu-id="89fee-123">status</span></span>|<span data-ttu-id="89fee-124">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="89fee-124">provisioningResult</span></span>| <span data-ttu-id="89fee-125">Status da etapa.</span><span class="sxs-lookup"><span data-stu-id="89fee-125">Status of the step.</span></span> <span data-ttu-id="89fee-126">Os valores possíveis são: `success` , , , , `warning`  `failure` `skipped` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="89fee-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89fee-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89fee-127">JSON representation</span></span>

<span data-ttu-id="89fee-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89fee-128">The following is a JSON representation of the resource.</span></span>

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


