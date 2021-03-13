---
title: Tipo de recurso policyBase
description: Representa um tipo de base abstrato para tipos de política herdado.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a091fb23be66f476b03b725e29dced32b138c9bc
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761511"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="8b32f-103">Tipo de recurso policyBase</span><span class="sxs-lookup"><span data-stu-id="8b32f-103">policyBase resource type</span></span>

<span data-ttu-id="8b32f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b32f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b32f-105">Representa um tipo de base abstrato para tipos de política herdado.</span><span class="sxs-lookup"><span data-stu-id="8b32f-105">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="8b32f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8b32f-106">Methods</span></span>

<span data-ttu-id="8b32f-107">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b32f-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="8b32f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b32f-108">Properties</span></span>

| <span data-ttu-id="8b32f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b32f-109">Property</span></span>     | <span data-ttu-id="8b32f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b32f-110">Type</span></span>        | <span data-ttu-id="8b32f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b32f-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b32f-112">id</span><span class="sxs-lookup"><span data-stu-id="8b32f-112">id</span></span>|<span data-ttu-id="8b32f-113">String</span><span class="sxs-lookup"><span data-stu-id="8b32f-113">String</span></span>| <span data-ttu-id="8b32f-114">Identificador exclusivo dessa política.</span><span class="sxs-lookup"><span data-stu-id="8b32f-114">Unique identifier for this policy.</span></span> <span data-ttu-id="8b32f-115">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8b32f-115">Read-only.</span></span>|
|<span data-ttu-id="8b32f-116">description</span><span class="sxs-lookup"><span data-stu-id="8b32f-116">description</span></span>|<span data-ttu-id="8b32f-117">String</span><span class="sxs-lookup"><span data-stu-id="8b32f-117">String</span></span>| <span data-ttu-id="8b32f-118">Descrição dessa política.</span><span class="sxs-lookup"><span data-stu-id="8b32f-118">Description for this policy.</span></span>|
|<span data-ttu-id="8b32f-119">displayName</span><span class="sxs-lookup"><span data-stu-id="8b32f-119">displayName</span></span>|<span data-ttu-id="8b32f-120">String</span><span class="sxs-lookup"><span data-stu-id="8b32f-120">String</span></span>| <span data-ttu-id="8b32f-121">Nome de exibição para esta política.</span><span class="sxs-lookup"><span data-stu-id="8b32f-121">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8b32f-122">Relações</span><span class="sxs-lookup"><span data-stu-id="8b32f-122">Relationships</span></span>

<span data-ttu-id="8b32f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b32f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b32f-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b32f-124">JSON representation</span></span>

<span data-ttu-id="8b32f-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b32f-125">The following is a JSON representation of the resource.</span></span>

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
