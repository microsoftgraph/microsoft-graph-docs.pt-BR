---
title: tipo de recurso de educationOneNoteResource
description: 'Uma subclasse de educationResource. Isso representa o local da página do OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 60b0e4647f1a601d3cbe206e264f7d288ee2110c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521415"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="1e9d5-104">tipo de recurso de educationOneNoteResource</span><span class="sxs-lookup"><span data-stu-id="1e9d5-104">educationOneNoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e9d5-105">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="1e9d5-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="1e9d5-106">Isso representa o local da página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="1e9d5-106">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="1e9d5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e9d5-107">Properties</span></span>
| <span data-ttu-id="1e9d5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e9d5-108">Property</span></span>     | <span data-ttu-id="1e9d5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e9d5-109">Type</span></span>   |<span data-ttu-id="1e9d5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e9d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e9d5-111">pageUrl</span><span class="sxs-lookup"><span data-stu-id="1e9d5-111">pageUrl</span></span>|<span data-ttu-id="1e9d5-112">String</span><span class="sxs-lookup"><span data-stu-id="1e9d5-112">String</span></span>|<span data-ttu-id="1e9d5-113">A URL de gráfico da Microsoft a página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="1e9d5-113">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="1e9d5-114">sectionName</span><span class="sxs-lookup"><span data-stu-id="1e9d5-114">sectionName</span></span>|<span data-ttu-id="1e9d5-115">String</span><span class="sxs-lookup"><span data-stu-id="1e9d5-115">String</span></span>|<span data-ttu-id="1e9d5-116">Nome da seção que devem ser copiadas para distribuições ou que foram copiadas para.</span><span class="sxs-lookup"><span data-stu-id="1e9d5-116">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e9d5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e9d5-117">JSON representation</span></span>

<span data-ttu-id="1e9d5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e9d5-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonenoteresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
