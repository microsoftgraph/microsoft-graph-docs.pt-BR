---
title: tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 866176f1c831c70b7a057d1a53ad6b5fa7e5cda4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966640"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="95a29-103">tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="95a29-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95a29-104">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="95a29-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95a29-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95a29-105">JSON representation</span></span>

<span data-ttu-id="95a29-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95a29-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="95a29-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95a29-107">Properties</span></span>
| <span data-ttu-id="95a29-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95a29-108">Property</span></span>     | <span data-ttu-id="95a29-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="95a29-109">Type</span></span>   |<span data-ttu-id="95a29-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95a29-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95a29-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="95a29-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="95a29-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="95a29-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="95a29-113">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="95a29-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="95a29-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="95a29-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="95a29-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="95a29-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="95a29-116">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="95a29-116">Opens the notebook in OneNote on the web.</span></span>|

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
