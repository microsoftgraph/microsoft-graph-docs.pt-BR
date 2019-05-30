---
title: tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: dd9eccac3a1b6b1bdc3b0eca4c87b5e29e2135a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536170"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="4ea90-103">tipo de recurso educationCategory</span><span class="sxs-lookup"><span data-stu-id="4ea90-103">educationCategory resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ea90-104">Uma categoria que pode ser aplicada a atribuições.</span><span class="sxs-lookup"><span data-stu-id="4ea90-104">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="4ea90-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4ea90-105">Methods</span></span>

| <span data-ttu-id="4ea90-106">Método</span><span class="sxs-lookup"><span data-stu-id="4ea90-106">Method</span></span>           | <span data-ttu-id="4ea90-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4ea90-107">Return Type</span></span>    |<span data-ttu-id="4ea90-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ea90-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ea90-109">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="4ea90-109">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="4ea90-110">educationCategory</span><span class="sxs-lookup"><span data-stu-id="4ea90-110">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="4ea90-111">Obter um **educationCategory**existente.</span><span class="sxs-lookup"><span data-stu-id="4ea90-111">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="4ea90-112">Excluir categoria</span><span class="sxs-lookup"><span data-stu-id="4ea90-112">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="4ea90-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ea90-113">None</span></span> | <span data-ttu-id="4ea90-114">Remover um **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="4ea90-114">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="4ea90-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ea90-115">Properties</span></span>
| <span data-ttu-id="4ea90-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ea90-116">Property</span></span>     | <span data-ttu-id="4ea90-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ea90-117">Type</span></span>   |<span data-ttu-id="4ea90-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ea90-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ea90-119">id</span><span class="sxs-lookup"><span data-stu-id="4ea90-119">id</span></span>|<span data-ttu-id="4ea90-120">String</span><span class="sxs-lookup"><span data-stu-id="4ea90-120">String</span></span>|<span data-ttu-id="4ea90-121">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="4ea90-121">Unique identifier for the category.</span></span>|
|<span data-ttu-id="4ea90-122">displayName</span><span class="sxs-lookup"><span data-stu-id="4ea90-122">displayName</span></span>|<span data-ttu-id="4ea90-123">String</span><span class="sxs-lookup"><span data-stu-id="4ea90-123">String</span></span>|<span data-ttu-id="4ea90-124">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="4ea90-124">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ea90-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ea90-125">JSON representation</span></span>

<span data-ttu-id="4ea90-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ea90-126">The following is a JSON representation of the resource.</span></span>

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
