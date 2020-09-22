---
title: tipo de recurso itens
description: Um objeto de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 89ccee3123fc3f0fc04b620e5b3528f4a253d1fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058446"
---
# <a name="items-resource-type"></a><span data-ttu-id="b899e-103">tipo de recurso itens</span><span class="sxs-lookup"><span data-stu-id="b899e-103">items resource type</span></span>

<span data-ttu-id="b899e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b899e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b899e-105">Representa um item no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b899e-105">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b899e-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b899e-106">Methods</span></span>

| <span data-ttu-id="b899e-107">Método</span><span class="sxs-lookup"><span data-stu-id="b899e-107">Method</span></span>                                      |<span data-ttu-id="b899e-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b899e-108">Return Type</span></span>|<span data-ttu-id="b899e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b899e-109">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="b899e-110">Obter itens</span><span class="sxs-lookup"><span data-stu-id="b899e-110">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="b899e-111">items</span><span class="sxs-lookup"><span data-stu-id="b899e-111">items</span></span>     |<span data-ttu-id="b899e-112">Obtém um objeto item.</span><span class="sxs-lookup"><span data-stu-id="b899e-112">Gets an item object.</span></span>   |
|[<span data-ttu-id="b899e-113">Itens post</span><span class="sxs-lookup"><span data-stu-id="b899e-113">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="b899e-114">items</span><span class="sxs-lookup"><span data-stu-id="b899e-114">items</span></span>     |<span data-ttu-id="b899e-115">Cria um objeto item.</span><span class="sxs-lookup"><span data-stu-id="b899e-115">Creates an item object.</span></span>|
|[<span data-ttu-id="b899e-116">Item de patch</span><span class="sxs-lookup"><span data-stu-id="b899e-116">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="b899e-117">items</span><span class="sxs-lookup"><span data-stu-id="b899e-117">items</span></span>     |<span data-ttu-id="b899e-118">Atualiza um objeto item.</span><span class="sxs-lookup"><span data-stu-id="b899e-118">Updates an item object.</span></span>|
|[<span data-ttu-id="b899e-119">Excluir itens</span><span class="sxs-lookup"><span data-stu-id="b899e-119">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="b899e-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b899e-120">none</span></span>      |<span data-ttu-id="b899e-121">Exclui um objeto item.</span><span class="sxs-lookup"><span data-stu-id="b899e-121">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b899e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b899e-122">Properties</span></span>
| <span data-ttu-id="b899e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b899e-123">Property</span></span>           | <span data-ttu-id="b899e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b899e-124">Type</span></span> |<span data-ttu-id="b899e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b899e-125">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="b899e-126">id</span><span class="sxs-lookup"><span data-stu-id="b899e-126">id</span></span>                  |<span data-ttu-id="b899e-127">GUID</span><span class="sxs-lookup"><span data-stu-id="b899e-127">GUID</span></span>    |<span data-ttu-id="b899e-128">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="b899e-128">The unique ID of the item.</span></span> <span data-ttu-id="b899e-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="b899e-129">Non-editable.</span></span>             |
|<span data-ttu-id="b899e-130">number</span><span class="sxs-lookup"><span data-stu-id="b899e-130">number</span></span>              |<span data-ttu-id="b899e-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b899e-131">string</span></span>  |<span data-ttu-id="b899e-132">O número do item.</span><span class="sxs-lookup"><span data-stu-id="b899e-132">The item number.</span></span>                                     |
|<span data-ttu-id="b899e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b899e-133">displayName</span></span>         |<span data-ttu-id="b899e-134">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b899e-134">string</span></span>  |<span data-ttu-id="b899e-135">Especifica uma descrição do item.</span><span class="sxs-lookup"><span data-stu-id="b899e-135">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="b899e-136">tipo</span><span class="sxs-lookup"><span data-stu-id="b899e-136">type</span></span>                |<span data-ttu-id="b899e-137">numéricos</span><span class="sxs-lookup"><span data-stu-id="b899e-137">numeric</span></span> |<span data-ttu-id="b899e-138">O tipo de inventário para o item.</span><span class="sxs-lookup"><span data-stu-id="b899e-138">The inventory type for the item.</span></span> <span data-ttu-id="b899e-139">1 = item de estoque, 2 = item de serviço.</span><span class="sxs-lookup"><span data-stu-id="b899e-139">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="b899e-140">Essa é uma propriedade obrigatória.</span><span class="sxs-lookup"><span data-stu-id="b899e-140">This is a required property.</span></span>|
|<span data-ttu-id="b899e-141">bloqueou</span><span class="sxs-lookup"><span data-stu-id="b899e-141">blocked</span></span>             |<span data-ttu-id="b899e-142">booliano</span><span class="sxs-lookup"><span data-stu-id="b899e-142">boolean</span></span> |<span data-ttu-id="b899e-143">Especifica que as transações com o item não podem ser lançadas, por exemplo, porque o item está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="b899e-143">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="b899e-144">Defina como **true**se o item estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="b899e-144">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="b899e-145">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="b899e-145">baseUnitOfMeasureId</span></span> |<span data-ttu-id="b899e-146">GUID</span><span class="sxs-lookup"><span data-stu-id="b899e-146">GUID</span></span>    |<span data-ttu-id="b899e-147">Especifica a ID da unidade de medida.</span><span class="sxs-lookup"><span data-stu-id="b899e-147">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="b899e-148">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="b899e-148">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="b899e-149">Extra. UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="b899e-149">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="b899e-150">Especifica a unidade na qual o item é mantido no estoque.</span><span class="sxs-lookup"><span data-stu-id="b899e-150">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="b899e-151">GTIN</span><span class="sxs-lookup"><span data-stu-id="b899e-151">gtin</span></span>                |<span data-ttu-id="b899e-152">numéricos</span><span class="sxs-lookup"><span data-stu-id="b899e-152">numeric</span></span> |<span data-ttu-id="b899e-153">Este é o número do item comercial global.</span><span class="sxs-lookup"><span data-stu-id="b899e-153">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="b899e-154">objectcategoryid</span><span class="sxs-lookup"><span data-stu-id="b899e-154">itemCategoryId</span></span>      |<span data-ttu-id="b899e-155">GUID</span><span class="sxs-lookup"><span data-stu-id="b899e-155">GUID</span></span> |<span data-ttu-id="b899e-156">Especifica a categoria à qual o item pertence.</span><span class="sxs-lookup"><span data-stu-id="b899e-156">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="b899e-157">As categorias de item também contêm qualquer atributo de item atribuído.</span><span class="sxs-lookup"><span data-stu-id="b899e-157">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="b899e-158">inventory</span><span class="sxs-lookup"><span data-stu-id="b899e-158">inventory</span></span>           |<span data-ttu-id="b899e-159">dígitos</span><span class="sxs-lookup"><span data-stu-id="b899e-159">decimal</span></span> |<span data-ttu-id="b899e-160">Especifica quantas unidades, como peças, caixas ou latas do item estão no estoque.</span><span class="sxs-lookup"><span data-stu-id="b899e-160">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="b899e-161">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b899e-161">Read-Only.</span></span>|
|<span data-ttu-id="b899e-162">PreçoUnitário</span><span class="sxs-lookup"><span data-stu-id="b899e-162">unitPrice</span></span>           |<span data-ttu-id="b899e-163">dígitos</span><span class="sxs-lookup"><span data-stu-id="b899e-163">decimal</span></span> |<span data-ttu-id="b899e-164">Especifica o preço de uma unidade do item na moeda especificada.</span><span class="sxs-lookup"><span data-stu-id="b899e-164">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="b899e-165">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="b899e-165">priceIncludesTax</span></span>    |<span data-ttu-id="b899e-166">booliano</span><span class="sxs-lookup"><span data-stu-id="b899e-166">boolean</span></span> |<span data-ttu-id="b899e-167">Especifica que o PreçoUnitário inclui o imposto.</span><span class="sxs-lookup"><span data-stu-id="b899e-167">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="b899e-168">Defina como **true**, se PreçoUnitário incluir imposto.</span><span class="sxs-lookup"><span data-stu-id="b899e-168">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="b899e-169">unitCost</span><span class="sxs-lookup"><span data-stu-id="b899e-169">unitCost</span></span>            |<span data-ttu-id="b899e-170">dígitos</span><span class="sxs-lookup"><span data-stu-id="b899e-170">decimal</span></span> |<span data-ttu-id="b899e-171">Especifica o custo por unidade do item.</span><span class="sxs-lookup"><span data-stu-id="b899e-171">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="b899e-172">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="b899e-172">taxGroupId</span></span>          |<span data-ttu-id="b899e-173">GUID</span><span class="sxs-lookup"><span data-stu-id="b899e-173">GUID</span></span>    |<span data-ttu-id="b899e-174">Especifica a ID do grupo de impostos para o item.</span><span class="sxs-lookup"><span data-stu-id="b899e-174">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="b899e-175">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="b899e-175">taxGroupCode</span></span>        |<span data-ttu-id="b899e-176">numéricos</span><span class="sxs-lookup"><span data-stu-id="b899e-176">numeric</span></span> |<span data-ttu-id="b899e-177">Um grupo de impostos representa um grupo de itens ou recursos de estoque sujeitos a termos de impostos idênticos.</span><span class="sxs-lookup"><span data-stu-id="b899e-177">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="b899e-178">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b899e-178">lastModifiedDateTime</span></span>|<span data-ttu-id="b899e-179">datetime</span><span class="sxs-lookup"><span data-stu-id="b899e-179">datetime</span></span>|<span data-ttu-id="b899e-180">A última data/hora em que o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="b899e-180">The last datetime the item was modified.</span></span> <span data-ttu-id="b899e-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b899e-181">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="b899e-182">Relações</span><span class="sxs-lookup"><span data-stu-id="b899e-182">Relationships</span></span>
<span data-ttu-id="b899e-183">Um grupo de impostos (taxGroupCode) deve existir na tabela de grupos de impostos.</span><span class="sxs-lookup"><span data-stu-id="b899e-183">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b899e-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b899e-184">JSON representation</span></span>

<span data-ttu-id="b899e-185">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b899e-185">Here is a JSON representation of the resource.</span></span>


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




