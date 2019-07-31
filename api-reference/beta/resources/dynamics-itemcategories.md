---
title: tipo de recurso docategories
description: Uma categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 18017c580637bb53a70b5f7a331ff7be1dc7a07c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972919"
---
# <a name="itemcategories-resource-type"></a><span data-ttu-id="00da5-103">tipo de recurso docategories</span><span class="sxs-lookup"><span data-stu-id="00da5-103">itemCategories resource type</span></span>
<span data-ttu-id="00da5-104">Representa uma categoria de vários itens no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="00da5-104">Represents a category for a number of items in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="00da5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="00da5-105">Methods</span></span>

| <span data-ttu-id="00da5-106">Método</span><span class="sxs-lookup"><span data-stu-id="00da5-106">Method</span></span>                                                          | <span data-ttu-id="00da5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="00da5-107">Return Type</span></span>  |<span data-ttu-id="00da5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="00da5-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="00da5-109">Obter as categorias</span><span class="sxs-lookup"><span data-stu-id="00da5-109">Get itemCategories</span></span>](../api/dynamics-itemcategories-get.md)      |<span data-ttu-id="00da5-110">Categoria de</span><span class="sxs-lookup"><span data-stu-id="00da5-110">itemCategories</span></span>|<span data-ttu-id="00da5-111">Obtenha uma categoria de item.</span><span class="sxs-lookup"><span data-stu-id="00da5-111">Get an item category.</span></span>   |
|[<span data-ttu-id="00da5-112">Postar categorias</span><span class="sxs-lookup"><span data-stu-id="00da5-112">Post itemCategories</span></span>](../api/dynamics-create-itemcategories.md)  |<span data-ttu-id="00da5-113">Categoria de</span><span class="sxs-lookup"><span data-stu-id="00da5-113">itemCategories</span></span>|<span data-ttu-id="00da5-114">Criar uma categoria de item.</span><span class="sxs-lookup"><span data-stu-id="00da5-114">Create an item category.</span></span>|
|[<span data-ttu-id="00da5-115">Patch, categorias</span><span class="sxs-lookup"><span data-stu-id="00da5-115">Patch itemCategories</span></span>](../api/dynamics-itemcategories-update.md) |<span data-ttu-id="00da5-116">Categoria de</span><span class="sxs-lookup"><span data-stu-id="00da5-116">itemCategories</span></span>|<span data-ttu-id="00da5-117">Atualize uma categoria de item.</span><span class="sxs-lookup"><span data-stu-id="00da5-117">Update an item category.</span></span>|
|[<span data-ttu-id="00da5-118">Excluir myCategories</span><span class="sxs-lookup"><span data-stu-id="00da5-118">Delete itemCategories</span></span>](../api/dynamics-itemcategories-delete.md)|<span data-ttu-id="00da5-119">none</span><span class="sxs-lookup"><span data-stu-id="00da5-119">none</span></span>          |<span data-ttu-id="00da5-120">Excluir uma categoria de item.</span><span class="sxs-lookup"><span data-stu-id="00da5-120">Delete an item category.</span></span>|

## <a name="properties"></a><span data-ttu-id="00da5-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00da5-121">Properties</span></span>
| <span data-ttu-id="00da5-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00da5-122">Property</span></span>           | <span data-ttu-id="00da5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="00da5-123">Type</span></span>   |<span data-ttu-id="00da5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="00da5-124">Description</span></span>                                     |
|:-------------------|:-------|:-----------------------------------------------|
|<span data-ttu-id="00da5-125">id</span><span class="sxs-lookup"><span data-stu-id="00da5-125">id</span></span>                  |<span data-ttu-id="00da5-126">GUID</span><span class="sxs-lookup"><span data-stu-id="00da5-126">GUID</span></span>    |<span data-ttu-id="00da5-127">A ID exclusiva do mycategory.</span><span class="sxs-lookup"><span data-stu-id="00da5-127">The unique ID of the itemCategory.</span></span> <span data-ttu-id="00da5-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="00da5-128">Non-editable.</span></span>|
|<span data-ttu-id="00da5-129">código</span><span class="sxs-lookup"><span data-stu-id="00da5-129">code</span></span>                |<span data-ttu-id="00da5-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00da5-130">string</span></span>  |<span data-ttu-id="00da5-131">O código de categoria.</span><span class="sxs-lookup"><span data-stu-id="00da5-131">The itemCategory code.</span></span>                          |
|<span data-ttu-id="00da5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="00da5-132">displayName</span></span>         |<span data-ttu-id="00da5-133">string</span><span class="sxs-lookup"><span data-stu-id="00da5-133">string</span></span>  |<span data-ttu-id="00da5-134">O nome de exibição de docategorias.</span><span class="sxs-lookup"><span data-stu-id="00da5-134">The itemCategories display name.</span></span>                |
|<span data-ttu-id="00da5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00da5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="00da5-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="00da5-136">datetime</span></span>|<span data-ttu-id="00da5-137">A última data e hora em que a categoria foi modificada.</span><span class="sxs-lookup"><span data-stu-id="00da5-137">The last datetime the itemCategory was modified.</span></span> <span data-ttu-id="00da5-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00da5-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="00da5-139">Relações</span><span class="sxs-lookup"><span data-stu-id="00da5-139">Relationships</span></span>
<span data-ttu-id="00da5-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00da5-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00da5-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00da5-141">JSON representation</span></span>

<span data-ttu-id="00da5-142">Veja a seguir uma representação JSON das categorias.</span><span class="sxs-lookup"><span data-stu-id="00da5-142">Here is a JSON representation of the itemCategories.</span></span>

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

