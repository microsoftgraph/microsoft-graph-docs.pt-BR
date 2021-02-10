---
title: Tipo de recurso policyBase
description: Representa um tipo base abstrato dos tipos de política dos quais herdar.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: deb6b11d9ebb8e2ef4ec9f5a2874903577f593b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156333"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="0d39c-103">Tipo de recurso policyBase</span><span class="sxs-lookup"><span data-stu-id="0d39c-103">policyBase resource type</span></span>

<span data-ttu-id="0d39c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d39c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d39c-105">Representa um tipo básico abstrato dos tipos de política dos quais herdar.</span><span class="sxs-lookup"><span data-stu-id="0d39c-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="0d39c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0d39c-106">Methods</span></span>

<span data-ttu-id="0d39c-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d39c-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="0d39c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d39c-108">Properties</span></span>

| <span data-ttu-id="0d39c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d39c-109">Property</span></span>     | <span data-ttu-id="0d39c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d39c-110">Type</span></span>        | <span data-ttu-id="0d39c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d39c-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d39c-112">id</span><span class="sxs-lookup"><span data-stu-id="0d39c-112">id</span></span>|<span data-ttu-id="0d39c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d39c-113">String</span></span>| <span data-ttu-id="0d39c-114">Identificador exclusivo desta política.</span><span class="sxs-lookup"><span data-stu-id="0d39c-114">Unique identifier for this policy.</span></span> <span data-ttu-id="0d39c-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0d39c-115">Read-only.</span></span>|
|<span data-ttu-id="0d39c-116">description</span><span class="sxs-lookup"><span data-stu-id="0d39c-116">description</span></span>|<span data-ttu-id="0d39c-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d39c-117">String</span></span>| <span data-ttu-id="0d39c-118">Descrição desta política.</span><span class="sxs-lookup"><span data-stu-id="0d39c-118">Description for this policy.</span></span>|
|<span data-ttu-id="0d39c-119">displayName</span><span class="sxs-lookup"><span data-stu-id="0d39c-119">displayName</span></span>|<span data-ttu-id="0d39c-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d39c-120">String</span></span>| <span data-ttu-id="0d39c-121">Nome para exibição desta política.</span><span class="sxs-lookup"><span data-stu-id="0d39c-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0d39c-122">Relações</span><span class="sxs-lookup"><span data-stu-id="0d39c-122">Relationships</span></span>

<span data-ttu-id="0d39c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d39c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d39c-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d39c-124">JSON representation</span></span>

<span data-ttu-id="0d39c-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d39c-125">The following is a JSON representation of the resource.</span></span>

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
