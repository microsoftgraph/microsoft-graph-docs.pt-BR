---
title: tipo de recurso metadataEntry
description: Metadados para o objeto especificado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 49c43e502cfb06832172f46c1e790b2a20eb0f08
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620553"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="cd4b8-103">tipo de recurso metadataEntry</span><span class="sxs-lookup"><span data-stu-id="cd4b8-103">metadataEntry resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd4b8-104">Metadados para o objeto especificado.</span><span class="sxs-lookup"><span data-stu-id="cd4b8-104">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="cd4b8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd4b8-105">Properties</span></span>
| <span data-ttu-id="cd4b8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd4b8-106">Property</span></span>     | <span data-ttu-id="cd4b8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd4b8-107">Type</span></span>   |<span data-ttu-id="cd4b8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd4b8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd4b8-109">key</span><span class="sxs-lookup"><span data-stu-id="cd4b8-109">key</span></span>|<span data-ttu-id="cd4b8-110">String</span><span class="sxs-lookup"><span data-stu-id="cd4b8-110">String</span></span>|<span data-ttu-id="cd4b8-111">Nome da propriedade de metadados.</span><span class="sxs-lookup"><span data-stu-id="cd4b8-111">Name of the metadata property.</span></span>|
|<span data-ttu-id="cd4b8-112">value</span><span class="sxs-lookup"><span data-stu-id="cd4b8-112">value</span></span>|<span data-ttu-id="cd4b8-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd4b8-113">String</span></span>|<span data-ttu-id="cd4b8-114">Valor da propriedade Metadata.</span><span class="sxs-lookup"><span data-stu-id="cd4b8-114">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd4b8-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd4b8-115">JSON representation</span></span>

<span data-ttu-id="cd4b8-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd4b8-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
