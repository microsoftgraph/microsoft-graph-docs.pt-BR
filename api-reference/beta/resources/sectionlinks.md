---
title: tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0e84f6d071423159918479bdb1836855fed113a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520868"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="bcf15-103">tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="bcf15-103">sectionLinks resource type</span></span>

<span data-ttu-id="bcf15-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bcf15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcf15-105">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="bcf15-105">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bcf15-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bcf15-106">JSON representation</span></span>

<span data-ttu-id="bcf15-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bcf15-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="bcf15-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bcf15-108">Properties</span></span>
| <span data-ttu-id="bcf15-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcf15-109">Property</span></span>     | <span data-ttu-id="bcf15-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcf15-110">Type</span></span>   |<span data-ttu-id="bcf15-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcf15-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcf15-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="bcf15-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="bcf15-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="bcf15-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="bcf15-114">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="bcf15-114">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="bcf15-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="bcf15-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="bcf15-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="bcf15-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="bcf15-117">Abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="bcf15-117">Opens the section in OneNote on the web.</span></span>|

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
