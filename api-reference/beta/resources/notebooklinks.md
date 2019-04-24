---
title: tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: f6995c112410d22cfe5849f54d0077bf8b79f6b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463277"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="e918e-103">tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="e918e-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e918e-104">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e918e-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e918e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e918e-105">JSON representation</span></span>

<span data-ttu-id="e918e-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e918e-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="e918e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e918e-107">Properties</span></span>
| <span data-ttu-id="e918e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e918e-108">Property</span></span>     | <span data-ttu-id="e918e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e918e-109">Type</span></span>   |<span data-ttu-id="e918e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e918e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e918e-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="e918e-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="e918e-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="e918e-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="e918e-113">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="e918e-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="e918e-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="e918e-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="e918e-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="e918e-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="e918e-116">Abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="e918e-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/notebooklinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
