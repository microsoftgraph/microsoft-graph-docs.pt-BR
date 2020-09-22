---
title: tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 4600877834a27c2f70ff0dea616ee53134135f18
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48043833"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="ed30f-103">tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="ed30f-103">notebookLinks resource type</span></span>

<span data-ttu-id="ed30f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed30f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed30f-105">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="ed30f-105">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed30f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed30f-106">JSON representation</span></span>

<span data-ttu-id="ed30f-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed30f-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ed30f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed30f-108">Properties</span></span>
| <span data-ttu-id="ed30f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed30f-109">Property</span></span>     | <span data-ttu-id="ed30f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed30f-110">Type</span></span>   |<span data-ttu-id="ed30f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed30f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed30f-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ed30f-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="ed30f-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="ed30f-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="ed30f-114">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="ed30f-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="ed30f-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ed30f-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="ed30f-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="ed30f-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="ed30f-117">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="ed30f-117">Opens the notebook in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

