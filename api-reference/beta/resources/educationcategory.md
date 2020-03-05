---
title: tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 14a399e09c74e439b64a273695b65e5a96cd25f8
ms.sourcegitcommit: fc818699566f03493937be95447eb9f656a1f950
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534392"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="c33f5-103">tipo de recurso educationCategory</span><span class="sxs-lookup"><span data-stu-id="c33f5-103">educationCategory resource type</span></span>

<span data-ttu-id="c33f5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c33f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c33f5-105">Uma categoria que pode ser aplicada a atribuições.</span><span class="sxs-lookup"><span data-stu-id="c33f5-105">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="c33f5-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c33f5-106">Methods</span></span>

| <span data-ttu-id="c33f5-107">Método</span><span class="sxs-lookup"><span data-stu-id="c33f5-107">Method</span></span>           | <span data-ttu-id="c33f5-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c33f5-108">Return Type</span></span>    |<span data-ttu-id="c33f5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33f5-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c33f5-110">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="c33f5-110">Create category</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="c33f5-111">educationCategory</span><span class="sxs-lookup"><span data-stu-id="c33f5-111">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="c33f5-112">Criar um novo **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="c33f5-112">Create a new **educationCategory**.</span></span>|
|[<span data-ttu-id="c33f5-113">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="c33f5-113">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="c33f5-114">educationCategory</span><span class="sxs-lookup"><span data-stu-id="c33f5-114">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="c33f5-115">Obter um **educationCategory**existente.</span><span class="sxs-lookup"><span data-stu-id="c33f5-115">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="c33f5-116">Excluir categoria</span><span class="sxs-lookup"><span data-stu-id="c33f5-116">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="c33f5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c33f5-117">None</span></span> | <span data-ttu-id="c33f5-118">Remover um **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="c33f5-118">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="c33f5-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c33f5-119">Properties</span></span>
| <span data-ttu-id="c33f5-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c33f5-120">Property</span></span>     | <span data-ttu-id="c33f5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c33f5-121">Type</span></span>   |<span data-ttu-id="c33f5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c33f5-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c33f5-123">id</span><span class="sxs-lookup"><span data-stu-id="c33f5-123">id</span></span>|<span data-ttu-id="c33f5-124">String</span><span class="sxs-lookup"><span data-stu-id="c33f5-124">String</span></span>|<span data-ttu-id="c33f5-125">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="c33f5-125">Unique identifier for the category.</span></span>|
|<span data-ttu-id="c33f5-126">displayName</span><span class="sxs-lookup"><span data-stu-id="c33f5-126">displayName</span></span>|<span data-ttu-id="c33f5-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c33f5-127">String</span></span>|<span data-ttu-id="c33f5-128">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="c33f5-128">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c33f5-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c33f5-129">JSON representation</span></span>

<span data-ttu-id="c33f5-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c33f5-130">The following is a JSON representation of the resource.</span></span>

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
