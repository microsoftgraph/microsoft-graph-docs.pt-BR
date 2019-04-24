---
title: tipo de recurso paymentTerms
description: Um objeto de condições de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4ed1f3791474cf6e29038e75fcd3625e4da300a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507326"
---
# <a name="paymentterms-resource-type"></a><span data-ttu-id="bc242-103">tipo de recurso paymentTerms</span><span class="sxs-lookup"><span data-stu-id="bc242-103">paymentTerms resource type</span></span>
<span data-ttu-id="bc242-104">Representa um termo de pagamento no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="bc242-104">Represents a payment term in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="bc242-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="bc242-105">Methods</span></span>

| <span data-ttu-id="bc242-106">Método</span><span class="sxs-lookup"><span data-stu-id="bc242-106">Method</span></span>                                                      | <span data-ttu-id="bc242-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc242-107">Return Type</span></span>|<span data-ttu-id="bc242-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc242-108">Description</span></span>            |
|:------------------------------------------------------------|:-----------|:----------------------|
|[<span data-ttu-id="bc242-109">Obter paymentTerms</span><span class="sxs-lookup"><span data-stu-id="bc242-109">Get paymentTerms</span></span>](../api/dynamics-paymentterms-get.md)      |<span data-ttu-id="bc242-110">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="bc242-110">paymentTerms</span></span>|<span data-ttu-id="bc242-111">Obter um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="bc242-111">Get a payment terms object.</span></span>   |
|[<span data-ttu-id="bc242-112">Postar paymentTerms</span><span class="sxs-lookup"><span data-stu-id="bc242-112">Post paymentTerms</span></span>](../api/dynamics-create-paymentterms.md)  |<span data-ttu-id="bc242-113">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="bc242-113">paymentTerms</span></span>|<span data-ttu-id="bc242-114">Criar um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="bc242-114">Create a payment terms object.</span></span>|
|[<span data-ttu-id="bc242-115">Patch paymentTerms</span><span class="sxs-lookup"><span data-stu-id="bc242-115">Patch paymentTerms</span></span>](../api/dynamics-paymentterms-update.md) |<span data-ttu-id="bc242-116">paymentTerms</span><span class="sxs-lookup"><span data-stu-id="bc242-116">paymentTerms</span></span>|<span data-ttu-id="bc242-117">Atualizar um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="bc242-117">Update a payment terms object.</span></span>|
|[<span data-ttu-id="bc242-118">Excluir paymentTerms</span><span class="sxs-lookup"><span data-stu-id="bc242-118">Delete paymentTerms</span></span>](../api/dynamics-paymentterms-delete.md)|<span data-ttu-id="bc242-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bc242-119">none</span></span>        |<span data-ttu-id="bc242-120">Excluir um objeto de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="bc242-120">Delete a payment terms object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc242-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc242-121">Properties</span></span>
| <span data-ttu-id="bc242-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc242-122">Property</span></span>                     | <span data-ttu-id="bc242-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc242-123">Type</span></span>     |<span data-ttu-id="bc242-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc242-124">Description</span></span>                                                |
|:-----------------------------|:-------|:----------------------------------------------------------|
|<span data-ttu-id="bc242-125">id</span><span class="sxs-lookup"><span data-stu-id="bc242-125">id</span></span>                            |<span data-ttu-id="bc242-126">GUID</span><span class="sxs-lookup"><span data-stu-id="bc242-126">GUID</span></span>    |<span data-ttu-id="bc242-127">A ID exclusiva do paymentTerms.</span><span class="sxs-lookup"><span data-stu-id="bc242-127">The unique ID of the paymentTerms.</span></span> <span data-ttu-id="bc242-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="bc242-128">Non-editable.</span></span>           |
|<span data-ttu-id="bc242-129">código</span><span class="sxs-lookup"><span data-stu-id="bc242-129">code</span></span>                          |<span data-ttu-id="bc242-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc242-130">string</span></span>  |<span data-ttu-id="bc242-131">Especifica o código da expressão de pagamento.</span><span class="sxs-lookup"><span data-stu-id="bc242-131">Specifies the payment term code.</span></span>                           |
|<span data-ttu-id="bc242-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bc242-132">displayName</span></span>                   |<span data-ttu-id="bc242-133">string</span><span class="sxs-lookup"><span data-stu-id="bc242-133">string</span></span>  |<span data-ttu-id="bc242-134">Especifica o nome de exibição do termo de pagamento.</span><span class="sxs-lookup"><span data-stu-id="bc242-134">Specifies the payment term display name.</span></span>                   |
|<span data-ttu-id="bc242-135">dueDateCalculation</span><span class="sxs-lookup"><span data-stu-id="bc242-135">dueDateCalculation</span></span>            |<span data-ttu-id="bc242-136">string</span><span class="sxs-lookup"><span data-stu-id="bc242-136">string</span></span>  |<span data-ttu-id="bc242-137">Especifica a fórmula usada para calcular a data em que um pagamento deve ser feito.</span><span class="sxs-lookup"><span data-stu-id="bc242-137">Specifies the formula that is used to calculate the date that a payment must be made.</span></span>|
|<span data-ttu-id="bc242-138">discountDateCalculation</span><span class="sxs-lookup"><span data-stu-id="bc242-138">discountDateCalculation</span></span>       |<span data-ttu-id="bc242-139">string</span><span class="sxs-lookup"><span data-stu-id="bc242-139">string</span></span>  |<span data-ttu-id="bc242-140">Especifica a fórmula usada para calcular a data em que um pagamento deve ser feito para obter um desconto.</span><span class="sxs-lookup"><span data-stu-id="bc242-140">Specifies the formula that is used to calculate the date that a payment must be made in order to obtain a discount.</span></span>|
|<span data-ttu-id="bc242-141">discountPercent</span><span class="sxs-lookup"><span data-stu-id="bc242-141">discountPercent</span></span>               |<span data-ttu-id="bc242-142">dígitos</span><span class="sxs-lookup"><span data-stu-id="bc242-142">decimal</span></span> |<span data-ttu-id="bc242-143">Especifica a porcentagem de desconto aplicada ao pagamento antecipado de um valor de fatura.</span><span class="sxs-lookup"><span data-stu-id="bc242-143">Specifies the discount percentage that is applied for early payment of an invoice amount.</span></span>|
|<span data-ttu-id="bc242-144">calculateDiscountOnCreditMemos</span><span class="sxs-lookup"><span data-stu-id="bc242-144">calculateDiscountOnCreditMemos</span></span>|<span data-ttu-id="bc242-145">booliano</span><span class="sxs-lookup"><span data-stu-id="bc242-145">boolean</span></span> |<span data-ttu-id="bc242-146">Especifica se o desconto deve ser aplicado a memorandos de crédito.</span><span class="sxs-lookup"><span data-stu-id="bc242-146">Specifies if the discount should be applied to credit memos.</span></span> <span data-ttu-id="bc242-147">**True** indica que um desconto será fornecido, **false** indica que um desconto não será fornecido.</span><span class="sxs-lookup"><span data-stu-id="bc242-147">**True** indicates a discount will be given, **false** indicates a discount will not be given.</span></span>|
|<span data-ttu-id="bc242-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc242-148">lastModifiedDateTime</span></span>          |<span data-ttu-id="bc242-149">DateTime</span><span class="sxs-lookup"><span data-stu-id="bc242-149">datetime</span></span>|<span data-ttu-id="bc242-150">O último DateTime que o paymentTerms foi modificado.</span><span class="sxs-lookup"><span data-stu-id="bc242-150">The last datetime the paymentTerms was modified.</span></span> <span data-ttu-id="bc242-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc242-151">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="bc242-152">Relações</span><span class="sxs-lookup"><span data-stu-id="bc242-152">Relationships</span></span>
<span data-ttu-id="bc242-153">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bc242-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc242-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc242-154">JSON representation</span></span>

<span data-ttu-id="bc242-155">Veja a seguir uma representação JSON do paymentTerms.</span><span class="sxs-lookup"><span data-stu-id="bc242-155">Here is a JSON representation of the paymentTerms.</span></span>


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
