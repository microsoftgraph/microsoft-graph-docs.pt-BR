---
title: tipo de recurso provisioningStep
description: 'Descreve as etapas executadas para executar uma ação. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b0ae3d280d6d9dfc8877739b1003ae0c51f6acd6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446558"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="ffda6-103">tipo de recurso provisioningStep</span><span class="sxs-lookup"><span data-stu-id="ffda6-103">provisioningStep resource type</span></span>

<span data-ttu-id="ffda6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffda6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffda6-105">Descreve as etapas executadas para executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="ffda6-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="ffda6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ffda6-106">Properties</span></span>

| <span data-ttu-id="ffda6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ffda6-107">Property</span></span>     | <span data-ttu-id="ffda6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffda6-108">Type</span></span>        | <span data-ttu-id="ffda6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffda6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ffda6-110">description</span><span class="sxs-lookup"><span data-stu-id="ffda6-110">description</span></span>|<span data-ttu-id="ffda6-111">String</span><span class="sxs-lookup"><span data-stu-id="ffda6-111">String</span></span>|<span data-ttu-id="ffda6-112">Resumo do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="ffda6-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="ffda6-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="ffda6-113">details</span></span>|[<span data-ttu-id="ffda6-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="ffda6-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="ffda6-115">Detalhes sobre o que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="ffda6-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="ffda6-116">nome</span><span class="sxs-lookup"><span data-stu-id="ffda6-116">name</span></span>|<span data-ttu-id="ffda6-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ffda6-117">String</span></span>|<span data-ttu-id="ffda6-118">Nome da etapa.</span><span class="sxs-lookup"><span data-stu-id="ffda6-118">Name of the step.</span></span>|
|<span data-ttu-id="ffda6-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="ffda6-119">provisioningStepType</span></span>|<span data-ttu-id="ffda6-120">String</span><span class="sxs-lookup"><span data-stu-id="ffda6-120">String</span></span>| <span data-ttu-id="ffda6-121">Tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="ffda6-121">Type of step.</span></span> <span data-ttu-id="ffda6-122">Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ffda6-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ffda6-123">status</span><span class="sxs-lookup"><span data-stu-id="ffda6-123">status</span></span>|<span data-ttu-id="ffda6-124">String</span><span class="sxs-lookup"><span data-stu-id="ffda6-124">String</span></span>| <span data-ttu-id="ffda6-125">Status da etapa.</span><span class="sxs-lookup"><span data-stu-id="ffda6-125">Status of the step.</span></span> <span data-ttu-id="ffda6-126">Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ffda6-126">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffda6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ffda6-127">JSON representation</span></span>

<span data-ttu-id="ffda6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ffda6-128">The following is a JSON representation of the resource.</span></span>

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
