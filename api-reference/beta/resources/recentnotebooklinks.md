---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8435c1c1af8e3c1bc13e4dc07548d303a9ad1a66
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965499"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="81f26-104">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="81f26-104">recentNotebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81f26-105">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="81f26-105">Links to open a OneNote notebook.</span></span> <span data-ttu-id="81f26-106">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="81f26-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="81f26-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81f26-107">Properties</span></span>
| <span data-ttu-id="81f26-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81f26-108">Property</span></span>     | <span data-ttu-id="81f26-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="81f26-109">Type</span></span>   |<span data-ttu-id="81f26-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="81f26-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81f26-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="81f26-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="81f26-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="81f26-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="81f26-113">Abre o bloco de anotações no cliente do OneNote, se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="81f26-113">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="81f26-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="81f26-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="81f26-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="81f26-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="81f26-116">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="81f26-116">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81f26-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81f26-117">JSON representation</span></span>

<span data-ttu-id="81f26-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81f26-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
