---
title: tipo de recurso provisioningStep
description: 'Descreve as etapas executadas para executar uma ação. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4275730cfd7c9c9c58496b674062ffedb5d7a6cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521324"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="42046-103">tipo de recurso provisioningStep</span><span class="sxs-lookup"><span data-stu-id="42046-103">provisioningStep resource type</span></span>

<span data-ttu-id="42046-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="42046-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42046-105">Descreve as etapas executadas para executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="42046-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="42046-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42046-106">Properties</span></span>

| <span data-ttu-id="42046-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42046-107">Property</span></span>     | <span data-ttu-id="42046-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="42046-108">Type</span></span>        | <span data-ttu-id="42046-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="42046-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="42046-110">description</span><span class="sxs-lookup"><span data-stu-id="42046-110">description</span></span>|<span data-ttu-id="42046-111">String</span><span class="sxs-lookup"><span data-stu-id="42046-111">String</span></span>|<span data-ttu-id="42046-112">Resumo do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="42046-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="42046-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="42046-113">details</span></span>|[<span data-ttu-id="42046-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="42046-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="42046-115">Detalhes sobre o que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="42046-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="42046-116">nome</span><span class="sxs-lookup"><span data-stu-id="42046-116">name</span></span>|<span data-ttu-id="42046-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="42046-117">String</span></span>|<span data-ttu-id="42046-118">Nome da etapa.</span><span class="sxs-lookup"><span data-stu-id="42046-118">Name of the step.</span></span>|
|<span data-ttu-id="42046-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="42046-119">provisioningStepType</span></span>|<span data-ttu-id="42046-120">String</span><span class="sxs-lookup"><span data-stu-id="42046-120">String</span></span>| <span data-ttu-id="42046-121">Tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="42046-121">Type of step.</span></span> <span data-ttu-id="42046-122">Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="42046-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="42046-123">status</span><span class="sxs-lookup"><span data-stu-id="42046-123">status</span></span>|<span data-ttu-id="42046-124">String</span><span class="sxs-lookup"><span data-stu-id="42046-124">String</span></span>| <span data-ttu-id="42046-125">Status da etapa.</span><span class="sxs-lookup"><span data-stu-id="42046-125">Status of the step.</span></span> <span data-ttu-id="42046-126">Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="42046-126">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42046-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42046-127">JSON representation</span></span>

<span data-ttu-id="42046-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42046-128">The following is a JSON representation of the resource.</span></span>

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
