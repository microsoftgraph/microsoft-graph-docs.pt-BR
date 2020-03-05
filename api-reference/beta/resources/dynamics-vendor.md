---
title: tipo de recurso fornecedores
description: Um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d05b30dbbb5ecb6aa8a1934a5fe2a1b35cbe890b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502855"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="dd318-103">tipo de recurso fornecedores</span><span class="sxs-lookup"><span data-stu-id="dd318-103">vendors resource type</span></span>

<span data-ttu-id="dd318-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dd318-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd318-105">Representa um fornecedor no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="dd318-105">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="dd318-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dd318-106">Methods</span></span>

| <span data-ttu-id="dd318-107">Método</span><span class="sxs-lookup"><span data-stu-id="dd318-107">Method</span></span>       | <span data-ttu-id="dd318-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dd318-108">Return Type</span></span>  |<span data-ttu-id="dd318-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd318-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd318-110">Obter fornecedores</span><span class="sxs-lookup"><span data-stu-id="dd318-110">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="dd318-111">fornecedor</span><span class="sxs-lookup"><span data-stu-id="dd318-111">vendors</span></span>|<span data-ttu-id="dd318-112">Obtém um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-112">Gets a vendor object.</span></span>|
|[<span data-ttu-id="dd318-113">Lançar fornecedores</span><span class="sxs-lookup"><span data-stu-id="dd318-113">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="dd318-114">fornecedor</span><span class="sxs-lookup"><span data-stu-id="dd318-114">vendors</span></span>|<span data-ttu-id="dd318-115">Cria um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-115">Creates a vendor object.</span></span>|
|[<span data-ttu-id="dd318-116">Fornecedores de patch</span><span class="sxs-lookup"><span data-stu-id="dd318-116">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="dd318-117">fornecedor</span><span class="sxs-lookup"><span data-stu-id="dd318-117">vendors</span></span>|<span data-ttu-id="dd318-118">Atualiza um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-118">Updates a vendor object.</span></span>|
|[<span data-ttu-id="dd318-119">Excluir fornecedor</span><span class="sxs-lookup"><span data-stu-id="dd318-119">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="dd318-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="dd318-120">none</span></span>|<span data-ttu-id="dd318-121">Exclui um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-121">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd318-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd318-122">Properties</span></span>
| <span data-ttu-id="dd318-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd318-123">Property</span></span>     | <span data-ttu-id="dd318-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd318-124">Type</span></span>   |<span data-ttu-id="dd318-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd318-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd318-126">id</span><span class="sxs-lookup"><span data-stu-id="dd318-126">id</span></span>|<span data-ttu-id="dd318-127">GUID</span><span class="sxs-lookup"><span data-stu-id="dd318-127">GUID</span></span>|<span data-ttu-id="dd318-128">A ID exclusiva do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-128">The unique ID of the vendor.</span></span> <span data-ttu-id="dd318-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="dd318-129">Non-editable.</span></span>|
|<span data-ttu-id="dd318-130">number</span><span class="sxs-lookup"><span data-stu-id="dd318-130">number</span></span>|<span data-ttu-id="dd318-131">string</span><span class="sxs-lookup"><span data-stu-id="dd318-131">string</span></span>|<span data-ttu-id="dd318-132">O número do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-132">The vendor number.</span></span>|
|<span data-ttu-id="dd318-133">displayName</span><span class="sxs-lookup"><span data-stu-id="dd318-133">displayName</span></span>|<span data-ttu-id="dd318-134">string</span><span class="sxs-lookup"><span data-stu-id="dd318-134">string</span></span>|<span data-ttu-id="dd318-135">O nome de exibição do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-135">The vendor's display name.</span></span>|
|<span data-ttu-id="dd318-136">address</span><span class="sxs-lookup"><span data-stu-id="dd318-136">address</span></span>|[<span data-ttu-id="dd318-137">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="dd318-137">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="dd318-138">O endereço do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-138">The vendor's address.</span></span>|
|<span data-ttu-id="dd318-139">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="dd318-139">phoneNumber</span></span>|<span data-ttu-id="dd318-140">string</span><span class="sxs-lookup"><span data-stu-id="dd318-140">string</span></span>|<span data-ttu-id="dd318-141">O número de telefone do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-141">The vendor's telephone number.</span></span>|
|<span data-ttu-id="dd318-142">email</span><span class="sxs-lookup"><span data-stu-id="dd318-142">email</span></span>|<span data-ttu-id="dd318-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd318-143">string</span></span>|<span data-ttu-id="dd318-144">O endereço de email do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-144">The vendor's email address.</span></span>|
|<span data-ttu-id="dd318-145">site</span><span class="sxs-lookup"><span data-stu-id="dd318-145">website</span></span>|<span data-ttu-id="dd318-146">string</span><span class="sxs-lookup"><span data-stu-id="dd318-146">string</span></span>|<span data-ttu-id="dd318-147">O endereço do site do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-147">The vendor's website address.</span></span>|
|<span data-ttu-id="dd318-148">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="dd318-148">taxRegistrationNumber</span></span>|<span data-ttu-id="dd318-149">string</span><span class="sxs-lookup"><span data-stu-id="dd318-149">string</span></span>|<span data-ttu-id="dd318-150">O número de registro de imposto do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-150">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="dd318-151">CurrencyID</span><span class="sxs-lookup"><span data-stu-id="dd318-151">currencyId</span></span>|<span data-ttu-id="dd318-152">GUID</span><span class="sxs-lookup"><span data-stu-id="dd318-152">GUID</span></span>|<span data-ttu-id="dd318-153">A ID do código de moeda padrão do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-153">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="dd318-154">currencyCode</span><span class="sxs-lookup"><span data-stu-id="dd318-154">currencyCode</span></span>|<span data-ttu-id="dd318-155">string</span><span class="sxs-lookup"><span data-stu-id="dd318-155">string</span></span>|<span data-ttu-id="dd318-156">O código de moeda padrão do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-156">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="dd318-157">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="dd318-157">irs1099Code</span></span>|<span data-ttu-id="dd318-158">string</span><span class="sxs-lookup"><span data-stu-id="dd318-158">string</span></span>|<span data-ttu-id="dd318-159">Especifica um código 1099 para o fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-159">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="dd318-160">Somente EUA.</span><span class="sxs-lookup"><span data-stu-id="dd318-160">US only.</span></span>|
|<span data-ttu-id="dd318-161">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="dd318-161">paymentTermsId</span></span>|<span data-ttu-id="dd318-162">GUID</span><span class="sxs-lookup"><span data-stu-id="dd318-162">GUID</span></span>|<span data-ttu-id="dd318-163">A ID padrão dos termos de pagamento do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-163">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="dd318-164">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="dd318-164">paymentMethodId</span></span>|<span data-ttu-id="dd318-165">GUID</span><span class="sxs-lookup"><span data-stu-id="dd318-165">GUID</span></span>|<span data-ttu-id="dd318-166">A ID de método de pagamento padrão para o fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-166">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="dd318-167">taxLiable</span><span class="sxs-lookup"><span data-stu-id="dd318-167">taxLiable</span></span>|<span data-ttu-id="dd318-168">booliano</span><span class="sxs-lookup"><span data-stu-id="dd318-168">boolean</span></span>|<span data-ttu-id="dd318-169">Especifica se o fornecedor é responsável por impostos.</span><span class="sxs-lookup"><span data-stu-id="dd318-169">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="dd318-170">bloqueou</span><span class="sxs-lookup"><span data-stu-id="dd318-170">blocked</span></span>|<span data-ttu-id="dd318-171">string</span><span class="sxs-lookup"><span data-stu-id="dd318-171">string</span></span>|<span data-ttu-id="dd318-172">Especifica quais transações com o fornecedor que não podem ser lançados.</span><span class="sxs-lookup"><span data-stu-id="dd318-172">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="dd318-173">Os valores aceitos estão em branco, pagamento ou todos</span><span class="sxs-lookup"><span data-stu-id="dd318-173">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="dd318-174">carga</span><span class="sxs-lookup"><span data-stu-id="dd318-174">balance</span></span>|<span data-ttu-id="dd318-175">dígitos</span><span class="sxs-lookup"><span data-stu-id="dd318-175">decimal</span></span>|<span data-ttu-id="dd318-176">O saldo do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-176">The vendor's balance.</span></span> <span data-ttu-id="dd318-177">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="dd318-177">Read-Only.</span></span>|
|<span data-ttu-id="dd318-178">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd318-178">lastModifiedDateTime</span></span>|<span data-ttu-id="dd318-179">datetime</span><span class="sxs-lookup"><span data-stu-id="dd318-179">datetime</span></span>|<span data-ttu-id="dd318-180">O último DateTime que o fornecedor foi modificado.</span><span class="sxs-lookup"><span data-stu-id="dd318-180">The last datetime the vendor was modified.</span></span> <span data-ttu-id="dd318-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd318-181">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="dd318-182">Relações</span><span class="sxs-lookup"><span data-stu-id="dd318-182">Relationships</span></span>
<span data-ttu-id="dd318-183">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd318-183">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd318-184">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd318-184">JSON representation</span></span>

<span data-ttu-id="dd318-185">Veja a seguir uma representação JSON do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dd318-185">Here is a JSON representation of the vendor.</span></span>

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}

```

