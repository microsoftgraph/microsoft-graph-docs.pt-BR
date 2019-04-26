---
title: tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bf5ee33ec7d217c0bc4c6e4d35666d6e9f34dadb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340589"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="bed8b-103">tipo de recurso educationCategory</span><span class="sxs-lookup"><span data-stu-id="bed8b-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bed8b-104">Uma categoria que pode ser aplicada a atribuições.</span><span class="sxs-lookup"><span data-stu-id="bed8b-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="bed8b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="bed8b-105">Methods</span></span>

| <span data-ttu-id="bed8b-106">Método</span><span class="sxs-lookup"><span data-stu-id="bed8b-106">Method</span></span>           | <span data-ttu-id="bed8b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bed8b-107">Return Type</span></span>    |<span data-ttu-id="bed8b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bed8b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bed8b-109">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="bed8b-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="bed8b-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="bed8b-110">educationCategory</span></span>](educationCategory.md) | <span data-ttu-id="bed8b-111">Obter um **educationCategory**existente.</span><span class="sxs-lookup"><span data-stu-id="bed8b-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="bed8b-112">Excluir categoria</span><span class="sxs-lookup"><span data-stu-id="bed8b-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="bed8b-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bed8b-113">None</span></span> | <span data-ttu-id="bed8b-114">Remover um **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="bed8b-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="bed8b-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bed8b-115">Properties</span></span>
| <span data-ttu-id="bed8b-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bed8b-116">Property</span></span>     | <span data-ttu-id="bed8b-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="bed8b-117">Type</span></span>   |<span data-ttu-id="bed8b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="bed8b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bed8b-119">id</span><span class="sxs-lookup"><span data-stu-id="bed8b-119">id</span></span>|<span data-ttu-id="bed8b-120">String</span><span class="sxs-lookup"><span data-stu-id="bed8b-120">String</span></span>|<span data-ttu-id="bed8b-121">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="bed8b-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="bed8b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="bed8b-122">displayName</span></span>|<span data-ttu-id="bed8b-123">String</span><span class="sxs-lookup"><span data-stu-id="bed8b-123">String</span></span>|<span data-ttu-id="bed8b-124">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="bed8b-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bed8b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bed8b-125">JSON representation</span></span>

<span data-ttu-id="bed8b-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bed8b-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
