---
title: tipo de recurso statusBase
description: Descreve o status do evento de Resumo de provisionamento.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5b63290442f4faddf4bcd9e25c01ab564a7fcc94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520321"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="bfac2-103">tipo de recurso statusBase</span><span class="sxs-lookup"><span data-stu-id="bfac2-103">statusBase resource type</span></span>

<span data-ttu-id="bfac2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bfac2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfac2-105">Descreve o status do evento de Resumo de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="bfac2-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="bfac2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfac2-106">Properties</span></span>

| <span data-ttu-id="bfac2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfac2-107">Property</span></span>     | <span data-ttu-id="bfac2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfac2-108">Type</span></span>        | <span data-ttu-id="bfac2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfac2-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bfac2-110">status</span><span class="sxs-lookup"><span data-stu-id="bfac2-110">status</span></span>|<span data-ttu-id="bfac2-111">String</span><span class="sxs-lookup"><span data-stu-id="bfac2-111">String</span></span>| <span data-ttu-id="bfac2-112">Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bfac2-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfac2-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfac2-113">JSON representation</span></span>

<span data-ttu-id="bfac2-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfac2-114">The following is a JSON representation of the resource.</span></span>

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
