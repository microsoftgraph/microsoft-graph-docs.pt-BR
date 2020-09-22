---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 46f68833487f6b542569a1b042daeed836c13053
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055572"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="183d6-105">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="183d6-105">educationTerm resource type</span></span>

<span data-ttu-id="183d6-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="183d6-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="183d6-107">Termo A.</span><span class="sxs-lookup"><span data-stu-id="183d6-107">A term.</span></span> <span data-ttu-id="183d6-108">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="183d6-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="183d6-109">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="183d6-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="183d6-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="183d6-110">Properties</span></span>
| <span data-ttu-id="183d6-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="183d6-111">Property</span></span>     | <span data-ttu-id="183d6-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="183d6-112">Type</span></span>   |<span data-ttu-id="183d6-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="183d6-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="183d6-114">displayName</span><span class="sxs-lookup"><span data-stu-id="183d6-114">displayName</span></span>| <span data-ttu-id="183d6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="183d6-115">String</span></span>| <span data-ttu-id="183d6-116">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="183d6-116">Display name of the term.</span></span>| 
|<span data-ttu-id="183d6-117">externalId</span><span class="sxs-lookup"><span data-stu-id="183d6-117">externalId</span></span>|<span data-ttu-id="183d6-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="183d6-118">String</span></span>| <span data-ttu-id="183d6-119">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="183d6-119">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="183d6-120">startDate</span><span class="sxs-lookup"><span data-stu-id="183d6-120">startDate</span></span>|<span data-ttu-id="183d6-121">Data</span><span class="sxs-lookup"><span data-stu-id="183d6-121">Date</span></span>|<span data-ttu-id="183d6-122">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="183d6-122">Start of the term.</span></span>|
|<span data-ttu-id="183d6-123">endDate</span><span class="sxs-lookup"><span data-stu-id="183d6-123">endDate</span></span>|<span data-ttu-id="183d6-124">Data</span><span class="sxs-lookup"><span data-stu-id="183d6-124">Date</span></span>|<span data-ttu-id="183d6-125">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="183d6-125">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="183d6-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="183d6-126">JSON representation</span></span>

<span data-ttu-id="183d6-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="183d6-127">The following is a JSON representation of the resource.</span></span>

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


