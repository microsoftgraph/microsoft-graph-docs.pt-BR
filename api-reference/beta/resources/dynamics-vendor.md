---
title: tipo de recurso fornecedores
description: Um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1cec20dee4a124bb704d60ceb8229ea820aa55b0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365658"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="4f23b-103">tipo de recurso fornecedores</span><span class="sxs-lookup"><span data-stu-id="4f23b-103">vendors resource type</span></span>
<span data-ttu-id="4f23b-104">Representa um fornecedor no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="4f23b-104">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="4f23b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4f23b-105">Methods</span></span>

| <span data-ttu-id="4f23b-106">Método</span><span class="sxs-lookup"><span data-stu-id="4f23b-106">Method</span></span>       | <span data-ttu-id="4f23b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4f23b-107">Return Type</span></span>  |<span data-ttu-id="4f23b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f23b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f23b-109">Obter fornecedores</span><span class="sxs-lookup"><span data-stu-id="4f23b-109">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="4f23b-110">fornecedor</span><span class="sxs-lookup"><span data-stu-id="4f23b-110">vendors</span></span>|<span data-ttu-id="4f23b-111">Obtém um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-111">Gets a vendor object.</span></span>|
|[<span data-ttu-id="4f23b-112">Lançar fornecedores</span><span class="sxs-lookup"><span data-stu-id="4f23b-112">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="4f23b-113">fornecedor</span><span class="sxs-lookup"><span data-stu-id="4f23b-113">vendors</span></span>|<span data-ttu-id="4f23b-114">Cria um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-114">Creates a vendor object.</span></span>|
|[<span data-ttu-id="4f23b-115">Fornecedores de patch</span><span class="sxs-lookup"><span data-stu-id="4f23b-115">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="4f23b-116">fornecedor</span><span class="sxs-lookup"><span data-stu-id="4f23b-116">vendors</span></span>|<span data-ttu-id="4f23b-117">Atualiza um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-117">Updates a vendor object.</span></span>|
|[<span data-ttu-id="4f23b-118">Excluir fornecedor</span><span class="sxs-lookup"><span data-stu-id="4f23b-118">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="4f23b-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4f23b-119">none</span></span>|<span data-ttu-id="4f23b-120">Exclui um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-120">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4f23b-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f23b-121">Properties</span></span>
| <span data-ttu-id="4f23b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f23b-122">Property</span></span>     | <span data-ttu-id="4f23b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f23b-123">Type</span></span>   |<span data-ttu-id="4f23b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f23b-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f23b-125">id</span><span class="sxs-lookup"><span data-stu-id="4f23b-125">id</span></span>|<span data-ttu-id="4f23b-126">GUID</span><span class="sxs-lookup"><span data-stu-id="4f23b-126">GUID</span></span>|<span data-ttu-id="4f23b-127">A ID exclusiva do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-127">The unique ID of the vendor.</span></span> <span data-ttu-id="4f23b-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="4f23b-128">Non-editable.</span></span>|
|<span data-ttu-id="4f23b-129">number</span><span class="sxs-lookup"><span data-stu-id="4f23b-129">number</span></span>|<span data-ttu-id="4f23b-130">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-130">string</span></span>|<span data-ttu-id="4f23b-131">O número do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-131">The vendor number.</span></span>|
|<span data-ttu-id="4f23b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4f23b-132">displayName</span></span>|<span data-ttu-id="4f23b-133">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-133">string</span></span>|<span data-ttu-id="4f23b-134">O nome de exibição do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-134">The vendor's display name.</span></span>|
|<span data-ttu-id="4f23b-135">address</span><span class="sxs-lookup"><span data-stu-id="4f23b-135">address</span></span>|[<span data-ttu-id="4f23b-136">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="4f23b-136">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="4f23b-137">O endereço do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-137">The vendor's address.</span></span>|
|<span data-ttu-id="4f23b-138">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="4f23b-138">phoneNumber</span></span>|<span data-ttu-id="4f23b-139">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-139">string</span></span>|<span data-ttu-id="4f23b-140">O número de telefone do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-140">The vendor's telephone number.</span></span>|
|<span data-ttu-id="4f23b-141">email</span><span class="sxs-lookup"><span data-stu-id="4f23b-141">email</span></span>|<span data-ttu-id="4f23b-142">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-142">string</span></span>|<span data-ttu-id="4f23b-143">O endereço de email do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-143">The vendor's email address.</span></span>|
|<span data-ttu-id="4f23b-144">site</span><span class="sxs-lookup"><span data-stu-id="4f23b-144">website</span></span>|<span data-ttu-id="4f23b-145">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-145">string</span></span>|<span data-ttu-id="4f23b-146">O endereço do site do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-146">The vendor's website address.</span></span>|
|<span data-ttu-id="4f23b-147">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="4f23b-147">taxRegistrationNumber</span></span>|<span data-ttu-id="4f23b-148">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-148">string</span></span>|<span data-ttu-id="4f23b-149">O número de registro de imposto do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-149">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="4f23b-150">CurrencyID</span><span class="sxs-lookup"><span data-stu-id="4f23b-150">currencyId</span></span>|<span data-ttu-id="4f23b-151">GUID</span><span class="sxs-lookup"><span data-stu-id="4f23b-151">GUID</span></span>|<span data-ttu-id="4f23b-152">A ID do código de moeda padrão do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-152">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="4f23b-153">currencyCode</span><span class="sxs-lookup"><span data-stu-id="4f23b-153">currencyCode</span></span>|<span data-ttu-id="4f23b-154">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-154">string</span></span>|<span data-ttu-id="4f23b-155">O código de moeda padrão do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-155">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="4f23b-156">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="4f23b-156">irs1099Code</span></span>|<span data-ttu-id="4f23b-157">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-157">string</span></span>|<span data-ttu-id="4f23b-158">Especifica um código 1099 para o fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-158">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="4f23b-159">Somente EUA.</span><span class="sxs-lookup"><span data-stu-id="4f23b-159">US only.</span></span>|
|<span data-ttu-id="4f23b-160">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="4f23b-160">paymentTermsId</span></span>|<span data-ttu-id="4f23b-161">GUID</span><span class="sxs-lookup"><span data-stu-id="4f23b-161">GUID</span></span>|<span data-ttu-id="4f23b-162">A ID padrão dos termos de pagamento do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-162">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="4f23b-163">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="4f23b-163">paymentMethodId</span></span>|<span data-ttu-id="4f23b-164">GUID</span><span class="sxs-lookup"><span data-stu-id="4f23b-164">GUID</span></span>|<span data-ttu-id="4f23b-165">A ID de método de pagamento padrão para o fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-165">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="4f23b-166">taxLiable</span><span class="sxs-lookup"><span data-stu-id="4f23b-166">taxLiable</span></span>|<span data-ttu-id="4f23b-167">boolean</span><span class="sxs-lookup"><span data-stu-id="4f23b-167">boolean</span></span>|<span data-ttu-id="4f23b-168">Especifica se o fornecedor é responsável por impostos.</span><span class="sxs-lookup"><span data-stu-id="4f23b-168">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="4f23b-169">bloqueou</span><span class="sxs-lookup"><span data-stu-id="4f23b-169">blocked</span></span>|<span data-ttu-id="4f23b-170">string</span><span class="sxs-lookup"><span data-stu-id="4f23b-170">string</span></span>|<span data-ttu-id="4f23b-171">Especifica quais transações com o fornecedor que não podem ser lançados.</span><span class="sxs-lookup"><span data-stu-id="4f23b-171">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="4f23b-172">Os valores aceitos estão em branco, pagamento ou todos</span><span class="sxs-lookup"><span data-stu-id="4f23b-172">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="4f23b-173">carga</span><span class="sxs-lookup"><span data-stu-id="4f23b-173">balance</span></span>|<span data-ttu-id="4f23b-174">dígitos</span><span class="sxs-lookup"><span data-stu-id="4f23b-174">decimal</span></span>|<span data-ttu-id="4f23b-175">O saldo do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-175">The vendor's balance.</span></span> <span data-ttu-id="4f23b-176">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="4f23b-176">Read-Only.</span></span>|
|<span data-ttu-id="4f23b-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f23b-177">lastModifiedDateTime</span></span>|<span data-ttu-id="4f23b-178">DateTime</span><span class="sxs-lookup"><span data-stu-id="4f23b-178">datetime</span></span>|<span data-ttu-id="4f23b-179">O último DateTime que o fornecedor foi modificado.</span><span class="sxs-lookup"><span data-stu-id="4f23b-179">The last datetime the vendor was modified.</span></span> <span data-ttu-id="4f23b-180">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="4f23b-180">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="4f23b-181">Relações</span><span class="sxs-lookup"><span data-stu-id="4f23b-181">Relationships</span></span>
<span data-ttu-id="4f23b-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4f23b-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f23b-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f23b-183">JSON representation</span></span>

<span data-ttu-id="4f23b-184">Veja a seguir uma representação JSON do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="4f23b-184">Here is a JSON representation of the vendor.</span></span>

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

