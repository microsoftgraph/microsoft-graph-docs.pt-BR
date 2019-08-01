---
title: tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 8ec315e3dbf5e807408c4de289b2bedf42999159
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035956"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="4e53a-103">tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="4e53a-103">notebookLinks resource type</span></span>

<span data-ttu-id="4e53a-104">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="4e53a-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e53a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e53a-105">JSON representation</span></span>

<span data-ttu-id="4e53a-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e53a-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="4e53a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e53a-107">Properties</span></span>
| <span data-ttu-id="4e53a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e53a-108">Property</span></span>     | <span data-ttu-id="4e53a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e53a-109">Type</span></span>   |<span data-ttu-id="4e53a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e53a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e53a-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="4e53a-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="4e53a-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="4e53a-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="4e53a-113">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="4e53a-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="4e53a-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="4e53a-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="4e53a-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="4e53a-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="4e53a-116">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="4e53a-116">Opens the notebook in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
