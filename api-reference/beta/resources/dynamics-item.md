---
title: tipo de recurso itens
description: Um objeto de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: e5578cc2bc05aedd417230cc3e9d3b171e9ba577
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503898"
---
# <a name="items-resource-type"></a><span data-ttu-id="50cb7-103">tipo de recurso itens</span><span class="sxs-lookup"><span data-stu-id="50cb7-103">items resource type</span></span>

<span data-ttu-id="50cb7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="50cb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50cb7-105">Representa um item no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="50cb7-105">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="50cb7-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="50cb7-106">Methods</span></span>

| <span data-ttu-id="50cb7-107">Método</span><span class="sxs-lookup"><span data-stu-id="50cb7-107">Method</span></span>                                      |<span data-ttu-id="50cb7-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50cb7-108">Return Type</span></span>|<span data-ttu-id="50cb7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="50cb7-109">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="50cb7-110">Obter itens</span><span class="sxs-lookup"><span data-stu-id="50cb7-110">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="50cb7-111">items</span><span class="sxs-lookup"><span data-stu-id="50cb7-111">items</span></span>     |<span data-ttu-id="50cb7-112">Obtém um objeto item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-112">Gets an item object.</span></span>   |
|[<span data-ttu-id="50cb7-113">Itens post</span><span class="sxs-lookup"><span data-stu-id="50cb7-113">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="50cb7-114">items</span><span class="sxs-lookup"><span data-stu-id="50cb7-114">items</span></span>     |<span data-ttu-id="50cb7-115">Cria um objeto item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-115">Creates an item object.</span></span>|
|[<span data-ttu-id="50cb7-116">Item de patch</span><span class="sxs-lookup"><span data-stu-id="50cb7-116">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="50cb7-117">items</span><span class="sxs-lookup"><span data-stu-id="50cb7-117">items</span></span>     |<span data-ttu-id="50cb7-118">Atualiza um objeto item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-118">Updates an item object.</span></span>|
|[<span data-ttu-id="50cb7-119">Excluir itens</span><span class="sxs-lookup"><span data-stu-id="50cb7-119">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="50cb7-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="50cb7-120">none</span></span>      |<span data-ttu-id="50cb7-121">Exclui um objeto item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-121">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50cb7-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50cb7-122">Properties</span></span>
| <span data-ttu-id="50cb7-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50cb7-123">Property</span></span>           | <span data-ttu-id="50cb7-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="50cb7-124">Type</span></span> |<span data-ttu-id="50cb7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="50cb7-125">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="50cb7-126">id</span><span class="sxs-lookup"><span data-stu-id="50cb7-126">id</span></span>                  |<span data-ttu-id="50cb7-127">GUID</span><span class="sxs-lookup"><span data-stu-id="50cb7-127">GUID</span></span>    |<span data-ttu-id="50cb7-128">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-128">The unique ID of the item.</span></span> <span data-ttu-id="50cb7-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="50cb7-129">Non-editable.</span></span>             |
|<span data-ttu-id="50cb7-130">number</span><span class="sxs-lookup"><span data-stu-id="50cb7-130">number</span></span>              |<span data-ttu-id="50cb7-131">string</span><span class="sxs-lookup"><span data-stu-id="50cb7-131">string</span></span>  |<span data-ttu-id="50cb7-132">O número do item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-132">The item number.</span></span>                                     |
|<span data-ttu-id="50cb7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="50cb7-133">displayName</span></span>         |<span data-ttu-id="50cb7-134">string</span><span class="sxs-lookup"><span data-stu-id="50cb7-134">string</span></span>  |<span data-ttu-id="50cb7-135">Especifica uma descrição do item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-135">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="50cb7-136">type</span><span class="sxs-lookup"><span data-stu-id="50cb7-136">type</span></span>                |<span data-ttu-id="50cb7-137">numéricos</span><span class="sxs-lookup"><span data-stu-id="50cb7-137">numeric</span></span> |<span data-ttu-id="50cb7-138">O tipo de inventário para o item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-138">The inventory type for the item.</span></span> <span data-ttu-id="50cb7-139">1 = item de estoque, 2 = item de serviço.</span><span class="sxs-lookup"><span data-stu-id="50cb7-139">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="50cb7-140">Essa é uma propriedade obrigatória.</span><span class="sxs-lookup"><span data-stu-id="50cb7-140">This is a required property.</span></span>|
|<span data-ttu-id="50cb7-141">bloqueou</span><span class="sxs-lookup"><span data-stu-id="50cb7-141">blocked</span></span>             |<span data-ttu-id="50cb7-142">booliano</span><span class="sxs-lookup"><span data-stu-id="50cb7-142">boolean</span></span> |<span data-ttu-id="50cb7-143">Especifica que as transações com o item não podem ser lançadas, por exemplo, porque o item está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="50cb7-143">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="50cb7-144">Defina como **true**se o item estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="50cb7-144">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="50cb7-145">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="50cb7-145">baseUnitOfMeasureId</span></span> |<span data-ttu-id="50cb7-146">GUID</span><span class="sxs-lookup"><span data-stu-id="50cb7-146">GUID</span></span>    |<span data-ttu-id="50cb7-147">Especifica a ID da unidade de medida.</span><span class="sxs-lookup"><span data-stu-id="50cb7-147">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="50cb7-148">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="50cb7-148">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="50cb7-149">Extra. UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="50cb7-149">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="50cb7-150">Especifica a unidade na qual o item é mantido no estoque.</span><span class="sxs-lookup"><span data-stu-id="50cb7-150">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="50cb7-151">GTIN</span><span class="sxs-lookup"><span data-stu-id="50cb7-151">gtin</span></span>                |<span data-ttu-id="50cb7-152">numéricos</span><span class="sxs-lookup"><span data-stu-id="50cb7-152">numeric</span></span> |<span data-ttu-id="50cb7-153">Este é o número do item comercial global.</span><span class="sxs-lookup"><span data-stu-id="50cb7-153">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="50cb7-154">objectcategoryid</span><span class="sxs-lookup"><span data-stu-id="50cb7-154">itemCategoryId</span></span>      |<span data-ttu-id="50cb7-155">GUID</span><span class="sxs-lookup"><span data-stu-id="50cb7-155">GUID</span></span> |<span data-ttu-id="50cb7-156">Especifica a categoria à qual o item pertence.</span><span class="sxs-lookup"><span data-stu-id="50cb7-156">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="50cb7-157">As categorias de item também contêm qualquer atributo de item atribuído.</span><span class="sxs-lookup"><span data-stu-id="50cb7-157">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="50cb7-158">inventory</span><span class="sxs-lookup"><span data-stu-id="50cb7-158">inventory</span></span>           |<span data-ttu-id="50cb7-159">dígitos</span><span class="sxs-lookup"><span data-stu-id="50cb7-159">decimal</span></span> |<span data-ttu-id="50cb7-160">Especifica quantas unidades, como peças, caixas ou latas do item estão no estoque.</span><span class="sxs-lookup"><span data-stu-id="50cb7-160">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="50cb7-161">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="50cb7-161">Read-Only.</span></span>|
|<span data-ttu-id="50cb7-162">PreçoUnitário</span><span class="sxs-lookup"><span data-stu-id="50cb7-162">unitPrice</span></span>           |<span data-ttu-id="50cb7-163">dígitos</span><span class="sxs-lookup"><span data-stu-id="50cb7-163">decimal</span></span> |<span data-ttu-id="50cb7-164">Especifica o preço de uma unidade do item na moeda especificada.</span><span class="sxs-lookup"><span data-stu-id="50cb7-164">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="50cb7-165">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="50cb7-165">priceIncludesTax</span></span>    |<span data-ttu-id="50cb7-166">booliano</span><span class="sxs-lookup"><span data-stu-id="50cb7-166">boolean</span></span> |<span data-ttu-id="50cb7-167">Especifica que o PreçoUnitário inclui o imposto.</span><span class="sxs-lookup"><span data-stu-id="50cb7-167">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="50cb7-168">Defina como **true**, se PreçoUnitário incluir imposto.</span><span class="sxs-lookup"><span data-stu-id="50cb7-168">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="50cb7-169">unitCost</span><span class="sxs-lookup"><span data-stu-id="50cb7-169">unitCost</span></span>            |<span data-ttu-id="50cb7-170">dígitos</span><span class="sxs-lookup"><span data-stu-id="50cb7-170">decimal</span></span> |<span data-ttu-id="50cb7-171">Especifica o custo por unidade do item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-171">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="50cb7-172">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="50cb7-172">taxGroupId</span></span>          |<span data-ttu-id="50cb7-173">GUID</span><span class="sxs-lookup"><span data-stu-id="50cb7-173">GUID</span></span>    |<span data-ttu-id="50cb7-174">Especifica a ID do grupo de impostos para o item.</span><span class="sxs-lookup"><span data-stu-id="50cb7-174">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="50cb7-175">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="50cb7-175">taxGroupCode</span></span>        |<span data-ttu-id="50cb7-176">numéricos</span><span class="sxs-lookup"><span data-stu-id="50cb7-176">numeric</span></span> |<span data-ttu-id="50cb7-177">Um grupo de impostos representa um grupo de itens ou recursos de estoque sujeitos a termos de impostos idênticos.</span><span class="sxs-lookup"><span data-stu-id="50cb7-177">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="50cb7-178">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50cb7-178">lastModifiedDateTime</span></span>|<span data-ttu-id="50cb7-179">datetime</span><span class="sxs-lookup"><span data-stu-id="50cb7-179">datetime</span></span>|<span data-ttu-id="50cb7-180">A última data/hora em que o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="50cb7-180">The last datetime the item was modified.</span></span> <span data-ttu-id="50cb7-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="50cb7-181">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="50cb7-182">Relações</span><span class="sxs-lookup"><span data-stu-id="50cb7-182">Relationships</span></span>
<span data-ttu-id="50cb7-183">Um grupo de impostos (taxGroupCode) deve existir na tabela de grupos de impostos.</span><span class="sxs-lookup"><span data-stu-id="50cb7-183">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="50cb7-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50cb7-184">JSON representation</span></span>

<span data-ttu-id="50cb7-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50cb7-185">Here is a JSON representation of the resource.</span></span>


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


