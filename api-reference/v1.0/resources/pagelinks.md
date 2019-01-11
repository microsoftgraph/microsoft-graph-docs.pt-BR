---
title: Tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
ms.openlocfilehash: a5950366f6c6079443338b68db258c5762c15a7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872944"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="0c40c-103">Tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="0c40c-103">pageLinks resource type</span></span>

<span data-ttu-id="0c40c-104">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="0c40c-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c40c-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c40c-105">JSON representation</span></span>

<span data-ttu-id="0c40c-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c40c-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="0c40c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c40c-107">Properties</span></span>
| <span data-ttu-id="0c40c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c40c-108">Property</span></span>     | <span data-ttu-id="0c40c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c40c-109">Type</span></span>   |<span data-ttu-id="0c40c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c40c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c40c-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="0c40c-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="0c40c-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="0c40c-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="0c40c-113">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="0c40c-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="0c40c-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="0c40c-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="0c40c-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="0c40c-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="0c40c-116">Abre a página no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="0c40c-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
