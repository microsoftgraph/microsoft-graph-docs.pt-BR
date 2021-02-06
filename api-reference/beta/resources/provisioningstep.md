---
title: Tipo de recurso provisioningStep
description: 'Descreve as etapas realizadas para executar uma ação. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: bfc0fef09c1dfa8da4161a75449894e391ca1974
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135342"
---
# <a name="provisioningstep-resource-type"></a><span data-ttu-id="8e113-103">Tipo de recurso provisioningStep</span><span class="sxs-lookup"><span data-stu-id="8e113-103">provisioningStep resource type</span></span>

<span data-ttu-id="8e113-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e113-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e113-105">Descreve as etapas realizadas para executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="8e113-105">Describes the steps taken to perform an action.</span></span>

## <a name="properties"></a><span data-ttu-id="8e113-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e113-106">Properties</span></span>

| <span data-ttu-id="8e113-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e113-107">Property</span></span>     | <span data-ttu-id="8e113-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e113-108">Type</span></span>        | <span data-ttu-id="8e113-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e113-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e113-110">description</span><span class="sxs-lookup"><span data-stu-id="8e113-110">description</span></span>|<span data-ttu-id="8e113-111">String</span><span class="sxs-lookup"><span data-stu-id="8e113-111">String</span></span>|<span data-ttu-id="8e113-112">Resumo do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="8e113-112">Summary of what occurred during the step.</span></span>|
|<span data-ttu-id="8e113-113">detalhes</span><span class="sxs-lookup"><span data-stu-id="8e113-113">details</span></span>|[<span data-ttu-id="8e113-114">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="8e113-114">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="8e113-115">Detalhes do que ocorreu durante a etapa.</span><span class="sxs-lookup"><span data-stu-id="8e113-115">Details of what occurred during the step.</span></span>|
|<span data-ttu-id="8e113-116">nome</span><span class="sxs-lookup"><span data-stu-id="8e113-116">name</span></span>|<span data-ttu-id="8e113-117">String</span><span class="sxs-lookup"><span data-stu-id="8e113-117">String</span></span>|<span data-ttu-id="8e113-118">Nome da etapa.</span><span class="sxs-lookup"><span data-stu-id="8e113-118">Name of the step.</span></span>|
|<span data-ttu-id="8e113-119">provisioningStepType</span><span class="sxs-lookup"><span data-stu-id="8e113-119">provisioningStepType</span></span>|<span data-ttu-id="8e113-120">String</span><span class="sxs-lookup"><span data-stu-id="8e113-120">String</span></span>| <span data-ttu-id="8e113-121">Tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="8e113-121">Type of step.</span></span> <span data-ttu-id="8e113-122">Os valores possíveis são: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8e113-122">Possible values are: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8e113-123">status</span><span class="sxs-lookup"><span data-stu-id="8e113-123">status</span></span>|<span data-ttu-id="8e113-124">String</span><span class="sxs-lookup"><span data-stu-id="8e113-124">String</span></span>| <span data-ttu-id="8e113-125">Status da etapa.</span><span class="sxs-lookup"><span data-stu-id="8e113-125">Status of the step.</span></span> <span data-ttu-id="8e113-126">Os valores possíveis `success` são: `warning` , , ,  `failure` `skipped` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="8e113-126">Possible values are: `success`, `warning`,  `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e113-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e113-127">JSON representation</span></span>

<span data-ttu-id="8e113-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e113-128">The following is a JSON representation of the resource.</span></span>

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


