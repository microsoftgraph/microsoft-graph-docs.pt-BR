---
title: tipo de recurso itens
description: Um objeto de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 42ec7720e2e858f319beab8576fbe57542dd470c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507305"
---
# <a name="items-resource-type"></a><span data-ttu-id="f58d6-103">tipo de recurso itens</span><span class="sxs-lookup"><span data-stu-id="f58d6-103">items resource type</span></span>
<span data-ttu-id="f58d6-104">Representa um item no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="f58d6-104">Represents an item in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f58d6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f58d6-105">Methods</span></span>

| <span data-ttu-id="f58d6-106">Método</span><span class="sxs-lookup"><span data-stu-id="f58d6-106">Method</span></span>                                      |<span data-ttu-id="f58d6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f58d6-107">Return Type</span></span>|<span data-ttu-id="f58d6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f58d6-108">Description</span></span> |
|:--------------------------------------------|:----------|:-----------|
|[<span data-ttu-id="f58d6-109">Obter itens</span><span class="sxs-lookup"><span data-stu-id="f58d6-109">Get items</span></span>](../api/dynamics-item-get.md)      |<span data-ttu-id="f58d6-110">items</span><span class="sxs-lookup"><span data-stu-id="f58d6-110">items</span></span>     |<span data-ttu-id="f58d6-111">Obtém um objeto item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-111">Gets an item object.</span></span>   |
|[<span data-ttu-id="f58d6-112">Itens post</span><span class="sxs-lookup"><span data-stu-id="f58d6-112">Post items</span></span>](../api/dynamics-create-item.md)  |<span data-ttu-id="f58d6-113">items</span><span class="sxs-lookup"><span data-stu-id="f58d6-113">items</span></span>     |<span data-ttu-id="f58d6-114">Cria um objeto item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-114">Creates an item object.</span></span>|
|[<span data-ttu-id="f58d6-115">Item de patch</span><span class="sxs-lookup"><span data-stu-id="f58d6-115">Patch item</span></span>](../api/dynamics-item-update.md)  |<span data-ttu-id="f58d6-116">items</span><span class="sxs-lookup"><span data-stu-id="f58d6-116">items</span></span>     |<span data-ttu-id="f58d6-117">Atualiza um objeto item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-117">Updates an item object.</span></span>|
|[<span data-ttu-id="f58d6-118">Excluir itens</span><span class="sxs-lookup"><span data-stu-id="f58d6-118">Delete items</span></span>](../api/dynamics-item-delete.md)|<span data-ttu-id="f58d6-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f58d6-119">none</span></span>      |<span data-ttu-id="f58d6-120">Exclui um objeto item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-120">Deletes an item object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f58d6-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f58d6-121">Properties</span></span>
| <span data-ttu-id="f58d6-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f58d6-122">Property</span></span>           | <span data-ttu-id="f58d6-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f58d6-123">Type</span></span> |<span data-ttu-id="f58d6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f58d6-124">Description</span></span>                                          |
|:-------------------|:-------|:----------------------------------------------------|
|<span data-ttu-id="f58d6-125">id</span><span class="sxs-lookup"><span data-stu-id="f58d6-125">id</span></span>                  |<span data-ttu-id="f58d6-126">GUID</span><span class="sxs-lookup"><span data-stu-id="f58d6-126">GUID</span></span>    |<span data-ttu-id="f58d6-127">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-127">The unique ID of the item.</span></span> <span data-ttu-id="f58d6-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="f58d6-128">Non-editable.</span></span>             |
|<span data-ttu-id="f58d6-129">number</span><span class="sxs-lookup"><span data-stu-id="f58d6-129">number</span></span>              |<span data-ttu-id="f58d6-130">string</span><span class="sxs-lookup"><span data-stu-id="f58d6-130">string</span></span>  |<span data-ttu-id="f58d6-131">O número do item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-131">The item number.</span></span>                                     |
|<span data-ttu-id="f58d6-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f58d6-132">displayName</span></span>         |<span data-ttu-id="f58d6-133">string</span><span class="sxs-lookup"><span data-stu-id="f58d6-133">string</span></span>  |<span data-ttu-id="f58d6-134">Especifica uma descrição do item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-134">Specifies a description of the item.</span></span>                 |
|<span data-ttu-id="f58d6-135">type</span><span class="sxs-lookup"><span data-stu-id="f58d6-135">type</span></span>                |<span data-ttu-id="f58d6-136">numéricos</span><span class="sxs-lookup"><span data-stu-id="f58d6-136">numeric</span></span> |<span data-ttu-id="f58d6-137">O tipo de inventário para o item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-137">The inventory type for the item.</span></span> <span data-ttu-id="f58d6-138">1 = item de estoque, 2 = item de serviço.</span><span class="sxs-lookup"><span data-stu-id="f58d6-138">1 = inventory item, 2 = service item.</span></span> <span data-ttu-id="f58d6-139">Essa é uma propriedade obrigatória.</span><span class="sxs-lookup"><span data-stu-id="f58d6-139">This is a required property.</span></span>|
|<span data-ttu-id="f58d6-140">bloqueou</span><span class="sxs-lookup"><span data-stu-id="f58d6-140">blocked</span></span>             |<span data-ttu-id="f58d6-141">booliano</span><span class="sxs-lookup"><span data-stu-id="f58d6-141">boolean</span></span> |<span data-ttu-id="f58d6-142">Especifica que as transações com o item não podem ser lançadas, por exemplo, porque o item está em quarentena.</span><span class="sxs-lookup"><span data-stu-id="f58d6-142">Specifies that transactions with the item cannot be posted, for example, because the item is in quarantine.</span></span> <span data-ttu-id="f58d6-143">Defina como **true**se o item estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f58d6-143">Set to **true**, if item is blocked.</span></span>|
|<span data-ttu-id="f58d6-144">baseUnitOfMeasureId</span><span class="sxs-lookup"><span data-stu-id="f58d6-144">baseUnitOfMeasureId</span></span> |<span data-ttu-id="f58d6-145">GUID</span><span class="sxs-lookup"><span data-stu-id="f58d6-145">GUID</span></span>    |<span data-ttu-id="f58d6-146">Especifica a ID da unidade de medida.</span><span class="sxs-lookup"><span data-stu-id="f58d6-146">Specifies the ID of the unit of measure.</span></span>             |
|<span data-ttu-id="f58d6-147">baseUnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="f58d6-147">baseUnitOfMeasure</span></span>   |[<span data-ttu-id="f58d6-148">Extra. UnitOfMeasure</span><span class="sxs-lookup"><span data-stu-id="f58d6-148">NAV.UnitOfMeasure</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="f58d6-149">Especifica a unidade na qual o item é mantido no estoque.</span><span class="sxs-lookup"><span data-stu-id="f58d6-149">Specifies the unit in which the item is held in inventory.</span></span>|
|<span data-ttu-id="f58d6-150">GTIN</span><span class="sxs-lookup"><span data-stu-id="f58d6-150">gtin</span></span>                |<span data-ttu-id="f58d6-151">numéricos</span><span class="sxs-lookup"><span data-stu-id="f58d6-151">numeric</span></span> |<span data-ttu-id="f58d6-152">Este é o número do item comercial global.</span><span class="sxs-lookup"><span data-stu-id="f58d6-152">This is the Global Trade Item Number.</span></span>                |
|<span data-ttu-id="f58d6-153">objectCategoryid</span><span class="sxs-lookup"><span data-stu-id="f58d6-153">itemCategoryId</span></span>      |<span data-ttu-id="f58d6-154">GUID</span><span class="sxs-lookup"><span data-stu-id="f58d6-154">GUID</span></span> |<span data-ttu-id="f58d6-155">Especifica a categoria à qual o item pertence.</span><span class="sxs-lookup"><span data-stu-id="f58d6-155">Specifies the category that the item belongs to.</span></span> <span data-ttu-id="f58d6-156">As categorias de item também contêm qualquer atributo de item atribuído.</span><span class="sxs-lookup"><span data-stu-id="f58d6-156">Item categories also contain any assigned item attributes.</span></span>|
|<span data-ttu-id="f58d6-157">inventory</span><span class="sxs-lookup"><span data-stu-id="f58d6-157">inventory</span></span>           |<span data-ttu-id="f58d6-158">dígitos</span><span class="sxs-lookup"><span data-stu-id="f58d6-158">decimal</span></span> |<span data-ttu-id="f58d6-159">Especifica quantas unidades, como peças, caixas ou latas do item estão no estoque.</span><span class="sxs-lookup"><span data-stu-id="f58d6-159">Specifies how many units, such as pieces, boxes, or cans, of the item are in inventory.</span></span> <span data-ttu-id="f58d6-160">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="f58d6-160">Read-Only.</span></span>|
|<span data-ttu-id="f58d6-161">PreçoUnitário</span><span class="sxs-lookup"><span data-stu-id="f58d6-161">unitPrice</span></span>           |<span data-ttu-id="f58d6-162">dígitos</span><span class="sxs-lookup"><span data-stu-id="f58d6-162">decimal</span></span> |<span data-ttu-id="f58d6-163">Especifica o preço de uma unidade do item na moeda especificada.</span><span class="sxs-lookup"><span data-stu-id="f58d6-163">Specifies the price for one unit of the item in the specified currency.</span></span>|
|<span data-ttu-id="f58d6-164">priceIncludesTax</span><span class="sxs-lookup"><span data-stu-id="f58d6-164">priceIncludesTax</span></span>    |<span data-ttu-id="f58d6-165">booliano</span><span class="sxs-lookup"><span data-stu-id="f58d6-165">boolean</span></span> |<span data-ttu-id="f58d6-166">Especifica que o PreçoUnitário inclui o imposto.</span><span class="sxs-lookup"><span data-stu-id="f58d6-166">Specifies that the unitPrice includes tax.</span></span> <span data-ttu-id="f58d6-167">Defina como **true**, se PreçoUnitário incluir imposto.</span><span class="sxs-lookup"><span data-stu-id="f58d6-167">Set to **true**, if unitPrice includes tax.</span></span>|
|<span data-ttu-id="f58d6-168">unitCost</span><span class="sxs-lookup"><span data-stu-id="f58d6-168">unitCost</span></span>            |<span data-ttu-id="f58d6-169">dígitos</span><span class="sxs-lookup"><span data-stu-id="f58d6-169">decimal</span></span> |<span data-ttu-id="f58d6-170">Especifica o custo por unidade do item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-170">Specifies the cost per unit of the item.</span></span>             |
|<span data-ttu-id="f58d6-171">taxGroupId</span><span class="sxs-lookup"><span data-stu-id="f58d6-171">taxGroupId</span></span>          |<span data-ttu-id="f58d6-172">GUID</span><span class="sxs-lookup"><span data-stu-id="f58d6-172">GUID</span></span>    |<span data-ttu-id="f58d6-173">Especifica a ID do grupo de impostos para o item.</span><span class="sxs-lookup"><span data-stu-id="f58d6-173">Specifies the ID of the Tax Group for the item.</span></span>      |
|<span data-ttu-id="f58d6-174">taxGroupCode</span><span class="sxs-lookup"><span data-stu-id="f58d6-174">taxGroupCode</span></span>        |<span data-ttu-id="f58d6-175">numéricos</span><span class="sxs-lookup"><span data-stu-id="f58d6-175">numeric</span></span> |<span data-ttu-id="f58d6-176">Um grupo de impostos representa um grupo de itens ou recursos de estoque sujeitos a termos de impostos idênticos.</span><span class="sxs-lookup"><span data-stu-id="f58d6-176">A Tax Group represents a group of inventory items or resources that are subject to identical tax terms.</span></span>|
|<span data-ttu-id="f58d6-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f58d6-177">lastModifiedDateTime</span></span>|<span data-ttu-id="f58d6-178">DateTime</span><span class="sxs-lookup"><span data-stu-id="f58d6-178">datetime</span></span>|<span data-ttu-id="f58d6-179">A última data/hora em que o item foi modificado.</span><span class="sxs-lookup"><span data-stu-id="f58d6-179">The last datetime the item was modified.</span></span> <span data-ttu-id="f58d6-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f58d6-180">Read-Only.</span></span>  |  


## <a name="relationships"></a><span data-ttu-id="f58d6-181">Relações</span><span class="sxs-lookup"><span data-stu-id="f58d6-181">Relationships</span></span>
<span data-ttu-id="f58d6-182">Um grupo de impostos (taxGroupCode) deve existir na tabela de grupos de impostos.</span><span class="sxs-lookup"><span data-stu-id="f58d6-182">A Tax Group(taxGroupCode) must exist in the Tax Group table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f58d6-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f58d6-183">JSON representation</span></span>

<span data-ttu-id="f58d6-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f58d6-184">Here is a JSON representation of the resource.</span></span>


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


