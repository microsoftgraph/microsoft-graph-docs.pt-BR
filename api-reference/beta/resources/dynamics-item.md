---
title: tipo de recurso itens
description: Um objeto de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 438fa0035b2c84b6fe702e3b1765e3d8b5adaf9d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006623"
---
# <a name="items-resource-type"></a><span data-ttu-id="8c6a9-103">tipo de recurso itens</span><span class="sxs-lookup"><span data-stu-id="8c6a9-103">items resource type</span></span>
<span data-ttu-id="8c6a9-104">Representa um item no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-104">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8c6a9-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8c6a9-105">Methods</span></span>

| <span data-ttu-id="8c6a9-106">Método</span><span class="sxs-lookup"><span data-stu-id="8c6a9-106">Method</span></span>                                      |<span data-ttu-id="8c6a9-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8c6a9-107">Return Type</span></span>|<span data-ttu-id="8c6a9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c6a9-108">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="8c6a9-109">Obter itens</span><span class="sxs-lookup"><span data-stu-id="8c6a9-109">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="8c6a9-110">items</span><span class="sxs-lookup"><span data-stu-id="8c6a9-110">items</span></span>     |<span data-ttu-id="8c6a9-111">Obtém um objeto item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-111">Gets an item object.</span></span>   |
|[<span data-ttu-id="8c6a9-112">Itens post</span><span class="sxs-lookup"><span data-stu-id="8c6a9-112">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="8c6a9-113">items</span><span class="sxs-lookup"><span data-stu-id="8c6a9-113">items</span></span>     |<span data-ttu-id="8c6a9-114">Cria um objeto item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-114">Creates an item object.</span></span>|
|[<span data-ttu-id="8c6a9-115">Item de patch</span><span class="sxs-lookup"><span data-stu-id="8c6a9-115">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="8c6a9-116">items</span><span class="sxs-lookup"><span data-stu-id="8c6a9-116">items</span></span>     |<span data-ttu-id="8c6a9-117">Atualiza um objeto item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-117">Updates an item object.</span></span>|
|[<span data-ttu-id="8c6a9-118">Excluir itens</span><span class="sxs-lookup"><span data-stu-id="8c6a9-118">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="8c6a9-119">none</span><span class="sxs-lookup"><span data-stu-id="8c6a9-119">none</span></span>      |<span data-ttu-id="8c6a9-120">Exclui um objeto item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-120">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8c6a9-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c6a9-121">Properties</span></span>
| <span data-ttu-id="8c6a9-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c6a9-122">Property</span></span>           | <span data-ttu-id="8c6a9-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c6a9-123">Type</span></span> |<span data-ttu-id="8c6a9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c6a9-124">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="8c6a9-125">id</span><span class="sxs-lookup"><span data-stu-id="8c6a9-125">id</span></span>                  |<span data-ttu-id="8c6a9-126">GUID</span><span class="sxs-lookup"><span data-stu-id="8c6a9-126">GUID</span></span>    |<span data-ttu-id="8c6a9-127">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-127">The unique ID of the item.</span></span> <span data-ttu-id="8c6a9-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-128">Non-editable.</span></span>             |
|<span data-ttu-id="8c6a9-129">number</span><span class="sxs-lookup"><span data-stu-id="8c6a9-129">number</span></span>              |<span data-ttu-id="8c6a9-130">string</span><span class="sxs-lookup"><span data-stu-id="8c6a9-130">string</span></span>  |<span data-ttu-id="8c6a9-131">O número do item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-131">The item number.</span></span>                                     |
|<span data-ttu-id="8c6a9-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8c6a9-132">displayName</span></span>         |<span data-ttu-id="8c6a9-133">string</span><span class="sxs-lookup"><span data-stu-id="8c6a9-133">string</span></span>  |<span data-ttu-id="8c6a9-134">Especifica uma descrição do item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-134">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="8c6a9-135">type</span><span class="sxs-lookup"><span data-stu-id="8c6a9-135">type</span></span>                |<span data-ttu-id="8c6a9-136">numéricos</span><span class="sxs-lookup"><span data-stu-id="8c6a9-136">numeric</span></span> |<span data-ttu-id="8c6a9-137">O tipo de inventário para o item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-137">The inventory type for the item.</span></span> <span data-ttu-id="8c6a9-138">1 = item de estoque, 2 = item de serviço.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-138">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="8c6a9-139">Essa é uma propriedade obrigatória.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-139">This is a required property.</span></span>|
|<span data-ttu-id="8c6a9-140">bloqueou</span><span class="sxs-lookup"><span data-stu-id="8c6a9-140">blocked</span></span>             |<span data-ttu-id="8c6a9-141">booliano</span><span class="sxs-lookup"><span data-stu-id="8c6a9-141">boolean</span></span> |<span data-ttu-id="8c6a9-142">Especifica que as transações com o item não podem ser lançadas, por exemplo, porque o item está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-142">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="8c6a9-143">Defina como **true**se o item estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-143">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="8c6a9-144">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="8c6a9-144">baseUnitOfMeasureId</span></span> |<span data-ttu-id="8c6a9-145">GUID</span><span class="sxs-lookup"><span data-stu-id="8c6a9-145">GUID</span></span>    |<span data-ttu-id="8c6a9-146">Especifica a ID da unidade de medida.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-146">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="8c6a9-147">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="8c6a9-147">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="8c6a9-148">Extra. UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="8c6a9-148">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="8c6a9-149">Especifica a unidade na qual o item é mantido no estoque.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-149">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="8c6a9-150">GTIN</span><span class="sxs-lookup"><span data-stu-id="8c6a9-150">gtin</span></span>                |<span data-ttu-id="8c6a9-151">numéricos</span><span class="sxs-lookup"><span data-stu-id="8c6a9-151">numeric</span></span> |<span data-ttu-id="8c6a9-152">Este é o número do item comercial global.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-152">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="8c6a9-153">objectcategoryid</span><span class="sxs-lookup"><span data-stu-id="8c6a9-153">itemCategoryId</span></span>      |<span data-ttu-id="8c6a9-154">GUID</span><span class="sxs-lookup"><span data-stu-id="8c6a9-154">GUID</span></span> |<span data-ttu-id="8c6a9-155">Especifica a categoria à qual o item pertence.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-155">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="8c6a9-156">As categorias de item também contêm qualquer atributo de item atribuído.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-156">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="8c6a9-157">inventory</span><span class="sxs-lookup"><span data-stu-id="8c6a9-157">inventory</span></span>           |<span data-ttu-id="8c6a9-158">dígitos</span><span class="sxs-lookup"><span data-stu-id="8c6a9-158">decimal</span></span> |<span data-ttu-id="8c6a9-159">Especifica quantas unidades, como peças, caixas ou latas do item estão no estoque.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-159">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="8c6a9-160">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-160">Read-Only.</span></span>|
|<span data-ttu-id="8c6a9-161">PreçoUnitário</span><span class="sxs-lookup"><span data-stu-id="8c6a9-161">unitPrice</span></span>           |<span data-ttu-id="8c6a9-162">dígitos</span><span class="sxs-lookup"><span data-stu-id="8c6a9-162">decimal</span></span> |<span data-ttu-id="8c6a9-163">Especifica o preço de uma unidade do item na moeda especificada.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-163">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="8c6a9-164">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="8c6a9-164">priceIncludesTax</span></span>    |<span data-ttu-id="8c6a9-165">booliano</span><span class="sxs-lookup"><span data-stu-id="8c6a9-165">boolean</span></span> |<span data-ttu-id="8c6a9-166">Especifica que o PreçoUnitário inclui o imposto.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-166">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="8c6a9-167">Defina como **true**, se PreçoUnitário incluir imposto.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-167">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="8c6a9-168">unitCost</span><span class="sxs-lookup"><span data-stu-id="8c6a9-168">unitCost</span></span>            |<span data-ttu-id="8c6a9-169">dígitos</span><span class="sxs-lookup"><span data-stu-id="8c6a9-169">decimal</span></span> |<span data-ttu-id="8c6a9-170">Especifica o custo por unidade do item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-170">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="8c6a9-171">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="8c6a9-171">taxGroupId</span></span>          |<span data-ttu-id="8c6a9-172">GUID</span><span class="sxs-lookup"><span data-stu-id="8c6a9-172">GUID</span></span>    |<span data-ttu-id="8c6a9-173">Especifica a ID do grupo de impostos para o item.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-173">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="8c6a9-174">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="8c6a9-174">taxGroupCode</span></span>        |<span data-ttu-id="8c6a9-175">numéricos</span><span class="sxs-lookup"><span data-stu-id="8c6a9-175">numeric</span></span> |<span data-ttu-id="8c6a9-176">Um grupo de impostos representa um grupo de itens ou recursos de estoque sujeitos a termos de impostos idênticos.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-176">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="8c6a9-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c6a9-177">lastModifiedDateTime</span></span>|<span data-ttu-id="8c6a9-178">DateTime</span><span class="sxs-lookup"><span data-stu-id="8c6a9-178">datetime</span></span>|<span data-ttu-id="8c6a9-179">A última data/hora em que o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-179">The last datetime the item was modified.</span></span> <span data-ttu-id="8c6a9-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-180">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="8c6a9-181">Relações</span><span class="sxs-lookup"><span data-stu-id="8c6a9-181">Relationships</span></span>
<span data-ttu-id="8c6a9-182">Um grupo de impostos (taxGroupCode) deve existir na tabela de grupos de impostos.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-182">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c6a9-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c6a9-183">JSON representation</span></span>

<span data-ttu-id="8c6a9-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c6a9-184">Here is a JSON representation of the resource.</span></span>


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```


