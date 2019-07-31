---
title: tipo de recurso educationOneNoteResource
description: 'Uma subclasse de educationResource. Isso representa o local da página do OneNote.  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 659ca7f55309499314f94ea62e9433c919856dc6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972646"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="6d29f-104">tipo de recurso educationOneNoteResource</span><span class="sxs-lookup"><span data-stu-id="6d29f-104">educationOneNoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d29f-105">Uma subclasse de [educationResource](educationresource.md).</span><span class="sxs-lookup"><span data-stu-id="6d29f-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="6d29f-106">Isso representa o local da página do OneNote.</span><span class="sxs-lookup"><span data-stu-id="6d29f-106">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="6d29f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d29f-107">Properties</span></span>
| <span data-ttu-id="6d29f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d29f-108">Property</span></span>     | <span data-ttu-id="6d29f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d29f-109">Type</span></span>   |<span data-ttu-id="6d29f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d29f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d29f-111">pageUrl</span><span class="sxs-lookup"><span data-stu-id="6d29f-111">pageUrl</span></span>|<span data-ttu-id="6d29f-112">String</span><span class="sxs-lookup"><span data-stu-id="6d29f-112">String</span></span>|<span data-ttu-id="6d29f-113">A URL do Microsoft Graph para a página no OneNote.</span><span class="sxs-lookup"><span data-stu-id="6d29f-113">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="6d29f-114">sectionName</span><span class="sxs-lookup"><span data-stu-id="6d29f-114">sectionName</span></span>|<span data-ttu-id="6d29f-115">String</span><span class="sxs-lookup"><span data-stu-id="6d29f-115">String</span></span>|<span data-ttu-id="6d29f-116">Nome da seção para a qual as distribuições devem ser copiadas ou copiadas no.</span><span class="sxs-lookup"><span data-stu-id="6d29f-116">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d29f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d29f-117">JSON representation</span></span>

<span data-ttu-id="6d29f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d29f-118">The following is a JSON representation of the resource.</span></span>

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
