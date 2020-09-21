---
title: tipo de recurso statusBase
description: Descreve o status do evento de Resumo de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ee205db24cf8591725ca7d9fc3c4a0fe8c72489e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067101"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="0cd1b-103">tipo de recurso statusBase</span><span class="sxs-lookup"><span data-stu-id="0cd1b-103">statusBase resource type</span></span>

<span data-ttu-id="0cd1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cd1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cd1b-105">Descreve o status do evento de Resumo de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="0cd1b-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="0cd1b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cd1b-106">Properties</span></span>

| <span data-ttu-id="0cd1b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cd1b-107">Property</span></span>     | <span data-ttu-id="0cd1b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cd1b-108">Type</span></span>        | <span data-ttu-id="0cd1b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cd1b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0cd1b-110">status</span><span class="sxs-lookup"><span data-stu-id="0cd1b-110">status</span></span>|<span data-ttu-id="0cd1b-111">String</span><span class="sxs-lookup"><span data-stu-id="0cd1b-111">String</span></span>| <span data-ttu-id="0cd1b-112">Os valores possíveis são: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0cd1b-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cd1b-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cd1b-113">JSON representation</span></span>

<span data-ttu-id="0cd1b-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cd1b-114">The following is a JSON representation of the resource.</span></span>

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


