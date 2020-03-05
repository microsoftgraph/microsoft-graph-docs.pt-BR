---
title: tipo de recurso policyBase
description: Representa um tipo de base abstrato para o qual os tipos de política herdam.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7675183d5b6316db42d9860ac54009b321720a29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521597"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="0b7fd-103">tipo de recurso policyBase</span><span class="sxs-lookup"><span data-stu-id="0b7fd-103">policyBase resource type</span></span>

<span data-ttu-id="0b7fd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0b7fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b7fd-105">Representa um tipo de base abstrato para o qual os tipos de política herdam.</span><span class="sxs-lookup"><span data-stu-id="0b7fd-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="0b7fd-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b7fd-106">Methods</span></span>

<span data-ttu-id="0b7fd-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b7fd-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="0b7fd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b7fd-108">Properties</span></span>

| <span data-ttu-id="0b7fd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b7fd-109">Property</span></span>     | <span data-ttu-id="0b7fd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b7fd-110">Type</span></span>        | <span data-ttu-id="0b7fd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b7fd-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b7fd-112">id</span><span class="sxs-lookup"><span data-stu-id="0b7fd-112">id</span></span>|<span data-ttu-id="0b7fd-113">String</span><span class="sxs-lookup"><span data-stu-id="0b7fd-113">String</span></span>| <span data-ttu-id="0b7fd-114">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="0b7fd-114">Unique identifier for this policy.</span></span> <span data-ttu-id="0b7fd-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0b7fd-115">Read-only.</span></span>|
|<span data-ttu-id="0b7fd-116">description</span><span class="sxs-lookup"><span data-stu-id="0b7fd-116">description</span></span>|<span data-ttu-id="0b7fd-117">String</span><span class="sxs-lookup"><span data-stu-id="0b7fd-117">String</span></span>| <span data-ttu-id="0b7fd-118">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="0b7fd-118">Description for this policy.</span></span>|
|<span data-ttu-id="0b7fd-119">displayName</span><span class="sxs-lookup"><span data-stu-id="0b7fd-119">displayName</span></span>|<span data-ttu-id="0b7fd-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b7fd-120">String</span></span>| <span data-ttu-id="0b7fd-121">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="0b7fd-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0b7fd-122">Relações</span><span class="sxs-lookup"><span data-stu-id="0b7fd-122">Relationships</span></span>

<span data-ttu-id="0b7fd-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b7fd-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b7fd-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b7fd-124">JSON representation</span></span>

<span data-ttu-id="0b7fd-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b7fd-125">The following is a JSON representation of the resource.</span></span>

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