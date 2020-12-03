---
title: tipo de recurso provisioningStep
description: 'Descreve as etapas executadas para executar uma ação. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 24685d0d2a25d00b19bcb796ae0df304c8224ebd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523536"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="b1767-103">tipo de recurso provisioningStep</span><span class="sxs-lookup"><span data-stu-id="b1767-103">provisioningStep resource type</span></span>

<span data-ttu-id="b1767-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1767-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1767-105">Descreve as etapas executadas para executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="b1767-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="b1767-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1767-106">Properties</span></span>

| <span data-ttu-id="b1767-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1767-107">Property</span></span>     | <span data-ttu-id="b1767-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1767-108">Type</span></span>        | <span data-ttu-id="b1767-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1767-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b1767-110">description</span><span class="sxs-lookup"><span data-stu-id="b1767-110">description</span></span>|<span data-ttu-id="b1767-111">String</span><span class="sxs-lookup"><span data-stu-id="b1767-111">String</span></span>|<span data-ttu-id="b1767-112">Resumo do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="b1767-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="b1767-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="b1767-113">details</span></span>|[<span data-ttu-id="b1767-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="b1767-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="b1767-115">Detalhes sobre o que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="b1767-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="b1767-116">nome</span><span class="sxs-lookup"><span data-stu-id="b1767-116">name</span></span>|<span data-ttu-id="b1767-117">String</span><span class="sxs-lookup"><span data-stu-id="b1767-117">String</span></span>|<span data-ttu-id="b1767-118">Nome da etapa.</span><span class="sxs-lookup"><span data-stu-id="b1767-118">Name of the step.</span></span>|
|<span data-ttu-id="b1767-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="b1767-119">provisioningStepType</span></span>|<span data-ttu-id="b1767-120">String</span><span class="sxs-lookup"><span data-stu-id="b1767-120">String</span></span>| <span data-ttu-id="b1767-121">Tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="b1767-121">Type of step.</span></span> <span data-ttu-id="b1767-122">Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b1767-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b1767-123">status</span><span class="sxs-lookup"><span data-stu-id="b1767-123">status</span></span>|<span data-ttu-id="b1767-124">String</span><span class="sxs-lookup"><span data-stu-id="b1767-124">String</span></span>| <span data-ttu-id="b1767-125">Status da etapa.</span><span class="sxs-lookup"><span data-stu-id="b1767-125">Status of the step.</span></span> <span data-ttu-id="b1767-126">Os valores possíveis são: `success` , `warning` ,  `failure` , `skipped` , `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="b1767-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1767-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1767-127">JSON representation</span></span>

<span data-ttu-id="b1767-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1767-128">The following is a JSON representation of the resource.</span></span>

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


