---
title: tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: dd6f5405f419561a2ec7587fab8f36245947f257
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534090"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="b73ad-103">tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="b73ad-103">pageLinks resource type</span></span>

<span data-ttu-id="b73ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b73ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b73ad-105">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="b73ad-105">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b73ad-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b73ad-106">JSON representation</span></span>

<span data-ttu-id="b73ad-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b73ad-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="b73ad-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b73ad-108">Properties</span></span>
| <span data-ttu-id="b73ad-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b73ad-109">Property</span></span>     | <span data-ttu-id="b73ad-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b73ad-110">Type</span></span>   |<span data-ttu-id="b73ad-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b73ad-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b73ad-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="b73ad-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="b73ad-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="b73ad-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="b73ad-114">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="b73ad-114">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="b73ad-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="b73ad-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="b73ad-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="b73ad-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="b73ad-117">Abre a página no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="b73ad-117">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
