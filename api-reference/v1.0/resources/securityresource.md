---
title: tipo de recurso securityResource
description: Representa os recursos relacionados a um alerta.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d73ec9b3e5bf1da262bdd3f1846e24d0eececff3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983988"
---
# <a name="securityresource-resource-type"></a><span data-ttu-id="11397-103">tipo de recurso securityResource</span><span class="sxs-lookup"><span data-stu-id="11397-103">securityResource resource type</span></span>

<span data-ttu-id="11397-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11397-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11397-105">Representa os recursos relacionados a um alerta.</span><span class="sxs-lookup"><span data-stu-id="11397-105">Represents the resources related to an alert.</span></span>

## <a name="properties"></a><span data-ttu-id="11397-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11397-106">Properties</span></span>

| <span data-ttu-id="11397-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11397-107">Property</span></span>   | <span data-ttu-id="11397-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="11397-108">Type</span></span>|<span data-ttu-id="11397-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="11397-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11397-110">recurso</span><span class="sxs-lookup"><span data-stu-id="11397-110">resource</span></span>|<span data-ttu-id="11397-111">String</span><span class="sxs-lookup"><span data-stu-id="11397-111">String</span></span>|<span data-ttu-id="11397-112">Nome do recurso relacionado ao alerta atual.</span><span class="sxs-lookup"><span data-stu-id="11397-112">Name of the resource that is related to current alert.</span></span> <span data-ttu-id="11397-113">**Obrigatório**.</span><span class="sxs-lookup"><span data-stu-id="11397-113">**Required**.</span></span>|
|<span data-ttu-id="11397-114">resourceType</span><span class="sxs-lookup"><span data-stu-id="11397-114">resourceType</span></span>|[<span data-ttu-id="11397-115">securityResourceType</span><span class="sxs-lookup"><span data-stu-id="11397-115">securityResourceType</span></span>](#securityresourcetype-values)|<span data-ttu-id="11397-116">Representa o tipo de recursos de segurança relacionados a um alerta.</span><span class="sxs-lookup"><span data-stu-id="11397-116">Represents type of security resources related to an alert.</span></span> <span data-ttu-id="11397-117">Os valores possíveis são: `attacked` e `related`.</span><span class="sxs-lookup"><span data-stu-id="11397-117">Possible values are: `attacked`, `related`.</span></span>|

### <a name="securityresourcetype-values"></a><span data-ttu-id="11397-118">valores de securityResourceType</span><span class="sxs-lookup"><span data-stu-id="11397-118">securityResourceType values</span></span>

|<span data-ttu-id="11397-119">Membro</span><span class="sxs-lookup"><span data-stu-id="11397-119">Member</span></span>|<span data-ttu-id="11397-120">Valor</span><span class="sxs-lookup"><span data-stu-id="11397-120">Value</span></span>|<span data-ttu-id="11397-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="11397-121">Description</span></span>|
|-|-|-|
|<span data-ttu-id="11397-122">atacada</span><span class="sxs-lookup"><span data-stu-id="11397-122">attacked</span></span>|<span data-ttu-id="11397-123">1 </span><span class="sxs-lookup"><span data-stu-id="11397-123">1</span></span>|<span data-ttu-id="11397-124">O recurso foi atacado no alerta.</span><span class="sxs-lookup"><span data-stu-id="11397-124">The resource was attacked in the alert.</span></span>|
|<span data-ttu-id="11397-125">correspondente</span><span class="sxs-lookup"><span data-stu-id="11397-125">related</span></span>|<span data-ttu-id="11397-126">2 </span><span class="sxs-lookup"><span data-stu-id="11397-126">2</span></span>|<span data-ttu-id="11397-127">O recurso está relacionado ao alerta, embora não seja atacado diretamente.</span><span class="sxs-lookup"><span data-stu-id="11397-127">The resource is related to the alert, though not directly attacked.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11397-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11397-128">JSON representation</span></span>

<span data-ttu-id="11397-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11397-129">The following is a JSON representation of the resource.</span></span>

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

