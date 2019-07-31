---
title: tipo de recurso paymentTerms
description: Um objeto de condições de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d367314d5546c59dd251b30e952aa17b9d60ce10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006588"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="fc552-103">tipo de recurso paymentTerms</span><span class="sxs-lookup"><span data-stu-id="fc552-103">paymentTerms resource type</span></span>
<span data-ttu-id="fc552-104">Representa um termo de pagamento no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="fc552-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="fc552-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fc552-105">Methods</span></span>

| <span data-ttu-id="fc552-106">Método</span><span class="sxs-lookup"><span data-stu-id="fc552-106">Method</span></span>                                                      | <span data-ttu-id="fc552-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fc552-107">Return Type</span></span>|<span data-ttu-id="fc552-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc552-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="fc552-109">Obter paymentTerms</span><span class="sxs-lookup"><span data-stu-id="fc552-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="fc552-110">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="fc552-110">paymentTerms</span></span>|<span data-ttu-id="fc552-111">Obter um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="fc552-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="fc552-112">Postar paymentTerms</span><span class="sxs-lookup"><span data-stu-id="fc552-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="fc552-113">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="fc552-113">paymentTerms</span></span>|<span data-ttu-id="fc552-114">Criar um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="fc552-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="fc552-115">Patch paymentTerms</span><span class="sxs-lookup"><span data-stu-id="fc552-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="fc552-116">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="fc552-116">paymentTerms</span></span>|<span data-ttu-id="fc552-117">Atualizar um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="fc552-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="fc552-118">Excluir paymentTerms</span><span class="sxs-lookup"><span data-stu-id="fc552-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="fc552-119">none</span><span class="sxs-lookup"><span data-stu-id="fc552-119">none</span></span>        |<span data-ttu-id="fc552-120">Excluir um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="fc552-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc552-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc552-121">Properties</span></span>
| <span data-ttu-id="fc552-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc552-122">Property</span></span>                     | <span data-ttu-id="fc552-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc552-123">Type</span></span>     |<span data-ttu-id="fc552-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc552-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="fc552-125">id</span><span class="sxs-lookup"><span data-stu-id="fc552-125">id</span></span>                            |<span data-ttu-id="fc552-126">GUID</span><span class="sxs-lookup"><span data-stu-id="fc552-126">GUID</span></span>    |<span data-ttu-id="fc552-127">A ID exclusiva do paymentTerms.</span><span class="sxs-lookup"><span data-stu-id="fc552-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="fc552-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="fc552-128">Non-editable.</span></span>           |
|<span data-ttu-id="fc552-129">código</span><span class="sxs-lookup"><span data-stu-id="fc552-129">code</span></span>                          |<span data-ttu-id="fc552-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc552-130">string</span></span>  |<span data-ttu-id="fc552-131">Especifica o código da expressão de pagamento.</span><span class="sxs-lookup"><span data-stu-id="fc552-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="fc552-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fc552-132">displayName</span></span>                   |<span data-ttu-id="fc552-133">string</span><span class="sxs-lookup"><span data-stu-id="fc552-133">string</span></span>  |<span data-ttu-id="fc552-134">Especifica o nome de exibição do termo de pagamento.</span><span class="sxs-lookup"><span data-stu-id="fc552-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="fc552-135">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="fc552-135">dueDateCalculation</span></span>            |<span data-ttu-id="fc552-136">string</span><span class="sxs-lookup"><span data-stu-id="fc552-136">string</span></span>  |<span data-ttu-id="fc552-137">Especifica a fórmula usada para calcular a data em que um pagamento deve ser feito.</span><span class="sxs-lookup"><span data-stu-id="fc552-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="fc552-138">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="fc552-138">discountDateCalculation</span></span>       |<span data-ttu-id="fc552-139">string</span><span class="sxs-lookup"><span data-stu-id="fc552-139">string</span></span>  |<span data-ttu-id="fc552-140">Especifica a fórmula usada para calcular a data em que um pagamento deve ser feito para obter um desconto.</span><span class="sxs-lookup"><span data-stu-id="fc552-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="fc552-141">discountPercent</span><span class="sxs-lookup"><span data-stu-id="fc552-141">discountPercent</span></span>               |<span data-ttu-id="fc552-142">dígitos</span><span class="sxs-lookup"><span data-stu-id="fc552-142">decimal</span></span> |<span data-ttu-id="fc552-143">Especifica a porcentagem de desconto aplicada ao pagamento antecipado de um valor de fatura.</span><span class="sxs-lookup"><span data-stu-id="fc552-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="fc552-144">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="fc552-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="fc552-145">booliano</span><span class="sxs-lookup"><span data-stu-id="fc552-145">boolean</span></span> |<span data-ttu-id="fc552-146">Especifica se o desconto deve ser aplicado a memorandos de crédito.</span><span class="sxs-lookup"><span data-stu-id="fc552-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="fc552-147">**True** indica que um desconto será fornecido, **false** indica que um desconto não será fornecido.</span><span class="sxs-lookup"><span data-stu-id="fc552-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="fc552-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc552-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="fc552-149">DateTime</span><span class="sxs-lookup"><span data-stu-id="fc552-149">datetime</span></span>|<span data-ttu-id="fc552-150">O último DateTime que o paymentTerms foi modificado.</span><span class="sxs-lookup"><span data-stu-id="fc552-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="fc552-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fc552-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="fc552-152">Relações</span><span class="sxs-lookup"><span data-stu-id="fc552-152">Relationships</span></span>
<span data-ttu-id="fc552-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc552-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc552-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc552-154">JSON representation</span></span>

<span data-ttu-id="fc552-155">Veja a seguir uma representação JSON do paymentTerms.</span><span class="sxs-lookup"><span data-stu-id="fc552-155">Here is a JSON representation of the paymentTerms.</span></span>


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
