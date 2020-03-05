---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2d93bba585393b11cdb0adc573a8fed5b895ed6a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499999"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="bb435-105">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="bb435-105">educationTerm resource type</span></span>

<span data-ttu-id="bb435-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bb435-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb435-107">Termo A.</span><span class="sxs-lookup"><span data-stu-id="bb435-107">A term.</span></span> <span data-ttu-id="bb435-108">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="bb435-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="bb435-109">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="bb435-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bb435-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bb435-110">Properties</span></span>
| <span data-ttu-id="bb435-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb435-111">Property</span></span>     | <span data-ttu-id="bb435-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb435-112">Type</span></span>   |<span data-ttu-id="bb435-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb435-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb435-114">displayName</span><span class="sxs-lookup"><span data-stu-id="bb435-114">displayName</span></span>| <span data-ttu-id="bb435-115">String</span><span class="sxs-lookup"><span data-stu-id="bb435-115">String</span></span>| <span data-ttu-id="bb435-116">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="bb435-116">Display name of the term.</span></span>| 
|<span data-ttu-id="bb435-117">externalId</span><span class="sxs-lookup"><span data-stu-id="bb435-117">externalId</span></span>|<span data-ttu-id="bb435-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb435-118">String</span></span>| <span data-ttu-id="bb435-119">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="bb435-119">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="bb435-120">startDate</span><span class="sxs-lookup"><span data-stu-id="bb435-120">startDate</span></span>|<span data-ttu-id="bb435-121">Date</span><span class="sxs-lookup"><span data-stu-id="bb435-121">Date</span></span>|<span data-ttu-id="bb435-122">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="bb435-122">Start of the term.</span></span>|
|<span data-ttu-id="bb435-123">endDate</span><span class="sxs-lookup"><span data-stu-id="bb435-123">endDate</span></span>|<span data-ttu-id="bb435-124">Data</span><span class="sxs-lookup"><span data-stu-id="bb435-124">Date</span></span>|<span data-ttu-id="bb435-125">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="bb435-125">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb435-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bb435-126">JSON representation</span></span>

<span data-ttu-id="bb435-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bb435-127">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
