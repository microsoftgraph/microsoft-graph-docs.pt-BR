---
title: tipo de recurso clientes
description: Representa um cliente no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e4daa28018001fb6cb6e4866bedf8e256a72abef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507256"
---
# <a name="customers-resource-type"></a><span data-ttu-id="7999a-103">tipo de recurso clientes</span><span class="sxs-lookup"><span data-stu-id="7999a-103">customers resource type</span></span>
<span data-ttu-id="7999a-104">Representa um cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="7999a-104">Represents a customer in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="7999a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7999a-105">Methods</span></span>

| <span data-ttu-id="7999a-106">Método</span><span class="sxs-lookup"><span data-stu-id="7999a-106">Method</span></span>                                              |<span data-ttu-id="7999a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7999a-107">Return Type</span></span>| <span data-ttu-id="7999a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7999a-108">Description</span></span>      |
|:----------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="7999a-109">Obter clientes</span><span class="sxs-lookup"><span data-stu-id="7999a-109">Get customers</span></span>](../api/dynamics-customer-get.md)      |<span data-ttu-id="7999a-110">Eles</span><span class="sxs-lookup"><span data-stu-id="7999a-110">customers</span></span>   |<span data-ttu-id="7999a-111">Obtém um cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-111">Gets a customer.</span></span>   |
|[<span data-ttu-id="7999a-112">Criar clientes</span><span class="sxs-lookup"><span data-stu-id="7999a-112">Create customers</span></span>](../api/dynamics-create-customer.md)|<span data-ttu-id="7999a-113">Eles</span><span class="sxs-lookup"><span data-stu-id="7999a-113">customers</span></span>   |<span data-ttu-id="7999a-114">Cria um cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-114">Creates a customer.</span></span>|
|[<span data-ttu-id="7999a-115">Atualizar clientes</span><span class="sxs-lookup"><span data-stu-id="7999a-115">Update customers</span></span>](../api/dynamics-customer-update.md)|<span data-ttu-id="7999a-116">Eles</span><span class="sxs-lookup"><span data-stu-id="7999a-116">customers</span></span>   |<span data-ttu-id="7999a-117">Atualiza um cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-117">Updates a customer.</span></span>|
|[<span data-ttu-id="7999a-118">Excluir clientes</span><span class="sxs-lookup"><span data-stu-id="7999a-118">Delete customers</span></span>](../api/dynamics-customer-delete.md)|<span data-ttu-id="7999a-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7999a-119">none</span></span>        |<span data-ttu-id="7999a-120">Exclui um cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-120">Deletes a customer.</span></span>|

## <a name="properties"></a><span data-ttu-id="7999a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7999a-121">Properties</span></span>
| <span data-ttu-id="7999a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7999a-122">Property</span></span>    | <span data-ttu-id="7999a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7999a-123">Type</span></span>     |<span data-ttu-id="7999a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7999a-124">Description</span></span>|
|:------------|:---------|:----------|
|<span data-ttu-id="7999a-125">id</span><span class="sxs-lookup"><span data-stu-id="7999a-125">id</span></span>           |<span data-ttu-id="7999a-126">GUID</span><span class="sxs-lookup"><span data-stu-id="7999a-126">GUID</span></span>      |<span data-ttu-id="7999a-127">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="7999a-127">The unique ID of the item.</span></span> <span data-ttu-id="7999a-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="7999a-128">Non-editable.</span></span>|
|<span data-ttu-id="7999a-129">number</span><span class="sxs-lookup"><span data-stu-id="7999a-129">number</span></span>       |<span data-ttu-id="7999a-130">string</span><span class="sxs-lookup"><span data-stu-id="7999a-130">string</span></span>    |<span data-ttu-id="7999a-131">O número do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-131">The customer number.</span></span>|
|<span data-ttu-id="7999a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7999a-132">displayName</span></span>  |<span data-ttu-id="7999a-133">string</span><span class="sxs-lookup"><span data-stu-id="7999a-133">string</span></span>    |<span data-ttu-id="7999a-134">Especifica o nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-134">Specifies the customer's name.</span></span> <span data-ttu-id="7999a-135">Esse nome aparecerá em todos os documentos de vendas do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-135">This name will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="7999a-136">type</span><span class="sxs-lookup"><span data-stu-id="7999a-136">type</span></span>         |<span data-ttu-id="7999a-137">string</span><span class="sxs-lookup"><span data-stu-id="7999a-137">string</span></span>    |<span data-ttu-id="7999a-138">Especifica o tipo de cliente, pode ser "empresa" ou "pessoa".</span><span class="sxs-lookup"><span data-stu-id="7999a-138">Specifies the type of customer, can be "Company" or "Person".</span></span>|
|<span data-ttu-id="7999a-139">address</span><span class="sxs-lookup"><span data-stu-id="7999a-139">address</span></span>      |[<span data-ttu-id="7999a-140">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="7999a-140">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="7999a-141">Especifica o endereço do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-141">Specifies the customer's address.</span></span> <span data-ttu-id="7999a-142">Esse endereço aparecerá em todos os documentos de vendas do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-142">This address will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="7999a-143">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="7999a-143">phoneNumber</span></span>  |<span data-ttu-id="7999a-144">string</span><span class="sxs-lookup"><span data-stu-id="7999a-144">string</span></span>    |<span data-ttu-id="7999a-145">Especifica o número de telefone do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-145">Specifies the customer's telephone number.</span></span>|
|<span data-ttu-id="7999a-146">email</span><span class="sxs-lookup"><span data-stu-id="7999a-146">email</span></span>        |<span data-ttu-id="7999a-147">string</span><span class="sxs-lookup"><span data-stu-id="7999a-147">string</span></span>    |<span data-ttu-id="7999a-148">Especifica o endereço de email do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-148">Specifies the customer's email address.</span></span>|
|<span data-ttu-id="7999a-149">site</span><span class="sxs-lookup"><span data-stu-id="7999a-149">website</span></span>      |<span data-ttu-id="7999a-150">string</span><span class="sxs-lookup"><span data-stu-id="7999a-150">string</span></span>    |<span data-ttu-id="7999a-151">Especifica o endereço da home page do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-151">Specifies the customer's home page address.</span></span>|
|<span data-ttu-id="7999a-152">taxLiable</span><span class="sxs-lookup"><span data-stu-id="7999a-152">taxLiable</span></span>    |<span data-ttu-id="7999a-153">booliano</span><span class="sxs-lookup"><span data-stu-id="7999a-153">boolean</span></span>   |<span data-ttu-id="7999a-154">Especifica se o cliente ou fornecedor é responsável pelo imposto sobre vendas.</span><span class="sxs-lookup"><span data-stu-id="7999a-154">Specifies if the customer or vendor is liable for sales tax.</span></span> <span data-ttu-id="7999a-155">Defina como **true** se o cliente for responsável por impostos.</span><span class="sxs-lookup"><span data-stu-id="7999a-155">Set to **true** if the customer is tax liable.</span></span>|
|<span data-ttu-id="7999a-156">taxAreaId</span><span class="sxs-lookup"><span data-stu-id="7999a-156">taxAreaId</span></span>    |<span data-ttu-id="7999a-157">GUID</span><span class="sxs-lookup"><span data-stu-id="7999a-157">GUID</span></span>      |<span data-ttu-id="7999a-158">Especifica a área de impostos à qual o cliente pertence.</span><span class="sxs-lookup"><span data-stu-id="7999a-158">Specifies which tax area the customer belongs to.</span></span>|
|<span data-ttu-id="7999a-159">taxAreaDisplayName</span><span class="sxs-lookup"><span data-stu-id="7999a-159">taxAreaDisplayName</span></span>|<span data-ttu-id="7999a-160">string</span><span class="sxs-lookup"><span data-stu-id="7999a-160">string</span></span>|<span data-ttu-id="7999a-161">Especificou o nome de exibição da área de impostos à qual o cliente pertence.</span><span class="sxs-lookup"><span data-stu-id="7999a-161">Specified the display name of the tax area the customer belongs to.</span></span>|
|<span data-ttu-id="7999a-162">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="7999a-162">taxRegistrationNumber</span></span>|<span data-ttu-id="7999a-163">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="7999a-163">string, maximum size 20</span></span>|<span data-ttu-id="7999a-164">Especificado o número de registro de imposto do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-164">Specified the tax registration number of the customer.</span></span>|
|<span data-ttu-id="7999a-165">CurrencyID</span><span class="sxs-lookup"><span data-stu-id="7999a-165">currencyId</span></span>   |<span data-ttu-id="7999a-166">GUID</span><span class="sxs-lookup"><span data-stu-id="7999a-166">GUID</span></span>      |<span data-ttu-id="7999a-167">Especifica a moeda usada pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-167">Specifies which currency the customer uses.</span></span>|
|<span data-ttu-id="7999a-168">currencyCode</span><span class="sxs-lookup"><span data-stu-id="7999a-168">currencyCode</span></span> |<span data-ttu-id="7999a-169">numéricos</span><span class="sxs-lookup"><span data-stu-id="7999a-169">numeric</span></span>   |<span data-ttu-id="7999a-170">O código de moeda padrão para o cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-170">The default currency code for the customer.</span></span>|
|<span data-ttu-id="7999a-171">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="7999a-171">paymentTermsId</span></span>|<span data-ttu-id="7999a-172">GUID</span><span class="sxs-lookup"><span data-stu-id="7999a-172">GUID</span></span>     |<span data-ttu-id="7999a-173">Especifica qual termo de pagamento o cliente utiliza.</span><span class="sxs-lookup"><span data-stu-id="7999a-173">Specifies which payment term the customer uses.</span></span>|
|<span data-ttu-id="7999a-174">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="7999a-174">paymentMethodId</span></span>|<span data-ttu-id="7999a-175">GUID</span><span class="sxs-lookup"><span data-stu-id="7999a-175">GUID</span></span>    |<span data-ttu-id="7999a-176">Especifica qual método de pagamento o cliente utiliza.</span><span class="sxs-lookup"><span data-stu-id="7999a-176">Specifies which payment method the customer uses.</span></span>|
|<span data-ttu-id="7999a-177">shipmentMethodId</span><span class="sxs-lookup"><span data-stu-id="7999a-177">shipmentMethodId</span></span>|<span data-ttu-id="7999a-178">GUID</span><span class="sxs-lookup"><span data-stu-id="7999a-178">GUID</span></span>   |<span data-ttu-id="7999a-179">Especifica o método de remessa que o cliente usa.</span><span class="sxs-lookup"><span data-stu-id="7999a-179">Specifies which shipment method the customer uses.</span></span>|
|<span data-ttu-id="7999a-180">bloqueou</span><span class="sxs-lookup"><span data-stu-id="7999a-180">blocked</span></span>      |<span data-ttu-id="7999a-181">string</span><span class="sxs-lookup"><span data-stu-id="7999a-181">string</span></span>    |<span data-ttu-id="7999a-182">Especifica que as transações com o cliente não podem ser lançadas.</span><span class="sxs-lookup"><span data-stu-id="7999a-182">Specifies that transactions with the customer cannot be posted.</span></span> <span data-ttu-id="7999a-183">Defina como **todos**, se o cliente estiver bloqueado, defina como em branco se não for bloqueado.</span><span class="sxs-lookup"><span data-stu-id="7999a-183">Set to **All**, if the customer is blocked, set to blank if not blocked.</span></span>|
|<span data-ttu-id="7999a-184">carga</span><span class="sxs-lookup"><span data-stu-id="7999a-184">balance</span></span>      |<span data-ttu-id="7999a-185">numéricos</span><span class="sxs-lookup"><span data-stu-id="7999a-185">numeric</span></span>   |<span data-ttu-id="7999a-186">Especifica o valor do pagamento que o cliente está procurando para vendas concluídas.</span><span class="sxs-lookup"><span data-stu-id="7999a-186">Specifies the payment amount that the customer owes for completed sales.</span></span> <span data-ttu-id="7999a-187">Esse valor também é conhecido como o saldo do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-187">This value is also known as the customer's balance.</span></span> <span data-ttu-id="7999a-188">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="7999a-188">Read-Only.</span></span>|
|<span data-ttu-id="7999a-189">overdueAmount</span><span class="sxs-lookup"><span data-stu-id="7999a-189">overdueAmount</span></span>|<span data-ttu-id="7999a-190">numéricos</span><span class="sxs-lookup"><span data-stu-id="7999a-190">numeric</span></span>   |<span data-ttu-id="7999a-191">Especifica o valor vencido do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-191">Specifies the customer's overdue amount.</span></span>|
|<span data-ttu-id="7999a-192">totalSalesExcludingTax</span><span class="sxs-lookup"><span data-stu-id="7999a-192">totalSalesExcludingTax</span></span>|<span data-ttu-id="7999a-193">numéricos</span><span class="sxs-lookup"><span data-stu-id="7999a-193">numeric</span></span>|<span data-ttu-id="7999a-194">Especifica o valor total de vendas excluindo o imposto do cliente.</span><span class="sxs-lookup"><span data-stu-id="7999a-194">Specifies the total sales amount excluding tax of the customer.</span></span>|
|<span data-ttu-id="7999a-195">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7999a-195">lastModifiedDateTime</span></span>|<span data-ttu-id="7999a-196">DateTime</span><span class="sxs-lookup"><span data-stu-id="7999a-196">datetime</span></span>|<span data-ttu-id="7999a-197">O último DateTime que o cliente foi modificado.</span><span class="sxs-lookup"><span data-stu-id="7999a-197">The last datetime the customer was modified.</span></span> <span data-ttu-id="7999a-198">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7999a-198">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="7999a-199">Relações</span><span class="sxs-lookup"><span data-stu-id="7999a-199">Relationships</span></span>
<span data-ttu-id="7999a-200">Uma moeda (currencyCode) deve existir na tabela moedas.</span><span class="sxs-lookup"><span data-stu-id="7999a-200">A Currency(currencyCode) must exist in the Currencies table.</span></span>

<span data-ttu-id="7999a-201">Um termo de pagamento (paymentTerms) deve existir na tabela de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="7999a-201">A Payment Term(paymentTerms) must exist in the Payment Terms table.</span></span>

<span data-ttu-id="7999a-202">Um método de remessa (shipmentMethod) deve existir na tabela do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="7999a-202">A Shipment Method(shipmentMethod) must exist in the Shipment Method table.</span></span>

<span data-ttu-id="7999a-203">Um método de pagamento (paymentMethod) deve existir na tabela de métodos de pagamento.</span><span class="sxs-lookup"><span data-stu-id="7999a-203">A Payment Method(paymentMethod) must exist in the Payment Method table.</span></span>

<span data-ttu-id="7999a-204">Uma área de impostos (taxArea) deve existir na tabela de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="7999a-204">A Tax Area(taxArea) must exist in the Tax Area table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7999a-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7999a-205">JSON representation</span></span>

<span data-ttu-id="7999a-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7999a-206">Here is a JSON representation of the resource.</span></span>


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

