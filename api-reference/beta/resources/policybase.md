---
title: Tipo de recurso policyBase
description: Representa um tipo de base abstrato para tipos de política herdado.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b495503cf01ce13e5f5d44d371b824a1eedfccb5
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760845"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="3fb2b-103">Tipo de recurso policyBase</span><span class="sxs-lookup"><span data-stu-id="3fb2b-103">policyBase resource type</span></span>

<span data-ttu-id="3fb2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fb2b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fb2b-105">Representa um tipo de base abstrato para tipos de política herdado.</span><span class="sxs-lookup"><span data-stu-id="3fb2b-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="3fb2b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3fb2b-106">Methods</span></span>

<span data-ttu-id="3fb2b-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3fb2b-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="3fb2b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fb2b-108">Properties</span></span>

| <span data-ttu-id="3fb2b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fb2b-109">Property</span></span>     | <span data-ttu-id="3fb2b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fb2b-110">Type</span></span>        | <span data-ttu-id="3fb2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fb2b-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3fb2b-112">id</span><span class="sxs-lookup"><span data-stu-id="3fb2b-112">id</span></span>|<span data-ttu-id="3fb2b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fb2b-113">String</span></span>| <span data-ttu-id="3fb2b-114">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="3fb2b-114">Unique identifier for this policy.</span></span> <span data-ttu-id="3fb2b-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3fb2b-115">Read-only.</span></span>|
|<span data-ttu-id="3fb2b-116">description</span><span class="sxs-lookup"><span data-stu-id="3fb2b-116">description</span></span>|<span data-ttu-id="3fb2b-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fb2b-117">String</span></span>| <span data-ttu-id="3fb2b-118">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="3fb2b-118">Description for this policy.</span></span>|
|<span data-ttu-id="3fb2b-119">displayName</span><span class="sxs-lookup"><span data-stu-id="3fb2b-119">displayName</span></span>|<span data-ttu-id="3fb2b-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fb2b-120">String</span></span>| <span data-ttu-id="3fb2b-121">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="3fb2b-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3fb2b-122">Relações</span><span class="sxs-lookup"><span data-stu-id="3fb2b-122">Relationships</span></span>

<span data-ttu-id="3fb2b-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3fb2b-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fb2b-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fb2b-124">JSON representation</span></span>

<span data-ttu-id="3fb2b-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fb2b-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
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

