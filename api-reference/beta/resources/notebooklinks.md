---
title: Tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: da6896fccbea412fb29d88e02088dd7a52e25173
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956175"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="978ee-103">Tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="978ee-103">notebookLinks resource type</span></span>

> <span data-ttu-id="978ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="978ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="978ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="978ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="978ee-106">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="978ee-106">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="978ee-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="978ee-107">JSON representation</span></span>

<span data-ttu-id="978ee-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="978ee-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="978ee-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="978ee-109">Properties</span></span>
| <span data-ttu-id="978ee-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="978ee-110">Property</span></span>     | <span data-ttu-id="978ee-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="978ee-111">Type</span></span>   |<span data-ttu-id="978ee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="978ee-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="978ee-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="978ee-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="978ee-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="978ee-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="978ee-115">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="978ee-115">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="978ee-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="978ee-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="978ee-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="978ee-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="978ee-118">Abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="978ee-118">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
