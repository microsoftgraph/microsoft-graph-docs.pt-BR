---
title: tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
ms.openlocfilehash: 7dab353d4e936559e26a16e64b58bbf3f4c01232
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236549"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="fbdf0-103">tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="fbdf0-103">pageLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbdf0-104">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="fbdf0-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbdf0-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbdf0-105">JSON representation</span></span>

<span data-ttu-id="fbdf0-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbdf0-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="fbdf0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbdf0-107">Properties</span></span>
| <span data-ttu-id="fbdf0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbdf0-108">Property</span></span>     | <span data-ttu-id="fbdf0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbdf0-109">Type</span></span>   |<span data-ttu-id="fbdf0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbdf0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fbdf0-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="fbdf0-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="fbdf0-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="fbdf0-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="fbdf0-113">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="fbdf0-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="fbdf0-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="fbdf0-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="fbdf0-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="fbdf0-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="fbdf0-116">Abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="fbdf0-116">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
