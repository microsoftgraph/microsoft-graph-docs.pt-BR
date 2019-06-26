---
title: tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
ms.openlocfilehash: 54121a6232ae02d12571f925909be5b92a2bb0cd
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236605"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="f2ca1-103">tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="f2ca1-103">pageLinks resource type</span></span>

<span data-ttu-id="f2ca1-104">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f2ca1-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2ca1-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2ca1-105">JSON representation</span></span>

<span data-ttu-id="f2ca1-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2ca1-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f2ca1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2ca1-107">Properties</span></span>
| <span data-ttu-id="f2ca1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2ca1-108">Property</span></span>     | <span data-ttu-id="f2ca1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2ca1-109">Type</span></span>   |<span data-ttu-id="f2ca1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2ca1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2ca1-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="f2ca1-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="f2ca1-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="f2ca1-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="f2ca1-113">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="f2ca1-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="f2ca1-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="f2ca1-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="f2ca1-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="f2ca1-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="f2ca1-116">Abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="f2ca1-116">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
