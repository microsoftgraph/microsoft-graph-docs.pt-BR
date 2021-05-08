---
title: Tipo de recurso statusBase
description: Descreve o status do evento de resumo de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3e100c1b86c8d299a7d74431715a6e9ef1464393
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231973"
---
# <a name="statusbase-resource-type-deprecated"></a><span data-ttu-id="f66a4-103">Tipo de recurso statusBase (preterido)</span><span class="sxs-lookup"><span data-stu-id="f66a4-103">statusBase resource type (deprecated)</span></span>

<span data-ttu-id="f66a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f66a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
>[!CAUTION] 
> <span data-ttu-id="f66a4-105">A API statusBase está preterida e vai parar de retornar dados em 31 de dezembro de 2021.</span><span class="sxs-lookup"><span data-stu-id="f66a4-105">The statusBase API is deprecated and will stop returning data om December 31, 2021.</span></span> <span data-ttu-id="f66a4-106">Use o novo tipo [provisioningStatusInfo.](provisioningstatusinfo.md)</span><span class="sxs-lookup"><span data-stu-id="f66a4-106">Please use the new [provisioningStatusInfo](provisioningstatusinfo.md) type.</span></span>

<span data-ttu-id="f66a4-107">Descreve o status do evento de resumo de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="f66a4-107">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="f66a4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f66a4-108">Properties</span></span>

| <span data-ttu-id="f66a4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f66a4-109">Property</span></span>     | <span data-ttu-id="f66a4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f66a4-110">Type</span></span>        | <span data-ttu-id="f66a4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f66a4-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f66a4-112">status</span><span class="sxs-lookup"><span data-stu-id="f66a4-112">status</span></span>|<span data-ttu-id="f66a4-113">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="f66a4-113">provisioningResult</span></span>| <span data-ttu-id="f66a4-114">Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f66a4-114">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f66a4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f66a4-115">JSON representation</span></span>

<span data-ttu-id="f66a4-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f66a4-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusBase",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


