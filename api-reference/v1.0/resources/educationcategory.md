---
title: Tipo de recurso educationCategory
description: Uma categoria que pode ser aplicada a atribuições.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dc18c74ba7720aed93d58ee974438857f967e23a
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912198"
---
# <a name="educationcategory-resource-type"></a><span data-ttu-id="6718d-103">Tipo de recurso educationCategory</span><span class="sxs-lookup"><span data-stu-id="6718d-103">educationCategory resource type</span></span>

<span data-ttu-id="6718d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6718d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6718d-105">Uma categoria que pode ser aplicada a atribuições.</span><span class="sxs-lookup"><span data-stu-id="6718d-105">A category that can be applied to assignments.</span></span>


## <a name="methods"></a><span data-ttu-id="6718d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6718d-106">Methods</span></span>

| <span data-ttu-id="6718d-107">Método</span><span class="sxs-lookup"><span data-stu-id="6718d-107">Method</span></span>           | <span data-ttu-id="6718d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6718d-108">Return Type</span></span>    |<span data-ttu-id="6718d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6718d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6718d-110">Criar categoria</span><span class="sxs-lookup"><span data-stu-id="6718d-110">Create category</span></span>](../api/educationclass-post-category.md) | [<span data-ttu-id="6718d-111">educationCategory</span><span class="sxs-lookup"><span data-stu-id="6718d-111">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="6718d-112">Criar uma nova **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="6718d-112">Create a new **educationCategory**.</span></span>|
|[<span data-ttu-id="6718d-113">Obter educationCategory</span><span class="sxs-lookup"><span data-stu-id="6718d-113">Get educationCategory</span></span>](../api/educationcategory-get.md) | [<span data-ttu-id="6718d-114">educationCategory</span><span class="sxs-lookup"><span data-stu-id="6718d-114">educationCategory</span></span>](educationcategory.md) | <span data-ttu-id="6718d-115">Obter uma **educationCategory existente**.</span><span class="sxs-lookup"><span data-stu-id="6718d-115">Get an existing **educationCategory**.</span></span>|
|[<span data-ttu-id="6718d-116">Excluir categoria</span><span class="sxs-lookup"><span data-stu-id="6718d-116">Delete category</span></span>](../api/educationcategory-delete.md) | <span data-ttu-id="6718d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6718d-117">None</span></span> | <span data-ttu-id="6718d-118">Remover uma **educationCategory**.</span><span class="sxs-lookup"><span data-stu-id="6718d-118">Remove an **educationCategory**.</span></span>|


## <a name="properties"></a><span data-ttu-id="6718d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6718d-119">Properties</span></span>
| <span data-ttu-id="6718d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6718d-120">Property</span></span>     | <span data-ttu-id="6718d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6718d-121">Type</span></span>   |<span data-ttu-id="6718d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6718d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6718d-123">id</span><span class="sxs-lookup"><span data-stu-id="6718d-123">id</span></span>|<span data-ttu-id="6718d-124">String</span><span class="sxs-lookup"><span data-stu-id="6718d-124">String</span></span>|<span data-ttu-id="6718d-125">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="6718d-125">Unique identifier for the category.</span></span>|
|<span data-ttu-id="6718d-126">displayName</span><span class="sxs-lookup"><span data-stu-id="6718d-126">displayName</span></span>|<span data-ttu-id="6718d-127">String</span><span class="sxs-lookup"><span data-stu-id="6718d-127">String</span></span>|<span data-ttu-id="6718d-128">Identificador exclusivo da categoria.</span><span class="sxs-lookup"><span data-stu-id="6718d-128">Unique identifier for the category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6718d-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6718d-129">JSON representation</span></span>

<span data-ttu-id="6718d-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6718d-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
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


