---
title: tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: b0050463ec3b88bd32e69efa6cfde5189fdce8d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033668"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="e3823-103">tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="e3823-103">notebookLinks resource type</span></span>

<span data-ttu-id="e3823-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3823-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3823-105">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e3823-105">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3823-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3823-106">JSON representation</span></span>

<span data-ttu-id="e3823-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3823-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e3823-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3823-108">Properties</span></span>
| <span data-ttu-id="e3823-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3823-109">Property</span></span>     | <span data-ttu-id="e3823-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3823-110">Type</span></span>   |<span data-ttu-id="e3823-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3823-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3823-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="e3823-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="e3823-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="e3823-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="e3823-114">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="e3823-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="e3823-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="e3823-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="e3823-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="e3823-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="e3823-117">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="e3823-117">Opens the notebook in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


