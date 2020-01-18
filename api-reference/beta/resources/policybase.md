---
title: tipo de recurso policyBase
description: Representa um tipo de base abstrato para o qual os tipos de política herdam.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 757f6771065d60818611662da4dfdcc37ff65853
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234130"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="2c4fa-103">tipo de recurso policyBase</span><span class="sxs-lookup"><span data-stu-id="2c4fa-103">policyBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c4fa-104">Representa um tipo de base abstrato para o qual os tipos de política herdam.</span><span class="sxs-lookup"><span data-stu-id="2c4fa-104">Represents an abstract base type for policy types to inherit from.</span></span>

## <a name="methods"></a><span data-ttu-id="2c4fa-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c4fa-105">Methods</span></span>

<span data-ttu-id="2c4fa-106">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="2c4fa-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="2c4fa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c4fa-107">Properties</span></span>

| <span data-ttu-id="2c4fa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c4fa-108">Property</span></span>     | <span data-ttu-id="2c4fa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c4fa-109">Type</span></span>        | <span data-ttu-id="2c4fa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c4fa-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2c4fa-111">id</span><span class="sxs-lookup"><span data-stu-id="2c4fa-111">id</span></span>|<span data-ttu-id="2c4fa-112">String</span><span class="sxs-lookup"><span data-stu-id="2c4fa-112">String</span></span>| <span data-ttu-id="2c4fa-113">Identificador exclusivo da política.</span><span class="sxs-lookup"><span data-stu-id="2c4fa-113">Unique identifier for this policy.</span></span> <span data-ttu-id="2c4fa-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2c4fa-114">Read-only.</span></span>|
|<span data-ttu-id="2c4fa-115">description</span><span class="sxs-lookup"><span data-stu-id="2c4fa-115">description</span></span>|<span data-ttu-id="2c4fa-116">String</span><span class="sxs-lookup"><span data-stu-id="2c4fa-116">String</span></span>| <span data-ttu-id="2c4fa-117">Descrição da política.</span><span class="sxs-lookup"><span data-stu-id="2c4fa-117">Description for this policy.</span></span>|
|<span data-ttu-id="2c4fa-118">displayName</span><span class="sxs-lookup"><span data-stu-id="2c4fa-118">displayName</span></span>|<span data-ttu-id="2c4fa-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c4fa-119">String</span></span>| <span data-ttu-id="2c4fa-120">Nome para exibição dessa política.</span><span class="sxs-lookup"><span data-stu-id="2c4fa-120">Display name for this policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2c4fa-121">Relações</span><span class="sxs-lookup"><span data-stu-id="2c4fa-121">Relationships</span></span>

<span data-ttu-id="2c4fa-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c4fa-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c4fa-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c4fa-123">JSON representation</span></span>

<span data-ttu-id="2c4fa-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c4fa-124">The following is a JSON representation of the resource.</span></span>

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