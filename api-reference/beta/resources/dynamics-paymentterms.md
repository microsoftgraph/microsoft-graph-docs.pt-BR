---
title: tipo de recurso paymentTerms
description: Um objeto de condições de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 1e9e7951da79d524002f004410ef6939d7be5b99
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027075"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="0626b-103">tipo de recurso paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0626b-103">paymentTerms resource type</span></span>

<span data-ttu-id="0626b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0626b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0626b-105">Representa um termo de pagamento no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="0626b-105">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="0626b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0626b-106">Methods</span></span>

| <span data-ttu-id="0626b-107">Método</span><span class="sxs-lookup"><span data-stu-id="0626b-107">Method</span></span>                                                      | <span data-ttu-id="0626b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0626b-108">Return Type</span></span>|<span data-ttu-id="0626b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0626b-109">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="0626b-110">Obter paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0626b-110">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="0626b-111">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0626b-111">paymentTerms</span></span>|<span data-ttu-id="0626b-112">Obter um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="0626b-112">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="0626b-113">Postar paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0626b-113">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="0626b-114">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0626b-114">paymentTerms</span></span>|<span data-ttu-id="0626b-115">Criar um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="0626b-115">Create a payment terms object.</span></span>|
|[<span data-ttu-id="0626b-116">Patch paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0626b-116">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="0626b-117">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0626b-117">paymentTerms</span></span>|<span data-ttu-id="0626b-118">Atualizar um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="0626b-118">Update a payment terms object.</span></span>|
|[<span data-ttu-id="0626b-119">Excluir paymentTerms</span><span class="sxs-lookup"><span data-stu-id="0626b-119">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="0626b-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0626b-120">none</span></span>        |<span data-ttu-id="0626b-121">Excluir um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="0626b-121">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0626b-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0626b-122">Properties</span></span>
| <span data-ttu-id="0626b-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0626b-123">Property</span></span>                     | <span data-ttu-id="0626b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0626b-124">Type</span></span>     |<span data-ttu-id="0626b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0626b-125">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="0626b-126">id</span><span class="sxs-lookup"><span data-stu-id="0626b-126">id</span></span>                            |<span data-ttu-id="0626b-127">GUID</span><span class="sxs-lookup"><span data-stu-id="0626b-127">GUID</span></span>    |<span data-ttu-id="0626b-128">A ID exclusiva do paymentTerms.</span><span class="sxs-lookup"><span data-stu-id="0626b-128">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="0626b-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="0626b-129">Non-editable.</span></span>           |
|<span data-ttu-id="0626b-130">código</span><span class="sxs-lookup"><span data-stu-id="0626b-130">code</span></span>                          |<span data-ttu-id="0626b-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0626b-131">string</span></span>  |<span data-ttu-id="0626b-132">Especifica o código da expressão de pagamento.</span><span class="sxs-lookup"><span data-stu-id="0626b-132">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="0626b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0626b-133">displayName</span></span>                   |<span data-ttu-id="0626b-134">string</span><span class="sxs-lookup"><span data-stu-id="0626b-134">string</span></span>  |<span data-ttu-id="0626b-135">Especifica o nome de exibição do termo de pagamento.</span><span class="sxs-lookup"><span data-stu-id="0626b-135">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="0626b-136">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="0626b-136">dueDateCalculation</span></span>            |<span data-ttu-id="0626b-137">string</span><span class="sxs-lookup"><span data-stu-id="0626b-137">string</span></span>  |<span data-ttu-id="0626b-138">Especifica a fórmula usada para calcular a data em que um pagamento deve ser feito.</span><span class="sxs-lookup"><span data-stu-id="0626b-138">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="0626b-139">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="0626b-139">discountDateCalculation</span></span>       |<span data-ttu-id="0626b-140">string</span><span class="sxs-lookup"><span data-stu-id="0626b-140">string</span></span>  |<span data-ttu-id="0626b-141">Especifica a fórmula usada para calcular a data em que um pagamento deve ser feito para obter um desconto.</span><span class="sxs-lookup"><span data-stu-id="0626b-141">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="0626b-142">discountPercent</span><span class="sxs-lookup"><span data-stu-id="0626b-142">discountPercent</span></span>               |<span data-ttu-id="0626b-143">dígitos</span><span class="sxs-lookup"><span data-stu-id="0626b-143">decimal</span></span> |<span data-ttu-id="0626b-144">Especifica a porcentagem de desconto aplicada ao pagamento antecipado de um valor de fatura.</span><span class="sxs-lookup"><span data-stu-id="0626b-144">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="0626b-145">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="0626b-145">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="0626b-146">booliano</span><span class="sxs-lookup"><span data-stu-id="0626b-146">boolean</span></span> |<span data-ttu-id="0626b-147">Especifica se o desconto deve ser aplicado a memorandos de crédito.</span><span class="sxs-lookup"><span data-stu-id="0626b-147">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="0626b-148">**True** indica que um desconto será fornecido, **false** indica que um desconto não será fornecido.</span><span class="sxs-lookup"><span data-stu-id="0626b-148">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="0626b-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0626b-149">lastModifiedDateTime</span></span>          |<span data-ttu-id="0626b-150">datetime</span><span class="sxs-lookup"><span data-stu-id="0626b-150">datetime</span></span>|<span data-ttu-id="0626b-151">O último DateTime que o paymentTerms foi modificado.</span><span class="sxs-lookup"><span data-stu-id="0626b-151">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="0626b-152">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0626b-152">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="0626b-153">Relações</span><span class="sxs-lookup"><span data-stu-id="0626b-153">Relationships</span></span>
<span data-ttu-id="0626b-154">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0626b-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0626b-155">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0626b-155">JSON representation</span></span>

<span data-ttu-id="0626b-156">Veja a seguir uma representação JSON do paymentTerms.</span><span class="sxs-lookup"><span data-stu-id="0626b-156">Here is a JSON representation of the paymentTerms.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "dueDateCalculation": "string",
  "discountDateCalculation": "string",
  "discountPercent": "decimal",
  "calculateDiscountOnCreditMemos": "boolean",
  "lastModifiedDateTime": "datetime"
}

```


