---
title: tipo de recurso provisioningStep
description: 'Descreve as etapas executadas para executar uma ação. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1658114615c4532f0a7f9b9f5ad3c3a25deff81b
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349317"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="568d9-103">tipo de recurso provisioningStep</span><span class="sxs-lookup"><span data-stu-id="568d9-103">provisioningStep resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="568d9-104">Descreve as etapas executadas para executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="568d9-104">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="568d9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="568d9-105">Properties</span></span>

| <span data-ttu-id="568d9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="568d9-106">Property</span></span>     | <span data-ttu-id="568d9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="568d9-107">Type</span></span>        | <span data-ttu-id="568d9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="568d9-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="568d9-109">description</span><span class="sxs-lookup"><span data-stu-id="568d9-109">description</span></span>|<span data-ttu-id="568d9-110">String</span><span class="sxs-lookup"><span data-stu-id="568d9-110">String</span></span>|<span data-ttu-id="568d9-111">Resumo do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="568d9-111">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="568d9-112">detalhes</span><span class="sxs-lookup"><span data-stu-id="568d9-112">details</span></span>|[<span data-ttu-id="568d9-113">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="568d9-113">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="568d9-114">Detalhes sobre o que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="568d9-114">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="568d9-115">name</span><span class="sxs-lookup"><span data-stu-id="568d9-115">name</span></span>|<span data-ttu-id="568d9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="568d9-116">String</span></span>|<span data-ttu-id="568d9-117">Nome da etapa.</span><span class="sxs-lookup"><span data-stu-id="568d9-117">Name of the step.</span></span>|
|<span data-ttu-id="568d9-118">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="568d9-118">provisioningStepType</span></span>|<span data-ttu-id="568d9-119">String</span><span class="sxs-lookup"><span data-stu-id="568d9-119">String</span></span>| <span data-ttu-id="568d9-120">Tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="568d9-120">Type of step.</span></span> <span data-ttu-id="568d9-121">Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="568d9-121">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="568d9-122">status</span><span class="sxs-lookup"><span data-stu-id="568d9-122">status</span></span>|<span data-ttu-id="568d9-123">String</span><span class="sxs-lookup"><span data-stu-id="568d9-123">String</span></span>| <span data-ttu-id="568d9-124">Status da etapa.</span><span class="sxs-lookup"><span data-stu-id="568d9-124">Status of the step.</span></span> <span data-ttu-id="568d9-125">Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="568d9-125">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="568d9-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="568d9-126">JSON representation</span></span>

<span data-ttu-id="568d9-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="568d9-127">The following is a JSON representation of the resource.</span></span>

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
