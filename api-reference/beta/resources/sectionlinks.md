---
title: Tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
ms.openlocfilehash: a5e2f4800472e8cedc495e6de1c17a6586710e87
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519910"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="d87ef-103">Tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="d87ef-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d87ef-104">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="d87ef-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d87ef-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d87ef-105">JSON representation</span></span>

<span data-ttu-id="d87ef-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d87ef-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d87ef-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d87ef-107">Properties</span></span>
| <span data-ttu-id="d87ef-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d87ef-108">Property</span></span>     | <span data-ttu-id="d87ef-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d87ef-109">Type</span></span>   |<span data-ttu-id="d87ef-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d87ef-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d87ef-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="d87ef-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="d87ef-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="d87ef-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="d87ef-113">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="d87ef-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="d87ef-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="d87ef-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="d87ef-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="d87ef-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="d87ef-116">Abre a seção no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="d87ef-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sectionlinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
