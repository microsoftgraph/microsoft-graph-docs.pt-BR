---
title: tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: e33e7d3457a72089e7f01972838fb07d9c9747cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522551"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="36efc-103">tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="36efc-103">notebookLinks resource type</span></span>

<span data-ttu-id="36efc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="36efc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36efc-105">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="36efc-105">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36efc-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36efc-106">JSON representation</span></span>

<span data-ttu-id="36efc-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36efc-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="36efc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36efc-108">Properties</span></span>
| <span data-ttu-id="36efc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36efc-109">Property</span></span>     | <span data-ttu-id="36efc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="36efc-110">Type</span></span>   |<span data-ttu-id="36efc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="36efc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36efc-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="36efc-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="36efc-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="36efc-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="36efc-114">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="36efc-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="36efc-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="36efc-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="36efc-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="36efc-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="36efc-117">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="36efc-117">Opens the notebook in OneNote on the web.</span></span>|

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
