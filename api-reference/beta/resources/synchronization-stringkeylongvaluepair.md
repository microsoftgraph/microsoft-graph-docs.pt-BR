---
title: tipo de recurso de stringKeyLongValuePair
description: Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é Int64.
ms.openlocfilehash: 0ceafbc4ab683469e616e068c0abc00804578908
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039752"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="af03e-103">tipo de recurso de stringKeyLongValuePair</span><span class="sxs-lookup"><span data-stu-id="af03e-103">stringKeyLongValuePair resource type</span></span>

> <span data-ttu-id="af03e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="af03e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af03e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af03e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af03e-106">Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é Int64.</span><span class="sxs-lookup"><span data-stu-id="af03e-106">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="af03e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af03e-107">Properties</span></span>
| <span data-ttu-id="af03e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af03e-108">Property</span></span>     | <span data-ttu-id="af03e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="af03e-109">Type</span></span>   |<span data-ttu-id="af03e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="af03e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af03e-111">key</span><span class="sxs-lookup"><span data-stu-id="af03e-111">key</span></span>|<span data-ttu-id="af03e-112">String</span><span class="sxs-lookup"><span data-stu-id="af03e-112">String</span></span>|<span data-ttu-id="af03e-113">Chave.</span><span class="sxs-lookup"><span data-stu-id="af03e-113">Key.</span></span>|
|<span data-ttu-id="af03e-114">valor</span><span class="sxs-lookup"><span data-stu-id="af03e-114">value</span></span>|<span data-ttu-id="af03e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="af03e-115">Int64</span></span>|<span data-ttu-id="af03e-116">Valor.</span><span class="sxs-lookup"><span data-stu-id="af03e-116">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af03e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af03e-117">JSON representation</span></span>

<span data-ttu-id="af03e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af03e-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->