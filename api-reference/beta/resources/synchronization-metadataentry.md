---
title: tipo de recurso de metadataEntry
description: Metadados para o objeto fornecido.
localization_priority: Normal
ms.openlocfilehash: ffdb2dd3b6729320b5991b1158e10d145e339968
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819478"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="5fde1-103">tipo de recurso de metadataEntry</span><span class="sxs-lookup"><span data-stu-id="5fde1-103">metadataEntry resource type</span></span>

> <span data-ttu-id="5fde1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5fde1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5fde1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5fde1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5fde1-106">Metadados para o objeto fornecido.</span><span class="sxs-lookup"><span data-stu-id="5fde1-106">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="5fde1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fde1-107">Properties</span></span>
| <span data-ttu-id="5fde1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fde1-108">Property</span></span>     | <span data-ttu-id="5fde1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fde1-109">Type</span></span>   |<span data-ttu-id="5fde1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fde1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fde1-111">key</span><span class="sxs-lookup"><span data-stu-id="5fde1-111">key</span></span>|<span data-ttu-id="5fde1-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fde1-112">String</span></span>|<span data-ttu-id="5fde1-113">Nome da propriedade metadados.</span><span class="sxs-lookup"><span data-stu-id="5fde1-113">Name of the metadata property.</span></span>|
|<span data-ttu-id="5fde1-114">valor</span><span class="sxs-lookup"><span data-stu-id="5fde1-114">value</span></span>|<span data-ttu-id="5fde1-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fde1-115">String</span></span>|<span data-ttu-id="5fde1-116">Valor da propriedade metadados.</span><span class="sxs-lookup"><span data-stu-id="5fde1-116">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fde1-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fde1-117">JSON representation</span></span>

<span data-ttu-id="5fde1-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5fde1-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
