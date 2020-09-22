---
title: tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33f5aa2c5953bc9e143d08d91047919cf73599b6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094208"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="34193-103">tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="34193-103">pageLinks resource type</span></span>

<span data-ttu-id="34193-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34193-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34193-105">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="34193-105">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34193-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34193-106">JSON representation</span></span>

<span data-ttu-id="34193-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34193-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="34193-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34193-108">Properties</span></span>
| <span data-ttu-id="34193-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34193-109">Property</span></span>     | <span data-ttu-id="34193-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="34193-110">Type</span></span>   |<span data-ttu-id="34193-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="34193-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34193-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="34193-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="34193-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="34193-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="34193-114">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="34193-114">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="34193-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="34193-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="34193-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="34193-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="34193-117">Abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="34193-117">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

