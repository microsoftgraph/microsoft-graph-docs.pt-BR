---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 59558512d27bb92c48fb5c0ac2dd0fb52f7c426d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531500"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="45dba-105">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="45dba-105">educationTerm resource type</span></span>

<span data-ttu-id="45dba-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45dba-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45dba-107">Termo A.</span><span class="sxs-lookup"><span data-stu-id="45dba-107">A term.</span></span> <span data-ttu-id="45dba-108">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="45dba-108">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="45dba-109">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="45dba-109">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="45dba-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45dba-110">Properties</span></span>
| <span data-ttu-id="45dba-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45dba-111">Property</span></span>     | <span data-ttu-id="45dba-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="45dba-112">Type</span></span>   |<span data-ttu-id="45dba-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="45dba-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45dba-114">displayName</span><span class="sxs-lookup"><span data-stu-id="45dba-114">displayName</span></span>| <span data-ttu-id="45dba-115">String</span><span class="sxs-lookup"><span data-stu-id="45dba-115">String</span></span>| <span data-ttu-id="45dba-116">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="45dba-116">Display name of the term.</span></span>| 
|<span data-ttu-id="45dba-117">externalId</span><span class="sxs-lookup"><span data-stu-id="45dba-117">externalId</span></span>|<span data-ttu-id="45dba-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45dba-118">String</span></span>| <span data-ttu-id="45dba-119">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="45dba-119">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="45dba-120">startDate</span><span class="sxs-lookup"><span data-stu-id="45dba-120">startDate</span></span>|<span data-ttu-id="45dba-121">Date</span><span class="sxs-lookup"><span data-stu-id="45dba-121">Date</span></span>|<span data-ttu-id="45dba-122">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="45dba-122">Start of the term.</span></span>|
|<span data-ttu-id="45dba-123">endDate</span><span class="sxs-lookup"><span data-stu-id="45dba-123">endDate</span></span>|<span data-ttu-id="45dba-124">Data</span><span class="sxs-lookup"><span data-stu-id="45dba-124">Date</span></span>|<span data-ttu-id="45dba-125">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="45dba-125">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45dba-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45dba-126">JSON representation</span></span>

<span data-ttu-id="45dba-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45dba-127">The following is a JSON representation of the resource.</span></span>

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
