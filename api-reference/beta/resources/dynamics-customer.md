---
title: tipo de recurso clientes
description: Representa um cliente no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: c6b39829d2b55dc872d281443eaad1b279715b50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989707"
---
# <a name="customers-resource-type"></a><span data-ttu-id="ed274-103">tipo de recurso clientes</span><span class="sxs-lookup"><span data-stu-id="ed274-103">customers resource type</span></span>

<span data-ttu-id="ed274-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed274-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed274-105">Representa um cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="ed274-105">Represents a customer in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ed274-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ed274-106">Methods</span></span>

| <span data-ttu-id="ed274-107">Método</span><span class="sxs-lookup"><span data-stu-id="ed274-107">Method</span></span>                                              |<span data-ttu-id="ed274-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed274-108">Return Type</span></span>| <span data-ttu-id="ed274-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed274-109">Description</span></span>      |
|:----------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="ed274-110">Obter clientes</span><span class="sxs-lookup"><span data-stu-id="ed274-110">Get customers</span></span>](../api/dynamics-customer-get.md)      |<span data-ttu-id="ed274-111">Eles</span><span class="sxs-lookup"><span data-stu-id="ed274-111">customers</span></span>   |<span data-ttu-id="ed274-112">Obtém um cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-112">Gets a customer.</span></span>   |
|[<span data-ttu-id="ed274-113">Criar clientes</span><span class="sxs-lookup"><span data-stu-id="ed274-113">Create customers</span></span>](../api/dynamics-create-customer.md)|<span data-ttu-id="ed274-114">Eles</span><span class="sxs-lookup"><span data-stu-id="ed274-114">customers</span></span>   |<span data-ttu-id="ed274-115">Cria um cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-115">Creates a customer.</span></span>|
|[<span data-ttu-id="ed274-116">Atualizar clientes</span><span class="sxs-lookup"><span data-stu-id="ed274-116">Update customers</span></span>](../api/dynamics-customer-update.md)|<span data-ttu-id="ed274-117">Eles</span><span class="sxs-lookup"><span data-stu-id="ed274-117">customers</span></span>   |<span data-ttu-id="ed274-118">Atualiza um cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-118">Updates a customer.</span></span>|
|[<span data-ttu-id="ed274-119">Excluir clientes</span><span class="sxs-lookup"><span data-stu-id="ed274-119">Delete customers</span></span>](../api/dynamics-customer-delete.md)|<span data-ttu-id="ed274-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ed274-120">none</span></span>        |<span data-ttu-id="ed274-121">Exclui um cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-121">Deletes a customer.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed274-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed274-122">Properties</span></span>
| <span data-ttu-id="ed274-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed274-123">Property</span></span>    | <span data-ttu-id="ed274-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed274-124">Type</span></span>     |<span data-ttu-id="ed274-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed274-125">Description</span></span>|
|:------------|:---------|:----------|
|<span data-ttu-id="ed274-126">id</span><span class="sxs-lookup"><span data-stu-id="ed274-126">id</span></span>           |<span data-ttu-id="ed274-127">GUID</span><span class="sxs-lookup"><span data-stu-id="ed274-127">GUID</span></span>      |<span data-ttu-id="ed274-128">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="ed274-128">The unique ID of the item.</span></span> <span data-ttu-id="ed274-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="ed274-129">Non-editable.</span></span>|
|<span data-ttu-id="ed274-130">number</span><span class="sxs-lookup"><span data-stu-id="ed274-130">number</span></span>       |<span data-ttu-id="ed274-131">string</span><span class="sxs-lookup"><span data-stu-id="ed274-131">string</span></span>    |<span data-ttu-id="ed274-132">O número do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-132">The customer number.</span></span>|
|<span data-ttu-id="ed274-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ed274-133">displayName</span></span>  |<span data-ttu-id="ed274-134">string</span><span class="sxs-lookup"><span data-stu-id="ed274-134">string</span></span>    |<span data-ttu-id="ed274-135">Especifica o nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-135">Specifies the customer's name.</span></span> <span data-ttu-id="ed274-136">Esse nome aparecerá em todos os documentos de vendas do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-136">This name will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="ed274-137">type</span><span class="sxs-lookup"><span data-stu-id="ed274-137">type</span></span>         |<span data-ttu-id="ed274-138">string</span><span class="sxs-lookup"><span data-stu-id="ed274-138">string</span></span>    |<span data-ttu-id="ed274-139">Especifica o tipo de cliente, pode ser "empresa" ou "pessoa".</span><span class="sxs-lookup"><span data-stu-id="ed274-139">Specifies the type of customer, can be "Company" or "Person".</span></span>|
|<span data-ttu-id="ed274-140">address</span><span class="sxs-lookup"><span data-stu-id="ed274-140">address</span></span>      |[<span data-ttu-id="ed274-141">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="ed274-141">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="ed274-142">Especifica o endereço do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-142">Specifies the customer's address.</span></span> <span data-ttu-id="ed274-143">Esse endereço aparecerá em todos os documentos de vendas do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-143">This address will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="ed274-144">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ed274-144">phoneNumber</span></span>  |<span data-ttu-id="ed274-145">string</span><span class="sxs-lookup"><span data-stu-id="ed274-145">string</span></span>    |<span data-ttu-id="ed274-146">Especifica o número de telefone do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-146">Specifies the customer's telephone number.</span></span>|
|<span data-ttu-id="ed274-147">email</span><span class="sxs-lookup"><span data-stu-id="ed274-147">email</span></span>        |<span data-ttu-id="ed274-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed274-148">string</span></span>    |<span data-ttu-id="ed274-149">Especifica o endereço de email do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-149">Specifies the customer's email address.</span></span>|
|<span data-ttu-id="ed274-150">site</span><span class="sxs-lookup"><span data-stu-id="ed274-150">website</span></span>      |<span data-ttu-id="ed274-151">string</span><span class="sxs-lookup"><span data-stu-id="ed274-151">string</span></span>    |<span data-ttu-id="ed274-152">Especifica o endereço da home page do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-152">Specifies the customer's home page address.</span></span>|
|<span data-ttu-id="ed274-153">taxLiable</span><span class="sxs-lookup"><span data-stu-id="ed274-153">taxLiable</span></span>    |<span data-ttu-id="ed274-154">booliano</span><span class="sxs-lookup"><span data-stu-id="ed274-154">boolean</span></span>   |<span data-ttu-id="ed274-155">Especifica se o cliente ou fornecedor é responsável pelo imposto sobre vendas.</span><span class="sxs-lookup"><span data-stu-id="ed274-155">Specifies if the customer or vendor is liable for sales tax.</span></span> <span data-ttu-id="ed274-156">Defina como **true** se o cliente for responsável por impostos.</span><span class="sxs-lookup"><span data-stu-id="ed274-156">Set to **true** if the customer is tax liable.</span></span>|
|<span data-ttu-id="ed274-157">taxAreaId</span><span class="sxs-lookup"><span data-stu-id="ed274-157">taxAreaId</span></span>    |<span data-ttu-id="ed274-158">GUID</span><span class="sxs-lookup"><span data-stu-id="ed274-158">GUID</span></span>      |<span data-ttu-id="ed274-159">Especifica a área de impostos à qual o cliente pertence.</span><span class="sxs-lookup"><span data-stu-id="ed274-159">Specifies which tax area the customer belongs to.</span></span>|
|<span data-ttu-id="ed274-160">taxAreaDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed274-160">taxAreaDisplayName</span></span>|<span data-ttu-id="ed274-161">string</span><span class="sxs-lookup"><span data-stu-id="ed274-161">string</span></span>|<span data-ttu-id="ed274-162">Especificou o nome de exibição da área de impostos à qual o cliente pertence.</span><span class="sxs-lookup"><span data-stu-id="ed274-162">Specified the display name of the tax area the customer belongs to.</span></span>|
|<span data-ttu-id="ed274-163">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="ed274-163">taxRegistrationNumber</span></span>|<span data-ttu-id="ed274-164">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="ed274-164">string, maximum size 20</span></span>|<span data-ttu-id="ed274-165">Especificado o número de registro de imposto do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-165">Specified the tax registration number of the customer.</span></span>|
|<span data-ttu-id="ed274-166">CurrencyID</span><span class="sxs-lookup"><span data-stu-id="ed274-166">currencyId</span></span>   |<span data-ttu-id="ed274-167">GUID</span><span class="sxs-lookup"><span data-stu-id="ed274-167">GUID</span></span>      |<span data-ttu-id="ed274-168">Especifica a moeda usada pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-168">Specifies which currency the customer uses.</span></span>|
|<span data-ttu-id="ed274-169">currencyCode</span><span class="sxs-lookup"><span data-stu-id="ed274-169">currencyCode</span></span> |<span data-ttu-id="ed274-170">numéricos</span><span class="sxs-lookup"><span data-stu-id="ed274-170">numeric</span></span>   |<span data-ttu-id="ed274-171">O código de moeda padrão para o cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-171">The default currency code for the customer.</span></span>|
|<span data-ttu-id="ed274-172">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="ed274-172">paymentTermsId</span></span>|<span data-ttu-id="ed274-173">GUID</span><span class="sxs-lookup"><span data-stu-id="ed274-173">GUID</span></span>     |<span data-ttu-id="ed274-174">Especifica qual termo de pagamento o cliente utiliza.</span><span class="sxs-lookup"><span data-stu-id="ed274-174">Specifies which payment term the customer uses.</span></span>|
|<span data-ttu-id="ed274-175">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="ed274-175">paymentMethodId</span></span>|<span data-ttu-id="ed274-176">GUID</span><span class="sxs-lookup"><span data-stu-id="ed274-176">GUID</span></span>    |<span data-ttu-id="ed274-177">Especifica qual método de pagamento o cliente utiliza.</span><span class="sxs-lookup"><span data-stu-id="ed274-177">Specifies which payment method the customer uses.</span></span>|
|<span data-ttu-id="ed274-178">shipmentMethodId</span><span class="sxs-lookup"><span data-stu-id="ed274-178">shipmentMethodId</span></span>|<span data-ttu-id="ed274-179">GUID</span><span class="sxs-lookup"><span data-stu-id="ed274-179">GUID</span></span>   |<span data-ttu-id="ed274-180">Especifica o método de remessa que o cliente usa.</span><span class="sxs-lookup"><span data-stu-id="ed274-180">Specifies which shipment method the customer uses.</span></span>|
|<span data-ttu-id="ed274-181">bloqueou</span><span class="sxs-lookup"><span data-stu-id="ed274-181">blocked</span></span>      |<span data-ttu-id="ed274-182">string</span><span class="sxs-lookup"><span data-stu-id="ed274-182">string</span></span>    |<span data-ttu-id="ed274-183">Especifica que as transações com o cliente não podem ser lançadas.</span><span class="sxs-lookup"><span data-stu-id="ed274-183">Specifies that transactions with the customer cannot be posted.</span></span> <span data-ttu-id="ed274-184">Defina como **todos**, se o cliente estiver bloqueado, defina como em branco se não for bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ed274-184">Set to **All**, if the customer is blocked, set to blank if not blocked.</span></span>|
|<span data-ttu-id="ed274-185">carga</span><span class="sxs-lookup"><span data-stu-id="ed274-185">balance</span></span>      |<span data-ttu-id="ed274-186">numéricos</span><span class="sxs-lookup"><span data-stu-id="ed274-186">numeric</span></span>   |<span data-ttu-id="ed274-187">Especifica o valor do pagamento que o cliente está procurando para vendas concluídas.</span><span class="sxs-lookup"><span data-stu-id="ed274-187">Specifies the payment amount that the customer owes for completed sales.</span></span> <span data-ttu-id="ed274-188">Esse valor também é conhecido como o saldo do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-188">This value is also known as the customer's balance.</span></span> <span data-ttu-id="ed274-189">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="ed274-189">Read-Only.</span></span>|
|<span data-ttu-id="ed274-190">overdueAmount</span><span class="sxs-lookup"><span data-stu-id="ed274-190">overdueAmount</span></span>|<span data-ttu-id="ed274-191">numéricos</span><span class="sxs-lookup"><span data-stu-id="ed274-191">numeric</span></span>   |<span data-ttu-id="ed274-192">Especifica o valor vencido do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-192">Specifies the customer's overdue amount.</span></span>|
|<span data-ttu-id="ed274-193">totalSalesExcludingTax</span><span class="sxs-lookup"><span data-stu-id="ed274-193">totalSalesExcludingTax</span></span>|<span data-ttu-id="ed274-194">numéricos</span><span class="sxs-lookup"><span data-stu-id="ed274-194">numeric</span></span>|<span data-ttu-id="ed274-195">Especifica o valor total de vendas excluindo o imposto do cliente.</span><span class="sxs-lookup"><span data-stu-id="ed274-195">Specifies the total sales amount excluding tax of the customer.</span></span>|
|<span data-ttu-id="ed274-196">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed274-196">lastModifiedDateTime</span></span>|<span data-ttu-id="ed274-197">datetime</span><span class="sxs-lookup"><span data-stu-id="ed274-197">datetime</span></span>|<span data-ttu-id="ed274-198">O último DateTime que o cliente foi modificado.</span><span class="sxs-lookup"><span data-stu-id="ed274-198">The last datetime the customer was modified.</span></span> <span data-ttu-id="ed274-199">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ed274-199">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ed274-200">Relações</span><span class="sxs-lookup"><span data-stu-id="ed274-200">Relationships</span></span>
<span data-ttu-id="ed274-201">Uma moeda (currencyCode) deve existir na tabela moedas.</span><span class="sxs-lookup"><span data-stu-id="ed274-201">A Currency(currencyCode) must exist in the Currencies table.</span></span>

<span data-ttu-id="ed274-202">Um termo de pagamento (paymentTerms) deve existir na tabela de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="ed274-202">A Payment Term(paymentTerms) must exist in the Payment Terms table.</span></span>

<span data-ttu-id="ed274-203">Um método de remessa (shipmentMethod) deve existir na tabela do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="ed274-203">A Shipment Method(shipmentMethod) must exist in the Shipment Method table.</span></span>

<span data-ttu-id="ed274-204">Um método de pagamento (paymentMethod) deve existir na tabela de métodos de pagamento.</span><span class="sxs-lookup"><span data-stu-id="ed274-204">A Payment Method(paymentMethod) must exist in the Payment Method table.</span></span>

<span data-ttu-id="ed274-205">Uma área de impostos (taxArea) deve existir na tabela de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="ed274-205">A Tax Area(taxArea) must exist in the Tax Area table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed274-206">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed274-206">JSON representation</span></span>

<span data-ttu-id="ed274-207">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed274-207">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "address": NAV.PostalAddress,
    "phoneNumber": "string",
    "email": "string",
    "website": "string",
    "taxLiable": "boolean",
    "taxAreaId": "GUID",
    "taxAreaDisplayName": "string",
    "taxRegistrationNumber": "string",
    "currencyCode": "string",
    "paymentTermsId": "GUID",
    "shipmentMethodId": "GUID",
    "paymentMethodId":  "GUID",
    "blocked": "string",
    "balance": "decimal",
    "overdueAmount": "numeric",
    "totalSalesExcludingTax": "numeric",
    "lastModifiedDateTime": "datetime"
}


```



