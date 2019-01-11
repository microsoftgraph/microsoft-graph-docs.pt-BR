---
title: Tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
ms.openlocfilehash: 190842708979d62430a4716a8785fd40309cb189
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858937"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="3e32f-103">Tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="3e32f-103">sectionLinks resource type</span></span>

> <span data-ttu-id="3e32f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e32f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e32f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e32f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e32f-106">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="3e32f-106">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e32f-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e32f-107">JSON representation</span></span>

<span data-ttu-id="3e32f-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e32f-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="3e32f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e32f-109">Properties</span></span>
| <span data-ttu-id="3e32f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e32f-110">Property</span></span>     | <span data-ttu-id="3e32f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e32f-111">Type</span></span>   |<span data-ttu-id="3e32f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e32f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e32f-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="3e32f-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="3e32f-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="3e32f-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="3e32f-115">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="3e32f-115">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="3e32f-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="3e32f-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="3e32f-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="3e32f-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="3e32f-118">Abre a seção no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="3e32f-118">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
