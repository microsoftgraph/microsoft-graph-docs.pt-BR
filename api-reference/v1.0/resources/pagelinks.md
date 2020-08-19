---
title: tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e12dda3b2f2370cf7491809ca0554f341f17fa4d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811872"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="66da9-103">tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="66da9-103">pageLinks resource type</span></span>

<span data-ttu-id="66da9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66da9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66da9-105">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="66da9-105">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66da9-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66da9-106">JSON representation</span></span>

<span data-ttu-id="66da9-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66da9-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="66da9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66da9-108">Properties</span></span>
| <span data-ttu-id="66da9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66da9-109">Property</span></span>     | <span data-ttu-id="66da9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="66da9-110">Type</span></span>   |<span data-ttu-id="66da9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="66da9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66da9-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="66da9-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="66da9-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="66da9-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="66da9-114">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="66da9-114">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="66da9-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="66da9-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="66da9-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="66da9-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="66da9-117">Abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="66da9-117">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
