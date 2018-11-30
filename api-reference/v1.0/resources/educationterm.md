---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
ms.openlocfilehash: a74ea283f153a535008003e6875018eb12a35d15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003390"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="7a156-105">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="7a156-105">educationTerm resource type</span></span>

<span data-ttu-id="7a156-106">Termo A.</span><span class="sxs-lookup"><span data-stu-id="7a156-106">A term.</span></span> <span data-ttu-id="7a156-107">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="7a156-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="7a156-108">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="7a156-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7a156-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a156-109">Properties</span></span>
| <span data-ttu-id="7a156-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a156-110">Property</span></span>     | <span data-ttu-id="7a156-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a156-111">Type</span></span>   |<span data-ttu-id="7a156-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a156-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a156-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7a156-113">displayName</span></span>| <span data-ttu-id="7a156-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a156-114">String</span></span>| <span data-ttu-id="7a156-115">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="7a156-115">Display name of the term.</span></span>| 
|<span data-ttu-id="7a156-116">externalId</span><span class="sxs-lookup"><span data-stu-id="7a156-116">externalId</span></span>|<span data-ttu-id="7a156-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a156-117">String</span></span>| <span data-ttu-id="7a156-118">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7a156-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="7a156-119">startDate</span><span class="sxs-lookup"><span data-stu-id="7a156-119">startDate</span></span>|<span data-ttu-id="7a156-120">Data</span><span class="sxs-lookup"><span data-stu-id="7a156-120">Date</span></span>|<span data-ttu-id="7a156-121">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="7a156-121">Start of the term.</span></span>|
|<span data-ttu-id="7a156-122">endDate</span><span class="sxs-lookup"><span data-stu-id="7a156-122">endDate</span></span>|<span data-ttu-id="7a156-123">Data</span><span class="sxs-lookup"><span data-stu-id="7a156-123">Date</span></span>|<span data-ttu-id="7a156-124">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="7a156-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7a156-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a156-125">JSON representation</span></span>

<span data-ttu-id="7a156-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a156-126">The following is a JSON representation of the resource.</span></span>

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