---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9c26565b552471fe2601d8e3cb629fd933d72937
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947579"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="faec1-105">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="faec1-105">educationTerm resource type</span></span>

<span data-ttu-id="faec1-106">Termo A.</span><span class="sxs-lookup"><span data-stu-id="faec1-106">A term.</span></span> <span data-ttu-id="faec1-107">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="faec1-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="faec1-108">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="faec1-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="faec1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faec1-109">Properties</span></span>
| <span data-ttu-id="faec1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faec1-110">Property</span></span>     | <span data-ttu-id="faec1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="faec1-111">Type</span></span>   |<span data-ttu-id="faec1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="faec1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faec1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="faec1-113">displayName</span></span>| <span data-ttu-id="faec1-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="faec1-114">String</span></span>| <span data-ttu-id="faec1-115">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="faec1-115">Display name of the term.</span></span>| 
|<span data-ttu-id="faec1-116">externalId</span><span class="sxs-lookup"><span data-stu-id="faec1-116">externalId</span></span>|<span data-ttu-id="faec1-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="faec1-117">String</span></span>| <span data-ttu-id="faec1-118">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="faec1-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="faec1-119">startDate</span><span class="sxs-lookup"><span data-stu-id="faec1-119">startDate</span></span>|<span data-ttu-id="faec1-120">Data</span><span class="sxs-lookup"><span data-stu-id="faec1-120">Date</span></span>|<span data-ttu-id="faec1-121">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="faec1-121">Start of the term.</span></span>|
|<span data-ttu-id="faec1-122">endDate</span><span class="sxs-lookup"><span data-stu-id="faec1-122">endDate</span></span>|<span data-ttu-id="faec1-123">Data</span><span class="sxs-lookup"><span data-stu-id="faec1-123">Date</span></span>|<span data-ttu-id="faec1-124">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="faec1-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="faec1-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="faec1-125">JSON representation</span></span>

<span data-ttu-id="faec1-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="faec1-126">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
