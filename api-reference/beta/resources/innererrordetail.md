---
title: tipo de recurso innerErrorDetail
description: Um erro interno contido em um objeto errorDetail.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c1dd87e6af015423441b75ada256456e748e3805
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495925"
---
# <a name="innererrordetail-resource-type"></a><span data-ttu-id="c831f-103">tipo de recurso innerErrorDetail</span><span class="sxs-lookup"><span data-stu-id="c831f-103">innerErrorDetail resource type</span></span>

<span data-ttu-id="c831f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c831f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c831f-105">Um erro interno contido em um objeto [errorDetail](errordetail.md) .</span><span class="sxs-lookup"><span data-stu-id="c831f-105">An inner error contained in an [errorDetail](errordetail.md) object.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="c831f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c831f-106">Properties</span></span>

| <span data-ttu-id="c831f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c831f-107">Property</span></span> | <span data-ttu-id="c831f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c831f-108">Type</span></span>   | <span data-ttu-id="c831f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c831f-109">Description</span></span>                                  |
|:---------|:-------|:---------------------------------------------|
| <span data-ttu-id="c831f-110">mensagem</span><span class="sxs-lookup"><span data-stu-id="c831f-110">message</span></span>  | <span data-ttu-id="c831f-111">String</span><span class="sxs-lookup"><span data-stu-id="c831f-111">String</span></span> | <span data-ttu-id="c831f-112">A mensagem de erro legível por pessoas.</span><span class="sxs-lookup"><span data-stu-id="c831f-112">The human-readable error message.</span></span> <span data-ttu-id="c831f-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c831f-113">Read-only.</span></span> |
| <span data-ttu-id="c831f-114">source</span><span class="sxs-lookup"><span data-stu-id="c831f-114">source</span></span>   | <span data-ttu-id="c831f-115">String</span><span class="sxs-lookup"><span data-stu-id="c831f-115">String</span></span> | <span data-ttu-id="c831f-116">A origem do erro.</span><span class="sxs-lookup"><span data-stu-id="c831f-116">The source of the error.</span></span> <span data-ttu-id="c831f-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c831f-117">Read-only.</span></span>          |

## <a name="json-representation"></a><span data-ttu-id="c831f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c831f-118">JSON representation</span></span>

<span data-ttu-id="c831f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c831f-119">The following is a JSON representation of the resource.</span></span>

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
