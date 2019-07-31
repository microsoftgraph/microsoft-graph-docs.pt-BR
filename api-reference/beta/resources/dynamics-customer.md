---
title: tipo de recurso clientes
description: Representa um cliente no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 2a3ad7bade33af9456e65e3c19b988b9d2f679b2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973636"
---
# <a name="customers-resource-type"></a><span data-ttu-id="ddaeb-103">tipo de recurso clientes</span><span class="sxs-lookup"><span data-stu-id="ddaeb-103">customers resource type</span></span>
<span data-ttu-id="ddaeb-104">Representa um cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-104">Represents a customer in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ddaeb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ddaeb-105">Methods</span></span>

| <span data-ttu-id="ddaeb-106">Método</span><span class="sxs-lookup"><span data-stu-id="ddaeb-106">Method</span></span>                                              |<span data-ttu-id="ddaeb-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ddaeb-107">Return Type</span></span>| <span data-ttu-id="ddaeb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddaeb-108">Description</span></span>      |
|:----------------------------------------------------|:----------|:-----------------|
|[<span data-ttu-id="ddaeb-109">Obter clientes</span><span class="sxs-lookup"><span data-stu-id="ddaeb-109">Get customers</span></span>](../api/dynamics-customer-get.md)      |<span data-ttu-id="ddaeb-110">Eles</span><span class="sxs-lookup"><span data-stu-id="ddaeb-110">customers</span></span>   |<span data-ttu-id="ddaeb-111">Obtém um cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-111">Gets a customer.</span></span>   |
|[<span data-ttu-id="ddaeb-112">Criar clientes</span><span class="sxs-lookup"><span data-stu-id="ddaeb-112">Create customers</span></span>](../api/dynamics-create-customer.md)|<span data-ttu-id="ddaeb-113">Eles</span><span class="sxs-lookup"><span data-stu-id="ddaeb-113">customers</span></span>   |<span data-ttu-id="ddaeb-114">Cria um cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-114">Creates a customer.</span></span>|
|[<span data-ttu-id="ddaeb-115">Atualizar clientes</span><span class="sxs-lookup"><span data-stu-id="ddaeb-115">Update customers</span></span>](../api/dynamics-customer-update.md)|<span data-ttu-id="ddaeb-116">Eles</span><span class="sxs-lookup"><span data-stu-id="ddaeb-116">customers</span></span>   |<span data-ttu-id="ddaeb-117">Atualiza um cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-117">Updates a customer.</span></span>|
|[<span data-ttu-id="ddaeb-118">Excluir clientes</span><span class="sxs-lookup"><span data-stu-id="ddaeb-118">Delete customers</span></span>](../api/dynamics-customer-delete.md)|<span data-ttu-id="ddaeb-119">none</span><span class="sxs-lookup"><span data-stu-id="ddaeb-119">none</span></span>        |<span data-ttu-id="ddaeb-120">Exclui um cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-120">Deletes a customer.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddaeb-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddaeb-121">Properties</span></span>
| <span data-ttu-id="ddaeb-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddaeb-122">Property</span></span>    | <span data-ttu-id="ddaeb-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddaeb-123">Type</span></span>     |<span data-ttu-id="ddaeb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddaeb-124">Description</span></span>|
|:------------|:---------|:----------|
|<span data-ttu-id="ddaeb-125">id</span><span class="sxs-lookup"><span data-stu-id="ddaeb-125">id</span></span>           |<span data-ttu-id="ddaeb-126">GUID</span><span class="sxs-lookup"><span data-stu-id="ddaeb-126">GUID</span></span>      |<span data-ttu-id="ddaeb-127">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-127">The unique ID of the item.</span></span> <span data-ttu-id="ddaeb-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-128">Non-editable.</span></span>|
|<span data-ttu-id="ddaeb-129">number</span><span class="sxs-lookup"><span data-stu-id="ddaeb-129">number</span></span>       |<span data-ttu-id="ddaeb-130">string</span><span class="sxs-lookup"><span data-stu-id="ddaeb-130">string</span></span>    |<span data-ttu-id="ddaeb-131">O número do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-131">The customer number.</span></span>|
|<span data-ttu-id="ddaeb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ddaeb-132">displayName</span></span>  |<span data-ttu-id="ddaeb-133">string</span><span class="sxs-lookup"><span data-stu-id="ddaeb-133">string</span></span>    |<span data-ttu-id="ddaeb-134">Especifica o nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-134">Specifies the customer's name.</span></span> <span data-ttu-id="ddaeb-135">Esse nome aparecerá em todos os documentos de vendas do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-135">This name will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="ddaeb-136">type</span><span class="sxs-lookup"><span data-stu-id="ddaeb-136">type</span></span>         |<span data-ttu-id="ddaeb-137">string</span><span class="sxs-lookup"><span data-stu-id="ddaeb-137">string</span></span>    |<span data-ttu-id="ddaeb-138">Especifica o tipo de cliente, pode ser "empresa" ou "pessoa".</span><span class="sxs-lookup"><span data-stu-id="ddaeb-138">Specifies the type of customer, can be "Company" or "Person".</span></span>|
|<span data-ttu-id="ddaeb-139">address</span><span class="sxs-lookup"><span data-stu-id="ddaeb-139">address</span></span>      |[<span data-ttu-id="ddaeb-140">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="ddaeb-140">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="ddaeb-141">Especifica o endereço do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-141">Specifies the customer's address.</span></span> <span data-ttu-id="ddaeb-142">Esse endereço aparecerá em todos os documentos de vendas do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-142">This address will appear on all sales documents for the customer.</span></span>|
|<span data-ttu-id="ddaeb-143">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ddaeb-143">phoneNumber</span></span>  |<span data-ttu-id="ddaeb-144">string</span><span class="sxs-lookup"><span data-stu-id="ddaeb-144">string</span></span>    |<span data-ttu-id="ddaeb-145">Especifica o número de telefone do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-145">Specifies the customer's telephone number.</span></span>|
|<span data-ttu-id="ddaeb-146">email</span><span class="sxs-lookup"><span data-stu-id="ddaeb-146">email</span></span>        |<span data-ttu-id="ddaeb-147">string</span><span class="sxs-lookup"><span data-stu-id="ddaeb-147">string</span></span>    |<span data-ttu-id="ddaeb-148">Especifica o endereço de email do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-148">Specifies the customer's email address.</span></span>|
|<span data-ttu-id="ddaeb-149">site</span><span class="sxs-lookup"><span data-stu-id="ddaeb-149">website</span></span>      |<span data-ttu-id="ddaeb-150">string</span><span class="sxs-lookup"><span data-stu-id="ddaeb-150">string</span></span>    |<span data-ttu-id="ddaeb-151">Especifica o endereço da home page do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-151">Specifies the customer's home page address.</span></span>|
|<span data-ttu-id="ddaeb-152">taxLiable</span><span class="sxs-lookup"><span data-stu-id="ddaeb-152">taxLiable</span></span>    |<span data-ttu-id="ddaeb-153">booliano</span><span class="sxs-lookup"><span data-stu-id="ddaeb-153">boolean</span></span>   |<span data-ttu-id="ddaeb-154">Especifica se o cliente ou fornecedor é responsável pelo imposto sobre vendas.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-154">Specifies if the customer or vendor is liable for sales tax.</span></span> <span data-ttu-id="ddaeb-155">Defina como **true** se o cliente for responsável por impostos.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-155">Set to **true** if the customer is tax liable.</span></span>|
|<span data-ttu-id="ddaeb-156">taxAreaId</span><span class="sxs-lookup"><span data-stu-id="ddaeb-156">taxAreaId</span></span>    |<span data-ttu-id="ddaeb-157">GUID</span><span class="sxs-lookup"><span data-stu-id="ddaeb-157">GUID</span></span>      |<span data-ttu-id="ddaeb-158">Especifica a área de impostos à qual o cliente pertence.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-158">Specifies which tax area the customer belongs to.</span></span>|
|<span data-ttu-id="ddaeb-159">taxAreaDisplayName</span><span class="sxs-lookup"><span data-stu-id="ddaeb-159">taxAreaDisplayName</span></span>|<span data-ttu-id="ddaeb-160">string</span><span class="sxs-lookup"><span data-stu-id="ddaeb-160">string</span></span>|<span data-ttu-id="ddaeb-161">Especificou o nome de exibição da área de impostos à qual o cliente pertence.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-161">Specified the display name of the tax area the customer belongs to.</span></span>|
|<span data-ttu-id="ddaeb-162">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="ddaeb-162">taxRegistrationNumber</span></span>|<span data-ttu-id="ddaeb-163">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="ddaeb-163">string, maximum size 20</span></span>|<span data-ttu-id="ddaeb-164">Especificado o número de registro de imposto do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-164">Specified the tax registration number of the customer.</span></span>|
|<span data-ttu-id="ddaeb-165">CurrencyID</span><span class="sxs-lookup"><span data-stu-id="ddaeb-165">currencyId</span></span>   |<span data-ttu-id="ddaeb-166">GUID</span><span class="sxs-lookup"><span data-stu-id="ddaeb-166">GUID</span></span>      |<span data-ttu-id="ddaeb-167">Especifica a moeda usada pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-167">Specifies which currency the customer uses.</span></span>|
|<span data-ttu-id="ddaeb-168">currencyCode</span><span class="sxs-lookup"><span data-stu-id="ddaeb-168">currencyCode</span></span> |<span data-ttu-id="ddaeb-169">numéricos</span><span class="sxs-lookup"><span data-stu-id="ddaeb-169">numeric</span></span>   |<span data-ttu-id="ddaeb-170">O código de moeda padrão para o cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-170">The default currency code for the customer.</span></span>|
|<span data-ttu-id="ddaeb-171">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="ddaeb-171">paymentTermsId</span></span>|<span data-ttu-id="ddaeb-172">GUID</span><span class="sxs-lookup"><span data-stu-id="ddaeb-172">GUID</span></span>     |<span data-ttu-id="ddaeb-173">Especifica qual termo de pagamento o cliente utiliza.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-173">Specifies which payment term the customer uses.</span></span>|
|<span data-ttu-id="ddaeb-174">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="ddaeb-174">paymentMethodId</span></span>|<span data-ttu-id="ddaeb-175">GUID</span><span class="sxs-lookup"><span data-stu-id="ddaeb-175">GUID</span></span>    |<span data-ttu-id="ddaeb-176">Especifica qual método de pagamento o cliente utiliza.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-176">Specifies which payment method the customer uses.</span></span>|
|<span data-ttu-id="ddaeb-177">shipmentMethodId</span><span class="sxs-lookup"><span data-stu-id="ddaeb-177">shipmentMethodId</span></span>|<span data-ttu-id="ddaeb-178">GUID</span><span class="sxs-lookup"><span data-stu-id="ddaeb-178">GUID</span></span>   |<span data-ttu-id="ddaeb-179">Especifica o método de remessa que o cliente usa.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-179">Specifies which shipment method the customer uses.</span></span>|
|<span data-ttu-id="ddaeb-180">bloqueou</span><span class="sxs-lookup"><span data-stu-id="ddaeb-180">blocked</span></span>      |<span data-ttu-id="ddaeb-181">string</span><span class="sxs-lookup"><span data-stu-id="ddaeb-181">string</span></span>    |<span data-ttu-id="ddaeb-182">Especifica que as transações com o cliente não podem ser lançadas.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-182">Specifies that transactions with the customer cannot be posted.</span></span> <span data-ttu-id="ddaeb-183">Defina como **todos**, se o cliente estiver bloqueado, defina como em branco se não for bloqueado.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-183">Set to **All**, if the customer is blocked, set to blank if not blocked.</span></span>|
|<span data-ttu-id="ddaeb-184">carga</span><span class="sxs-lookup"><span data-stu-id="ddaeb-184">balance</span></span>      |<span data-ttu-id="ddaeb-185">numéricos</span><span class="sxs-lookup"><span data-stu-id="ddaeb-185">numeric</span></span>   |<span data-ttu-id="ddaeb-186">Especifica o valor do pagamento que o cliente está procurando para vendas concluídas.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-186">Specifies the payment amount that the customer owes for completed sales.</span></span> <span data-ttu-id="ddaeb-187">Esse valor também é conhecido como o saldo do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-187">This value is also known as the customer's balance.</span></span> <span data-ttu-id="ddaeb-188">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-188">Read-Only.</span></span>|
|<span data-ttu-id="ddaeb-189">overdueAmount</span><span class="sxs-lookup"><span data-stu-id="ddaeb-189">overdueAmount</span></span>|<span data-ttu-id="ddaeb-190">numéricos</span><span class="sxs-lookup"><span data-stu-id="ddaeb-190">numeric</span></span>   |<span data-ttu-id="ddaeb-191">Especifica o valor vencido do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-191">Specifies the customer's overdue amount.</span></span>|
|<span data-ttu-id="ddaeb-192">totalSalesExcludingTax</span><span class="sxs-lookup"><span data-stu-id="ddaeb-192">totalSalesExcludingTax</span></span>|<span data-ttu-id="ddaeb-193">numéricos</span><span class="sxs-lookup"><span data-stu-id="ddaeb-193">numeric</span></span>|<span data-ttu-id="ddaeb-194">Especifica o valor total de vendas excluindo o imposto do cliente.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-194">Specifies the total sales amount excluding tax of the customer.</span></span>|
|<span data-ttu-id="ddaeb-195">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddaeb-195">lastModifiedDateTime</span></span>|<span data-ttu-id="ddaeb-196">DateTime</span><span class="sxs-lookup"><span data-stu-id="ddaeb-196">datetime</span></span>|<span data-ttu-id="ddaeb-197">O último DateTime que o cliente foi modificado.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-197">The last datetime the customer was modified.</span></span> <span data-ttu-id="ddaeb-198">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-198">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ddaeb-199">Relações</span><span class="sxs-lookup"><span data-stu-id="ddaeb-199">Relationships</span></span>
<span data-ttu-id="ddaeb-200">Uma moeda (currencyCode) deve existir na tabela moedas.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-200">A Currency(currencyCode) must exist in the Currencies table.</span></span>

<span data-ttu-id="ddaeb-201">Um termo de pagamento (paymentTerms) deve existir na tabela de condições de pagamento.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-201">A Payment Term(paymentTerms) must exist in the Payment Terms table.</span></span>

<span data-ttu-id="ddaeb-202">Um método de remessa (shipmentMethod) deve existir na tabela do método de remessa.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-202">A Shipment Method(shipmentMethod) must exist in the Shipment Method table.</span></span>

<span data-ttu-id="ddaeb-203">Um método de pagamento (paymentMethod) deve existir na tabela de métodos de pagamento.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-203">A Payment Method(paymentMethod) must exist in the Payment Method table.</span></span>

<span data-ttu-id="ddaeb-204">Uma área de impostos (taxArea) deve existir na tabela de área de impostos.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-204">A Tax Area(taxArea) must exist in the Tax Area table.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddaeb-205">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddaeb-205">JSON representation</span></span>

<span data-ttu-id="ddaeb-206">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ddaeb-206">Here is a JSON representation of the resource.</span></span>


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

