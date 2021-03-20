---
title: Tipo de recurso statusBase
description: Descreve o status do evento de resumo de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f486066b150ccd0321f23f47089aab67d87e9f7e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950293"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="8c437-103">Tipo de recurso statusBase</span><span class="sxs-lookup"><span data-stu-id="8c437-103">statusBase resource type</span></span>

<span data-ttu-id="8c437-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c437-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c437-105">Descreve o status do evento de resumo de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="8c437-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="8c437-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c437-106">Properties</span></span>

| <span data-ttu-id="8c437-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c437-107">Property</span></span>     | <span data-ttu-id="8c437-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c437-108">Type</span></span>        | <span data-ttu-id="8c437-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c437-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c437-110">status</span><span class="sxs-lookup"><span data-stu-id="8c437-110">status</span></span>|<span data-ttu-id="8c437-111">provisioningResult</span><span class="sxs-lookup"><span data-stu-id="8c437-111">provisioningResult</span></span>| <span data-ttu-id="8c437-112">Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8c437-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c437-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c437-113">JSON representation</span></span>

<span data-ttu-id="8c437-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c437-114">The following is a JSON representation of the resource.</span></span>

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


