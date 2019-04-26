---
title: tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
ms.openlocfilehash: a5e2f4800472e8cedc495e6de1c17a6586710e87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562871"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="67337-103">tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="67337-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67337-104">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="67337-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67337-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67337-105">JSON representation</span></span>

<span data-ttu-id="67337-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67337-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="67337-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67337-107">Properties</span></span>
| <span data-ttu-id="67337-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67337-108">Property</span></span>     | <span data-ttu-id="67337-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="67337-109">Type</span></span>   |<span data-ttu-id="67337-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="67337-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67337-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="67337-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="67337-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="67337-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="67337-113">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="67337-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="67337-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="67337-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="67337-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="67337-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="67337-116">Abre a seção no OneNote online.</span><span class="sxs-lookup"><span data-stu-id="67337-116">Opens the section in OneNote Online.</span></span>|

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
