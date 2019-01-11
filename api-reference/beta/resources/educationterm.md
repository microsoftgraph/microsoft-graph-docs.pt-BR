---
title: Tipo de recurso educationTerm
description: Termo A. Isso representa uma parte designada do ano acadêmico. É usada dentro de educationClass.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 67e7cd6c9942b61bb6f9ba45f8f25952ae916c5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835144"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="cada6-105">Tipo de recurso educationTerm</span><span class="sxs-lookup"><span data-stu-id="cada6-105">educationTerm resource type</span></span>

> <span data-ttu-id="cada6-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cada6-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cada6-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cada6-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cada6-108">Termo A.</span><span class="sxs-lookup"><span data-stu-id="cada6-108">A term.</span></span> <span data-ttu-id="cada6-109">Isso representa uma parte designada do ano acadêmico.</span><span class="sxs-lookup"><span data-stu-id="cada6-109">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="cada6-110">É usada dentro de [educationClass](educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="cada6-110">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cada6-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cada6-111">Properties</span></span>
| <span data-ttu-id="cada6-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cada6-112">Property</span></span>     | <span data-ttu-id="cada6-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="cada6-113">Type</span></span>   |<span data-ttu-id="cada6-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="cada6-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cada6-115">displayName</span><span class="sxs-lookup"><span data-stu-id="cada6-115">displayName</span></span>| <span data-ttu-id="cada6-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cada6-116">String</span></span>| <span data-ttu-id="cada6-117">Nome de exibição do termo.</span><span class="sxs-lookup"><span data-stu-id="cada6-117">Display name of the term.</span></span>| 
|<span data-ttu-id="cada6-118">externalId</span><span class="sxs-lookup"><span data-stu-id="cada6-118">externalId</span></span>|<span data-ttu-id="cada6-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cada6-119">String</span></span>| <span data-ttu-id="cada6-120">ID do termo no sistema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="cada6-120">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="cada6-121">startDate</span><span class="sxs-lookup"><span data-stu-id="cada6-121">startDate</span></span>|<span data-ttu-id="cada6-122">Data</span><span class="sxs-lookup"><span data-stu-id="cada6-122">Date</span></span>|<span data-ttu-id="cada6-123">Início do termo.</span><span class="sxs-lookup"><span data-stu-id="cada6-123">Start of the term.</span></span>|
|<span data-ttu-id="cada6-124">endDate</span><span class="sxs-lookup"><span data-stu-id="cada6-124">endDate</span></span>|<span data-ttu-id="cada6-125">Data</span><span class="sxs-lookup"><span data-stu-id="cada6-125">Date</span></span>|<span data-ttu-id="cada6-126">Fim do termo.</span><span class="sxs-lookup"><span data-stu-id="cada6-126">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cada6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cada6-127">JSON representation</span></span>

<span data-ttu-id="cada6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cada6-128">The following is a JSON representation of the resource.</span></span>

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
