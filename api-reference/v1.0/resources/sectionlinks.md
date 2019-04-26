---
title: tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
ms.openlocfilehash: afc740aebc494aa6f204febbce1be4433005a4b1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549668"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="d7e5d-103">tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="d7e5d-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7e5d-104">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="d7e5d-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7e5d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7e5d-105">JSON representation</span></span>

<span data-ttu-id="d7e5d-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7e5d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="d7e5d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7e5d-107">Properties</span></span>
| <span data-ttu-id="d7e5d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7e5d-108">Property</span></span>     | <span data-ttu-id="d7e5d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7e5d-109">Type</span></span>   |<span data-ttu-id="d7e5d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7e5d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7e5d-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="d7e5d-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="d7e5d-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="d7e5d-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="d7e5d-113">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="d7e5d-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="d7e5d-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="d7e5d-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="d7e5d-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="d7e5d-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="d7e5d-116">Abre a seção no OneNote online.</span><span class="sxs-lookup"><span data-stu-id="d7e5d-116">Opens the section in OneNote Online.</span></span>|

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
