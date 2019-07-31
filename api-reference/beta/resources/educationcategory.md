---
title: tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4732bab700ab23869e0463437288b1aa8897aa0e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972783"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="7afb3-103">tipo de recurso educationCategory</span><span class="sxs-lookup"><span data-stu-id="7afb3-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7afb3-104">Uma categoria que pode ser aplicada a atribuições.</span><span class="sxs-lookup"><span data-stu-id="7afb3-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="7afb3-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7afb3-105">Methods</span></span>

| <span data-ttu-id="7afb3-106">Método</span><span class="sxs-lookup"><span data-stu-id="7afb3-106">Method</span></span>           | <span data-ttu-id="7afb3-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7afb3-107">Return Type</span></span>    |<span data-ttu-id="7afb3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7afb3-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7afb3-109">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="7afb3-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="7afb3-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="7afb3-110">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="7afb3-111">Obter um **educationCategory**existente.</span><span class="sxs-lookup"><span data-stu-id="7afb3-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="7afb3-112">Excluir categoria</span><span class="sxs-lookup"><span data-stu-id="7afb3-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="7afb3-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7afb3-113">None</span></span> | <span data-ttu-id="7afb3-114">Remover um **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="7afb3-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="7afb3-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7afb3-115">Properties</span></span>
| <span data-ttu-id="7afb3-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7afb3-116">Property</span></span>     | <span data-ttu-id="7afb3-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="7afb3-117">Type</span></span>   |<span data-ttu-id="7afb3-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7afb3-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7afb3-119">id</span><span class="sxs-lookup"><span data-stu-id="7afb3-119">id</span></span>|<span data-ttu-id="7afb3-120">String</span><span class="sxs-lookup"><span data-stu-id="7afb3-120">String</span></span>|<span data-ttu-id="7afb3-121">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="7afb3-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="7afb3-122">displayName</span><span class="sxs-lookup"><span data-stu-id="7afb3-122">displayName</span></span>|<span data-ttu-id="7afb3-123">String</span><span class="sxs-lookup"><span data-stu-id="7afb3-123">String</span></span>|<span data-ttu-id="7afb3-124">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="7afb3-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7afb3-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7afb3-125">JSON representation</span></span>

<span data-ttu-id="7afb3-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7afb3-126">The following is a JSON representation of the resource.</span></span>

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
