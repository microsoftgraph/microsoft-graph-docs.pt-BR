---
title: tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
ms.openlocfilehash: 2054e2a7a61d6c715146b51fb97c02516d8b638e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343420"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="13a9f-103">tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="13a9f-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13a9f-104">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="13a9f-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="13a9f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13a9f-105">JSON representation</span></span>

<span data-ttu-id="13a9f-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13a9f-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="13a9f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13a9f-107">Properties</span></span>
| <span data-ttu-id="13a9f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13a9f-108">Property</span></span>     | <span data-ttu-id="13a9f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="13a9f-109">Type</span></span>   |<span data-ttu-id="13a9f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="13a9f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13a9f-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="13a9f-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="13a9f-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="13a9f-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="13a9f-113">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="13a9f-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="13a9f-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="13a9f-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="13a9f-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="13a9f-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="13a9f-116">Abre a seção no OneNote online.</span><span class="sxs-lookup"><span data-stu-id="13a9f-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
