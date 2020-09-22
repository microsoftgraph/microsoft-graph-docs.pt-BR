---
title: tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82ad4f009ca76625c148e8a42e58385195466fbb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095538"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="9d65c-103">tipo de recurso educationCategory</span><span class="sxs-lookup"><span data-stu-id="9d65c-103">educationCategory resource type</span></span>

<span data-ttu-id="9d65c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d65c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d65c-105">Uma categoria que pode ser aplicada a atribuições.</span><span class="sxs-lookup"><span data-stu-id="9d65c-105">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="9d65c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9d65c-106">Methods</span></span>

| <span data-ttu-id="9d65c-107">Método</span><span class="sxs-lookup"><span data-stu-id="9d65c-107">Method</span></span>           | <span data-ttu-id="9d65c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9d65c-108">Return Type</span></span>    |<span data-ttu-id="9d65c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d65c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9d65c-110">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="9d65c-110">Create category</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="9d65c-111">educationCategory</span><span class="sxs-lookup"><span data-stu-id="9d65c-111">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="9d65c-112">Criar um novo **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="9d65c-112">Create a new **educationCategory**.</span></span>|
|[<span data-ttu-id="9d65c-113">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="9d65c-113">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="9d65c-114">educationCategory</span><span class="sxs-lookup"><span data-stu-id="9d65c-114">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="9d65c-115">Obter um **educationCategory**existente.</span><span class="sxs-lookup"><span data-stu-id="9d65c-115">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="9d65c-116">Excluir categoria</span><span class="sxs-lookup"><span data-stu-id="9d65c-116">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="9d65c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d65c-117">None</span></span> | <span data-ttu-id="9d65c-118">Remover um **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="9d65c-118">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="9d65c-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d65c-119">Properties</span></span>
| <span data-ttu-id="9d65c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d65c-120">Property</span></span>     | <span data-ttu-id="9d65c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d65c-121">Type</span></span>   |<span data-ttu-id="9d65c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d65c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d65c-123">id</span><span class="sxs-lookup"><span data-stu-id="9d65c-123">id</span></span>|<span data-ttu-id="9d65c-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d65c-124">String</span></span>|<span data-ttu-id="9d65c-125">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="9d65c-125">Unique identifier for the category.</span></span>|
|<span data-ttu-id="9d65c-126">displayName</span><span class="sxs-lookup"><span data-stu-id="9d65c-126">displayName</span></span>|<span data-ttu-id="9d65c-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d65c-127">String</span></span>|<span data-ttu-id="9d65c-128">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="9d65c-128">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d65c-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d65c-129">JSON representation</span></span>

<span data-ttu-id="9d65c-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d65c-130">The following is a JSON representation of the resource.</span></span>

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


