---
title: Tipo de recurso pageLinks
description: Links para abrir uma página do OneNote.
ms.openlocfilehash: 598e39f5cf2b6bbd722b07b72f4fa63ad7fd8302
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039929"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="8ccf5-103">Tipo de recurso pageLinks</span><span class="sxs-lookup"><span data-stu-id="8ccf5-103">pageLinks resource type</span></span>

> <span data-ttu-id="8ccf5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8ccf5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ccf5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8ccf5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ccf5-106">Links para abrir uma página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="8ccf5-106">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ccf5-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ccf5-107">JSON representation</span></span>

<span data-ttu-id="8ccf5-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ccf5-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="8ccf5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ccf5-109">Properties</span></span>
| <span data-ttu-id="8ccf5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ccf5-110">Property</span></span>     | <span data-ttu-id="8ccf5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ccf5-111">Type</span></span>   |<span data-ttu-id="8ccf5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ccf5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ccf5-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="8ccf5-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="8ccf5-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="8ccf5-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="8ccf5-115">Abre a página no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="8ccf5-115">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="8ccf5-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="8ccf5-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="8ccf5-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="8ccf5-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="8ccf5-118">Abre a página no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="8ccf5-118">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->