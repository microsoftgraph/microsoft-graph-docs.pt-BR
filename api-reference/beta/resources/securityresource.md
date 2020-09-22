---
title: tipo de recurso securityResource
description: Representa os recursos relacionados a um alerta.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 4d27b5815366bdce76e5f99f0410f67684e608ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988818"
---
# <a name="securityresource-resource-type"></a><span data-ttu-id="a23d6-103">tipo de recurso securityResource</span><span class="sxs-lookup"><span data-stu-id="a23d6-103">securityResource resource type</span></span>

<span data-ttu-id="a23d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a23d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a23d6-105">Representa os recursos relacionados a um alerta.</span><span class="sxs-lookup"><span data-stu-id="a23d6-105">Represents the resources related to an alert.</span></span>

## <a name="properties"></a><span data-ttu-id="a23d6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a23d6-106">Properties</span></span>

| <span data-ttu-id="a23d6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a23d6-107">Property</span></span>   | <span data-ttu-id="a23d6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a23d6-108">Type</span></span>|<span data-ttu-id="a23d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a23d6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a23d6-110">recurso</span><span class="sxs-lookup"><span data-stu-id="a23d6-110">resource</span></span>|<span data-ttu-id="a23d6-111">String</span><span class="sxs-lookup"><span data-stu-id="a23d6-111">String</span></span>|<span data-ttu-id="a23d6-112">Nome do recurso relacionado ao alerta atual.</span><span class="sxs-lookup"><span data-stu-id="a23d6-112">Name of the resource that is related to current alert.</span></span> <span data-ttu-id="a23d6-113">**Obrigatório**.</span><span class="sxs-lookup"><span data-stu-id="a23d6-113">**Required**.</span></span>|
|<span data-ttu-id="a23d6-114">resourceType</span><span class="sxs-lookup"><span data-stu-id="a23d6-114">resourceType</span></span>|[<span data-ttu-id="a23d6-115">securityResourceType</span><span class="sxs-lookup"><span data-stu-id="a23d6-115">securityResourceType</span></span>](#securityresourcetype-values)|<span data-ttu-id="a23d6-116">Representa o tipo de recursos de segurança relacionados a um alerta.</span><span class="sxs-lookup"><span data-stu-id="a23d6-116">Represents type of security resources related to an alert.</span></span> <span data-ttu-id="a23d6-117">Os valores possíveis são: `attacked` e `related`.</span><span class="sxs-lookup"><span data-stu-id="a23d6-117">Possible values are: `attacked`, `related`.</span></span>|

### <a name="securityresourcetype-values"></a><span data-ttu-id="a23d6-118">valores de securityResourceType</span><span class="sxs-lookup"><span data-stu-id="a23d6-118">securityResourceType values</span></span>

|<span data-ttu-id="a23d6-119">Membro</span><span class="sxs-lookup"><span data-stu-id="a23d6-119">Member</span></span>|<span data-ttu-id="a23d6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a23d6-120">Value</span></span>|<span data-ttu-id="a23d6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a23d6-121">Description</span></span>|
|-|-|-|
|<span data-ttu-id="a23d6-122">atacada</span><span class="sxs-lookup"><span data-stu-id="a23d6-122">attacked</span></span>|<span data-ttu-id="a23d6-123">1 </span><span class="sxs-lookup"><span data-stu-id="a23d6-123">1</span></span>|<span data-ttu-id="a23d6-124">O recurso foi atacado no alerta.</span><span class="sxs-lookup"><span data-stu-id="a23d6-124">The resource was attacked in the alert.</span></span>|
|<span data-ttu-id="a23d6-125">correspondente</span><span class="sxs-lookup"><span data-stu-id="a23d6-125">related</span></span>|<span data-ttu-id="a23d6-126">2 </span><span class="sxs-lookup"><span data-stu-id="a23d6-126">2</span></span>|<span data-ttu-id="a23d6-127">O recurso está relacionado ao alerta, embora não seja atacado diretamente.</span><span class="sxs-lookup"><span data-stu-id="a23d6-127">The resource is related to the alert, though not directly attacked.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a23d6-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a23d6-128">JSON representation</span></span>

<span data-ttu-id="a23d6-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a23d6-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.securityResource"
}-->

```json
{
  "resource": "String",
  "resourceType": "@odata.type: microsoft.graph.securityResourceType"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


