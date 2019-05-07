---
title: tipo de recurso KeyValue
description: Tipo de recurso de par chave-valor padrão.
localization_priority: Normal
ms.openlocfilehash: aa026f36d69e894e056f21ba19865c730ec5b643
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629268"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="5360e-103">tipo de recurso KeyValue</span><span class="sxs-lookup"><span data-stu-id="5360e-103">keyValue resource type</span></span>

<span data-ttu-id="5360e-104">Representa um par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="5360e-104">Represents a key-value pair.</span></span>

## <a name="properties"></a><span data-ttu-id="5360e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5360e-105">Properties</span></span>

| <span data-ttu-id="5360e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5360e-106">Property</span></span>     | <span data-ttu-id="5360e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5360e-107">Type</span></span>   |<span data-ttu-id="5360e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5360e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5360e-109">key</span><span class="sxs-lookup"><span data-stu-id="5360e-109">key</span></span>|<span data-ttu-id="5360e-110">string</span><span class="sxs-lookup"><span data-stu-id="5360e-110">string</span></span>| <span data-ttu-id="5360e-111">Chave para o par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="5360e-111">Key for the key-value pair.</span></span> |
|<span data-ttu-id="5360e-112">value</span><span class="sxs-lookup"><span data-stu-id="5360e-112">value</span></span>|<span data-ttu-id="5360e-113">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5360e-113">string</span></span>| <span data-ttu-id="5360e-114">Valor para o par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="5360e-114">Value for the key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5360e-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5360e-115">JSON representation</span></span>

<span data-ttu-id="5360e-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5360e-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValue"
}-->

```json
{
  "key": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
