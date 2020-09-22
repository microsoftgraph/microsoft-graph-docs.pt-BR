---
title: tipo de recurso policyBase
description: Representa um tipo de base abstrato para o qual os tipos de política herdam.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 527549d4af2e2fb103cb7d2484d844fd3c876e4c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033637"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="6a61a-103">tipo de recurso policyBase</span><span class="sxs-lookup"><span data-stu-id="6a61a-103">policyBase resource type</span></span>

<span data-ttu-id="6a61a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a61a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a61a-105">Representa um tipo de base abstrato para o qual os tipos de política herdam.</span><span class="sxs-lookup"><span data-stu-id="6a61a-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="6a61a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6a61a-106">Methods</span></span>

<span data-ttu-id="6a61a-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a61a-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="6a61a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a61a-108">Properties</span></span>

| <span data-ttu-id="6a61a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a61a-109">Property</span></span>     | <span data-ttu-id="6a61a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a61a-110">Type</span></span>        | <span data-ttu-id="6a61a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a61a-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a61a-112">id</span><span class="sxs-lookup"><span data-stu-id="6a61a-112">id</span></span>|<span data-ttu-id="6a61a-113">String</span><span class="sxs-lookup"><span data-stu-id="6a61a-113">String</span></span>| <span data-ttu-id="6a61a-114">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="6a61a-114">Unique identifier for this policy.</span></span> <span data-ttu-id="6a61a-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a61a-115">Read-only.</span></span>|
|<span data-ttu-id="6a61a-116">description</span><span class="sxs-lookup"><span data-stu-id="6a61a-116">description</span></span>|<span data-ttu-id="6a61a-117">String</span><span class="sxs-lookup"><span data-stu-id="6a61a-117">String</span></span>| <span data-ttu-id="6a61a-118">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="6a61a-118">Description for this policy.</span></span>|
|<span data-ttu-id="6a61a-119">displayName</span><span class="sxs-lookup"><span data-stu-id="6a61a-119">displayName</span></span>|<span data-ttu-id="6a61a-120">String</span><span class="sxs-lookup"><span data-stu-id="6a61a-120">String</span></span>| <span data-ttu-id="6a61a-121">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="6a61a-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6a61a-122">Relações</span><span class="sxs-lookup"><span data-stu-id="6a61a-122">Relationships</span></span>

<span data-ttu-id="6a61a-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a61a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a61a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a61a-124">JSON representation</span></span>

<span data-ttu-id="6a61a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a61a-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policyBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

