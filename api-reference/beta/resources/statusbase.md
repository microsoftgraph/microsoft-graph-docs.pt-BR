---
title: tipo de recurso statusBase
description: Descreve o status do evento de Resumo de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5d655649f7e1edca4e269576c9bcb6d1f3014e89
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523025"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="195d9-103">tipo de recurso statusBase</span><span class="sxs-lookup"><span data-stu-id="195d9-103">statusBase resource type</span></span>

<span data-ttu-id="195d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="195d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="195d9-105">Descreve o status do evento de Resumo de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="195d9-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="195d9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="195d9-106">Properties</span></span>

| <span data-ttu-id="195d9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="195d9-107">Property</span></span>     | <span data-ttu-id="195d9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="195d9-108">Type</span></span>        | <span data-ttu-id="195d9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="195d9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="195d9-110">status</span><span class="sxs-lookup"><span data-stu-id="195d9-110">status</span></span>|<span data-ttu-id="195d9-111">String</span><span class="sxs-lookup"><span data-stu-id="195d9-111">String</span></span>| <span data-ttu-id="195d9-112">Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="195d9-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="195d9-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="195d9-113">JSON representation</span></span>

<span data-ttu-id="195d9-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="195d9-114">The following is a JSON representation of the resource.</span></span>

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


