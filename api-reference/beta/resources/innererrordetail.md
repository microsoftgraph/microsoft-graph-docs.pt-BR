---
title: tipo de recurso innerErrorDetail
description: Um erro interno contido em um objeto errorDetail.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6b3dfb2ec4caf8ae2b8ec9a279a6d001ad3aaae7
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703774"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="5a90e-103">tipo de recurso innerErrorDetail</span><span class="sxs-lookup"><span data-stu-id="5a90e-103">innerErrorDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a90e-104">Um erro interno contido em um objeto [errorDetail](errordetail.md) .</span><span class="sxs-lookup"><span data-stu-id="5a90e-104">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="5a90e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a90e-105">Properties</span></span>

| <span data-ttu-id="5a90e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a90e-106">Property</span></span> | <span data-ttu-id="5a90e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a90e-107">Type</span></span>   | <span data-ttu-id="5a90e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a90e-108">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="5a90e-109">mensagem</span><span class="sxs-lookup"><span data-stu-id="5a90e-109">message</span></span>  | <span data-ttu-id="5a90e-110">String</span><span class="sxs-lookup"><span data-stu-id="5a90e-110">String</span></span> | <span data-ttu-id="5a90e-111">A mensagem de erro legível por pessoas.</span><span class="sxs-lookup"><span data-stu-id="5a90e-111">The human-readable error message.</span></span> <span data-ttu-id="5a90e-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a90e-112">Read-only.</span></span> |
| <span data-ttu-id="5a90e-113">source</span><span class="sxs-lookup"><span data-stu-id="5a90e-113">source</span></span>   | <span data-ttu-id="5a90e-114">String</span><span class="sxs-lookup"><span data-stu-id="5a90e-114">String</span></span> | <span data-ttu-id="5a90e-115">A origem do erro.</span><span class="sxs-lookup"><span data-stu-id="5a90e-115">The source of the error.</span></span> <span data-ttu-id="5a90e-116">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a90e-116">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="5a90e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a90e-117">JSON representation</span></span>

<span data-ttu-id="5a90e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a90e-118">The following is a JSON representation of the resource.</span></span>

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
