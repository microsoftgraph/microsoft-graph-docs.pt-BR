---
title: tipo de recurso innerErrorDetail
description: Um erro interno contido em um objeto errorDetail.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 07220eaead4035dafcb7cd7032916ae4a5db0d75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021900"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="f6fd3-103">tipo de recurso innerErrorDetail</span><span class="sxs-lookup"><span data-stu-id="f6fd3-103">innerErrorDetail resource type</span></span>

<span data-ttu-id="f6fd3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6fd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6fd3-105">Um erro interno contido em um objeto [errorDetail](errordetail.md) .</span><span class="sxs-lookup"><span data-stu-id="f6fd3-105">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="f6fd3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6fd3-106">Properties</span></span>

| <span data-ttu-id="f6fd3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6fd3-107">Property</span></span> | <span data-ttu-id="f6fd3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6fd3-108">Type</span></span>   | <span data-ttu-id="f6fd3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6fd3-109">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="f6fd3-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="f6fd3-110">message</span></span>  | <span data-ttu-id="f6fd3-111">String</span><span class="sxs-lookup"><span data-stu-id="f6fd3-111">String</span></span> | <span data-ttu-id="f6fd3-112">A mensagem de erro legível por pessoas.</span><span class="sxs-lookup"><span data-stu-id="f6fd3-112">The human-readable error message.</span></span> <span data-ttu-id="f6fd3-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6fd3-113">Read-only.</span></span> |
| <span data-ttu-id="f6fd3-114">source</span><span class="sxs-lookup"><span data-stu-id="f6fd3-114">source</span></span>   | <span data-ttu-id="f6fd3-115">String</span><span class="sxs-lookup"><span data-stu-id="f6fd3-115">String</span></span> | <span data-ttu-id="f6fd3-116">A origem do erro.</span><span class="sxs-lookup"><span data-stu-id="f6fd3-116">The source of the error.</span></span> <span data-ttu-id="f6fd3-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6fd3-117">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="f6fd3-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6fd3-118">JSON representation</span></span>

<span data-ttu-id="f6fd3-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6fd3-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.innerErrorDetail",
  "baseType": null
}-->

```json
{
  "message": "String",
  "source": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "innerErrorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


