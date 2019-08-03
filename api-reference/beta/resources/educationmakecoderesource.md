---
title: tipo de recurso educationMakeCodeResource
description: Um recurso MakeCode
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e983f217af71b6e27f750599ee2f8db295da5fec
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173367"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="51f5f-103">tipo de recurso educationMakeCodeResource</span><span class="sxs-lookup"><span data-stu-id="51f5f-103">educationMakeCodeResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51f5f-104">Um recurso representando um projeto [MakeCode](https://www.microsoft.com/en-us/makecode) .</span><span class="sxs-lookup"><span data-stu-id="51f5f-104">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="51f5f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51f5f-105">Properties</span></span>

| <span data-ttu-id="51f5f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51f5f-106">Property</span></span>     | <span data-ttu-id="51f5f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="51f5f-107">Type</span></span>        | <span data-ttu-id="51f5f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="51f5f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51f5f-109">mkcd</span><span class="sxs-lookup"><span data-stu-id="51f5f-109">mkcd</span></span>|<span data-ttu-id="51f5f-110">String</span><span class="sxs-lookup"><span data-stu-id="51f5f-110">String</span></span>|<span data-ttu-id="51f5f-111">ID do projeto MakeCode</span><span class="sxs-lookup"><span data-stu-id="51f5f-111">ID of the MakeCode project</span></span>|
|<span data-ttu-id="51f5f-112">url</span><span class="sxs-lookup"><span data-stu-id="51f5f-112">url</span></span>|<span data-ttu-id="51f5f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51f5f-113">String</span></span>|<span data-ttu-id="51f5f-114">Host para o tipo de recurso MakeCode (por exemplo,, MICROBIT)</span><span class="sxs-lookup"><span data-stu-id="51f5f-114">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51f5f-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51f5f-115">JSON representation</span></span>

<span data-ttu-id="51f5f-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51f5f-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "mkcd": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->