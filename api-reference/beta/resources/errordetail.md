---
title: tipo de recurso errorDetail
description: Descreve um erro para uma solicitação com falha para criar um esquema de conexão de pesquisa da Microsoft de forma assíncrona.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d52d2953a9ec282b55b021f653854b6c3b6054eb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938987"
---
# <a name="errordetail-resource-type"></a><span data-ttu-id="a838f-103">tipo de recurso errorDetail</span><span class="sxs-lookup"><span data-stu-id="a838f-103">errorDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a838f-104">Descreve um erro para uma solicitação com falha para criar um [esquema](schema.md) de conexão de pesquisa da Microsoft de forma assíncrona.</span><span class="sxs-lookup"><span data-stu-id="a838f-104">Describes an error for a failed request to create a Microsoft Search connection [schema](schema.md) asynchronously.</span></span>

## <a name="properties"></a><span data-ttu-id="a838f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a838f-105">Properties</span></span>

| <span data-ttu-id="a838f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a838f-106">Property</span></span>  | <span data-ttu-id="a838f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a838f-107">Type</span></span>                                               | <span data-ttu-id="a838f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a838f-108">Description</span></span> |
|:----------|:---------------------------------------------------|:------------|
| <span data-ttu-id="a838f-109">detalhes</span><span class="sxs-lookup"><span data-stu-id="a838f-109">details</span></span>   | <span data-ttu-id="a838f-110">coleção [innerErrorDetail](innererrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="a838f-110">[innerErrorDetail](innererrordetail.md) collection</span></span> | <span data-ttu-id="a838f-111">Uma coleção de erros internos, se houver.</span><span class="sxs-lookup"><span data-stu-id="a838f-111">A collection of inner errors, if any.</span></span> <span data-ttu-id="a838f-112">Somente leitura, anulável.</span><span class="sxs-lookup"><span data-stu-id="a838f-112">Read-only, nullable.</span></span> |
| <span data-ttu-id="a838f-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="a838f-113">errorCode</span></span> | <span data-ttu-id="a838f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a838f-114">String</span></span>                                             | <span data-ttu-id="a838f-115">O código de erro associado ao erro, se houver.</span><span class="sxs-lookup"><span data-stu-id="a838f-115">The error code associated with the error, if any.</span></span> <span data-ttu-id="a838f-116">Somente leitura, anulável.</span><span class="sxs-lookup"><span data-stu-id="a838f-116">Read-only, nullable.</span></span> |
| <span data-ttu-id="a838f-117">mensagem</span><span class="sxs-lookup"><span data-stu-id="a838f-117">message</span></span>   | <span data-ttu-id="a838f-118">String</span><span class="sxs-lookup"><span data-stu-id="a838f-118">String</span></span>                                             | <span data-ttu-id="a838f-119">A mensagem de erro legível por pessoas.</span><span class="sxs-lookup"><span data-stu-id="a838f-119">The human-readable error message.</span></span> <span data-ttu-id="a838f-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a838f-120">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a838f-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a838f-121">JSON representation</span></span>

<span data-ttu-id="a838f-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a838f-122">The following is a JSON representation of the resource.</span></span>

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
