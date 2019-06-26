---
title: tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
ms.openlocfilehash: 1e699ed9739287637da0765f5ec0dbc87d8777fa
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236647"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="12dc5-103">tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="12dc5-103">sectionLinks resource type</span></span>

<span data-ttu-id="12dc5-104">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="12dc5-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12dc5-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12dc5-105">JSON representation</span></span>

<span data-ttu-id="12dc5-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12dc5-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="12dc5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12dc5-107">Properties</span></span>
| <span data-ttu-id="12dc5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12dc5-108">Property</span></span>     | <span data-ttu-id="12dc5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="12dc5-109">Type</span></span>   |<span data-ttu-id="12dc5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="12dc5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12dc5-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="12dc5-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="12dc5-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="12dc5-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="12dc5-113">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="12dc5-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="12dc5-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="12dc5-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="12dc5-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="12dc5-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="12dc5-116">Abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="12dc5-116">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
