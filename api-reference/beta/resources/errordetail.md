---
title: tipo de recurso errorDetail
description: Descreve um erro para uma solicitação com falha para criar um esquema de conexão de pesquisa da Microsoft de forma assíncrona.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0a2ae4137e619620c6dbab12e86a7ed39d4eef13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499159"
---
# <a name="errordetail-resource-type"></a><span data-ttu-id="962e7-103">tipo de recurso errorDetail</span><span class="sxs-lookup"><span data-stu-id="962e7-103">errorDetail resource type</span></span>

<span data-ttu-id="962e7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="962e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="962e7-105">Descreve um erro para uma solicitação com falha para criar um [esquema](schema.md) de conexão de pesquisa da Microsoft de forma assíncrona.</span><span class="sxs-lookup"><span data-stu-id="962e7-105">Describes an error for a failed request to create a Microsoft Search connection [schema](schema.md) asynchronously.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="962e7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="962e7-106">Properties</span></span>

| <span data-ttu-id="962e7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="962e7-107">Property</span></span>  | <span data-ttu-id="962e7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="962e7-108">Type</span></span>                                               | <span data-ttu-id="962e7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="962e7-109">Description</span></span> |
|:----------|:---------------------------------------------------|:------------|
| <span data-ttu-id="962e7-110">detalhes</span><span class="sxs-lookup"><span data-stu-id="962e7-110">details</span></span>   | <span data-ttu-id="962e7-111">coleção [innerErrorDetail](innererrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="962e7-111">[innerErrorDetail](innererrordetail.md) collection</span></span> | <span data-ttu-id="962e7-112">Uma coleção de erros internos, se houver.</span><span class="sxs-lookup"><span data-stu-id="962e7-112">A collection of inner errors, if any.</span></span> <span data-ttu-id="962e7-113">Somente leitura, anulável.</span><span class="sxs-lookup"><span data-stu-id="962e7-113">Read-only, nullable.</span></span> |
| <span data-ttu-id="962e7-114">errorCode</span><span class="sxs-lookup"><span data-stu-id="962e7-114">errorCode</span></span> | <span data-ttu-id="962e7-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="962e7-115">String</span></span>                                             | <span data-ttu-id="962e7-116">O código de erro associado ao erro, se houver.</span><span class="sxs-lookup"><span data-stu-id="962e7-116">The error code associated with the error, if any.</span></span> <span data-ttu-id="962e7-117">Somente leitura, anulável.</span><span class="sxs-lookup"><span data-stu-id="962e7-117">Read-only, nullable.</span></span> |
| <span data-ttu-id="962e7-118">mensagem</span><span class="sxs-lookup"><span data-stu-id="962e7-118">message</span></span>   | <span data-ttu-id="962e7-119">String</span><span class="sxs-lookup"><span data-stu-id="962e7-119">String</span></span>                                             | <span data-ttu-id="962e7-120">A mensagem de erro legível por pessoas.</span><span class="sxs-lookup"><span data-stu-id="962e7-120">The human-readable error message.</span></span> <span data-ttu-id="962e7-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="962e7-121">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="962e7-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="962e7-122">JSON representation</span></span>

<span data-ttu-id="962e7-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="962e7-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "details",
    "errorCode"
  ],
  "@odata.type": "microsoft.graph.errorDetail",
  "baseType": null
}-->

```json
{
  "details": [{"@odata.type": "microsoft.graph.innerErrorDetail"}],
  "errorCode": "String",
  "message": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "errorDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
