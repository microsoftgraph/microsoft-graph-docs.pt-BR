---
title: tipo de recurso docategories
description: Uma categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d0a751fe076c76fcb703c4d910ac35d3d0593b15
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503842"
---
# <a name="itemcategories-resource-type"></a><span data-ttu-id="211cd-103">tipo de recurso docategories</span><span class="sxs-lookup"><span data-stu-id="211cd-103">itemCategories resource type</span></span>

<span data-ttu-id="211cd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="211cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="211cd-105">Representa uma categoria de vários itens no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="211cd-105">Represents a category for a number of items in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="211cd-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="211cd-106">Methods</span></span>

| <span data-ttu-id="211cd-107">Método</span><span class="sxs-lookup"><span data-stu-id="211cd-107">Method</span></span>                                                          | <span data-ttu-id="211cd-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="211cd-108">Return Type</span></span>  |<span data-ttu-id="211cd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="211cd-109">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="211cd-110">Obter as categorias</span><span class="sxs-lookup"><span data-stu-id="211cd-110">Get itemCategories</span></span>](../api/dynamics-itemcategories-get.md)      |<span data-ttu-id="211cd-111">Categoria de</span><span class="sxs-lookup"><span data-stu-id="211cd-111">itemCategories</span></span>|<span data-ttu-id="211cd-112">Obtenha uma categoria de item.</span><span class="sxs-lookup"><span data-stu-id="211cd-112">Get an item category.</span></span>   |
|[<span data-ttu-id="211cd-113">Postar categorias</span><span class="sxs-lookup"><span data-stu-id="211cd-113">Post itemCategories</span></span>](../api/dynamics-create-itemcategories.md)  |<span data-ttu-id="211cd-114">Categoria de</span><span class="sxs-lookup"><span data-stu-id="211cd-114">itemCategories</span></span>|<span data-ttu-id="211cd-115">Criar uma categoria de item.</span><span class="sxs-lookup"><span data-stu-id="211cd-115">Create an item category.</span></span>|
|[<span data-ttu-id="211cd-116">Patch, categorias</span><span class="sxs-lookup"><span data-stu-id="211cd-116">Patch itemCategories</span></span>](../api/dynamics-itemcategories-update.md) |<span data-ttu-id="211cd-117">Categoria de</span><span class="sxs-lookup"><span data-stu-id="211cd-117">itemCategories</span></span>|<span data-ttu-id="211cd-118">Atualize uma categoria de item.</span><span class="sxs-lookup"><span data-stu-id="211cd-118">Update an item category.</span></span>|
|[<span data-ttu-id="211cd-119">Excluir myCategories</span><span class="sxs-lookup"><span data-stu-id="211cd-119">Delete itemCategories</span></span>](../api/dynamics-itemcategories-delete.md)|<span data-ttu-id="211cd-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="211cd-120">none</span></span>          |<span data-ttu-id="211cd-121">Excluir uma categoria de item.</span><span class="sxs-lookup"><span data-stu-id="211cd-121">Delete an item category.</span></span>|

## <a name="properties"></a><span data-ttu-id="211cd-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="211cd-122">Properties</span></span>
| <span data-ttu-id="211cd-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="211cd-123">Property</span></span>           | <span data-ttu-id="211cd-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="211cd-124">Type</span></span>   |<span data-ttu-id="211cd-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="211cd-125">Description</span></span>                                     |
|:-------------------|:-------|:-----------------------------------------------|
|<span data-ttu-id="211cd-126">id</span><span class="sxs-lookup"><span data-stu-id="211cd-126">id</span></span>                  |<span data-ttu-id="211cd-127">GUID</span><span class="sxs-lookup"><span data-stu-id="211cd-127">GUID</span></span>    |<span data-ttu-id="211cd-128">A ID exclusiva do mycategory.</span><span class="sxs-lookup"><span data-stu-id="211cd-128">The unique ID of the itemCategory.</span></span> <span data-ttu-id="211cd-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="211cd-129">Non-editable.</span></span>|
|<span data-ttu-id="211cd-130">código</span><span class="sxs-lookup"><span data-stu-id="211cd-130">code</span></span>                |<span data-ttu-id="211cd-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="211cd-131">string</span></span>  |<span data-ttu-id="211cd-132">O código de categoria.</span><span class="sxs-lookup"><span data-stu-id="211cd-132">The itemCategory code.</span></span>                          |
|<span data-ttu-id="211cd-133">displayName</span><span class="sxs-lookup"><span data-stu-id="211cd-133">displayName</span></span>         |<span data-ttu-id="211cd-134">string</span><span class="sxs-lookup"><span data-stu-id="211cd-134">string</span></span>  |<span data-ttu-id="211cd-135">O nome de exibição de docategorias.</span><span class="sxs-lookup"><span data-stu-id="211cd-135">The itemCategories display name.</span></span>                |
|<span data-ttu-id="211cd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="211cd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="211cd-137">datetime</span><span class="sxs-lookup"><span data-stu-id="211cd-137">datetime</span></span>|<span data-ttu-id="211cd-138">A última data e hora em que a categoria foi modificada.</span><span class="sxs-lookup"><span data-stu-id="211cd-138">The last datetime the itemCategory was modified.</span></span> <span data-ttu-id="211cd-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="211cd-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="211cd-140">Relações</span><span class="sxs-lookup"><span data-stu-id="211cd-140">Relationships</span></span>
<span data-ttu-id="211cd-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="211cd-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="211cd-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="211cd-142">JSON representation</span></span>

<span data-ttu-id="211cd-143">Veja a seguir uma representação JSON das categorias.</span><span class="sxs-lookup"><span data-stu-id="211cd-143">Here is a JSON representation of the itemCategories.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

