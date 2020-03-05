---
title: tipo de recurso educationOneNoteResource
description: 'Uma subclasse de educationResource. Isso representa o local da página do OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cec9c2f2a092175c7ccecaa09c7b8b510000205c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501546"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="d3497-104">tipo de recurso educationOneNoteResource</span><span class="sxs-lookup"><span data-stu-id="d3497-104">educationOneNoteResource resource type</span></span>

<span data-ttu-id="d3497-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3497-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3497-106">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="d3497-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="d3497-107">Isso representa o local da página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="d3497-107">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="d3497-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3497-108">Properties</span></span>
| <span data-ttu-id="d3497-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3497-109">Property</span></span>     | <span data-ttu-id="d3497-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3497-110">Type</span></span>   |<span data-ttu-id="d3497-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3497-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3497-112">pageUrl</span><span class="sxs-lookup"><span data-stu-id="d3497-112">pageUrl</span></span>|<span data-ttu-id="d3497-113">String</span><span class="sxs-lookup"><span data-stu-id="d3497-113">String</span></span>|<span data-ttu-id="d3497-114">A URL do Microsoft Graph para a página no OneNote.</span><span class="sxs-lookup"><span data-stu-id="d3497-114">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="d3497-115">sectionName</span><span class="sxs-lookup"><span data-stu-id="d3497-115">sectionName</span></span>|<span data-ttu-id="d3497-116">String</span><span class="sxs-lookup"><span data-stu-id="d3497-116">String</span></span>|<span data-ttu-id="d3497-117">Nome da seção para a qual as distribuições devem ser copiadas ou copiadas no.</span><span class="sxs-lookup"><span data-stu-id="d3497-117">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3497-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3497-118">JSON representation</span></span>

<span data-ttu-id="d3497-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3497-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
