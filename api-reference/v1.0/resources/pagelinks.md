---
title: Tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
ms.openlocfilehash: f1e4fe36d4356986bc88b744a9a62e28b8d368c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003993"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="9fe90-103">Tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="9fe90-103">pageLinks resource type</span></span>

<span data-ttu-id="9fe90-104">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="9fe90-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fe90-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fe90-105">JSON representation</span></span>

<span data-ttu-id="9fe90-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9fe90-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9fe90-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fe90-107">Properties</span></span>
| <span data-ttu-id="9fe90-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fe90-108">Property</span></span>     | <span data-ttu-id="9fe90-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fe90-109">Type</span></span>   |<span data-ttu-id="9fe90-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fe90-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fe90-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="9fe90-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="9fe90-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="9fe90-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="9fe90-113">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="9fe90-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="9fe90-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="9fe90-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="9fe90-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="9fe90-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="9fe90-116">Abre a página no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="9fe90-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->