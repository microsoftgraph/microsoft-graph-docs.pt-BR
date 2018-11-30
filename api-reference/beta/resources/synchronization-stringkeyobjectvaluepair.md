---
title: tipo de recurso de stringKeyObjectValuePair
description: Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de open do OData que espera tem uma propriedade denominada `value` ou seja um objeto JSON válido.
ms.openlocfilehash: ae536b2aab87b9920c2afcbe324e30b5f5380dbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036682"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="62e31-104">tipo de recurso de stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="62e31-104">stringKeyObjectValuePair resource type</span></span>

> <span data-ttu-id="62e31-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="62e31-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62e31-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="62e31-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="62e31-107">Representa um par de chave-valor em que a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="62e31-107">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="62e31-108">Este é um tipo de open do OData que espera tem uma propriedade denominada `value` ou seja um objeto JSON válido.</span><span class="sxs-lookup"><span data-stu-id="62e31-108">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="62e31-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62e31-109">Properties</span></span>
| <span data-ttu-id="62e31-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62e31-110">Property</span></span>     | <span data-ttu-id="62e31-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="62e31-111">Type</span></span>   |<span data-ttu-id="62e31-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="62e31-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62e31-113">key</span><span class="sxs-lookup"><span data-stu-id="62e31-113">key</span></span>|<span data-ttu-id="62e31-114">String</span><span class="sxs-lookup"><span data-stu-id="62e31-114">String</span></span>|<span data-ttu-id="62e31-115">Chave.</span><span class="sxs-lookup"><span data-stu-id="62e31-115">Key.</span></span>|
|<span data-ttu-id="62e31-116">valor</span><span class="sxs-lookup"><span data-stu-id="62e31-116">value</span></span>|<span data-ttu-id="62e31-117">Qualquer</span><span class="sxs-lookup"><span data-stu-id="62e31-117">Any</span></span>|<span data-ttu-id="62e31-118">Objeto JSON arbitrário.</span><span class="sxs-lookup"><span data-stu-id="62e31-118">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62e31-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62e31-119">JSON representation</span></span>

<span data-ttu-id="62e31-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62e31-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->