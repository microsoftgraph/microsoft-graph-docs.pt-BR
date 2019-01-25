---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b5cfe363922fe466eef7a7333ce81249311b4063
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527560"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="0b040-105">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="0b040-105">educationTerm resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b040-106">Termo A.</span><span class="sxs-lookup"><span data-stu-id="0b040-106">A term.</span></span> <span data-ttu-id="0b040-107">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="0b040-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="0b040-108">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="0b040-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0b040-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b040-109">Properties</span></span>
| <span data-ttu-id="0b040-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b040-110">Property</span></span>     | <span data-ttu-id="0b040-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b040-111">Type</span></span>   |<span data-ttu-id="0b040-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b040-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b040-113">displayName</span><span class="sxs-lookup"><span data-stu-id="0b040-113">displayName</span></span>| <span data-ttu-id="0b040-114">String</span><span class="sxs-lookup"><span data-stu-id="0b040-114">String</span></span>| <span data-ttu-id="0b040-115">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="0b040-115">Display name of the term.</span></span>| 
|<span data-ttu-id="0b040-116">externalId</span><span class="sxs-lookup"><span data-stu-id="0b040-116">externalId</span></span>|<span data-ttu-id="0b040-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b040-117">String</span></span>| <span data-ttu-id="0b040-118">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="0b040-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="0b040-119">startDate</span><span class="sxs-lookup"><span data-stu-id="0b040-119">startDate</span></span>|<span data-ttu-id="0b040-120">Data</span><span class="sxs-lookup"><span data-stu-id="0b040-120">Date</span></span>|<span data-ttu-id="0b040-121">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="0b040-121">Start of the term.</span></span>|
|<span data-ttu-id="0b040-122">endDate</span><span class="sxs-lookup"><span data-stu-id="0b040-122">endDate</span></span>|<span data-ttu-id="0b040-123">Data</span><span class="sxs-lookup"><span data-stu-id="0b040-123">Date</span></span>|<span data-ttu-id="0b040-124">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="0b040-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b040-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b040-125">JSON representation</span></span>

<span data-ttu-id="0b040-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b040-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationterm.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
