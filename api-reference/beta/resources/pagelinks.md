---
title: tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 27f4c45a9ea2747d5ca5748184b84e4fabb54f55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522050"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="f5f89-103">tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="f5f89-103">pageLinks resource type</span></span>

<span data-ttu-id="f5f89-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f5f89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5f89-105">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f5f89-105">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5f89-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5f89-106">JSON representation</span></span>

<span data-ttu-id="f5f89-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5f89-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f5f89-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5f89-108">Properties</span></span>
| <span data-ttu-id="f5f89-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5f89-109">Property</span></span>     | <span data-ttu-id="f5f89-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5f89-110">Type</span></span>   |<span data-ttu-id="f5f89-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5f89-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5f89-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="f5f89-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="f5f89-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="f5f89-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="f5f89-114">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="f5f89-114">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="f5f89-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="f5f89-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="f5f89-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="f5f89-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="f5f89-117">Abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="f5f89-117">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
