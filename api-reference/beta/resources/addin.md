---
title: tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 6e76b8f7981be5da9a2ac8437ff21d4a59dbbe73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884207"
---
# <a name="addin-resource-type"></a><span data-ttu-id="e2be2-103">tipo de recurso addIn</span><span class="sxs-lookup"><span data-stu-id="e2be2-103">addIn resource type</span></span>

> <span data-ttu-id="e2be2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e2be2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2be2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e2be2-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2be2-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2be2-106">JSON representation</span></span>

<span data-ttu-id="e2be2-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2be2-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyvalue"}],
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="e2be2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2be2-108">Properties</span></span>
| <span data-ttu-id="e2be2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2be2-109">Property</span></span>     | <span data-ttu-id="e2be2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2be2-110">Type</span></span>   |<span data-ttu-id="e2be2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2be2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2be2-112">id</span><span class="sxs-lookup"><span data-stu-id="e2be2-112">id</span></span>|<span data-ttu-id="e2be2-113">GUID</span><span class="sxs-lookup"><span data-stu-id="e2be2-113">guid</span></span>||
|<span data-ttu-id="e2be2-114">properties</span><span class="sxs-lookup"><span data-stu-id="e2be2-114">properties</span></span>|<span data-ttu-id="e2be2-115">coleção [keyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e2be2-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="e2be2-116">type</span><span class="sxs-lookup"><span data-stu-id="e2be2-116">type</span></span>|<span data-ttu-id="e2be2-117">string</span><span class="sxs-lookup"><span data-stu-id="e2be2-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
