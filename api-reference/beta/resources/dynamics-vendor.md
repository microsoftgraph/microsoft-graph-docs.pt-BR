---
title: tipo de recurso fornecedores
description: Um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1cec20dee4a124bb704d60ceb8229ea820aa55b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534854"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="ad775-103">tipo de recurso fornecedores</span><span class="sxs-lookup"><span data-stu-id="ad775-103">vendors resource type</span></span>
<span data-ttu-id="ad775-104">Representa um fornecedor no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="ad775-104">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="ad775-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ad775-105">Methods</span></span>

| <span data-ttu-id="ad775-106">Método</span><span class="sxs-lookup"><span data-stu-id="ad775-106">Method</span></span>       | <span data-ttu-id="ad775-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ad775-107">Return Type</span></span>  |<span data-ttu-id="ad775-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad775-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ad775-109">Obter fornecedores</span><span class="sxs-lookup"><span data-stu-id="ad775-109">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="ad775-110">fornecedor</span><span class="sxs-lookup"><span data-stu-id="ad775-110">vendors</span></span>|<span data-ttu-id="ad775-111">Obtém um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-111">Gets a vendor object.</span></span>|
|[<span data-ttu-id="ad775-112">Lançar fornecedores</span><span class="sxs-lookup"><span data-stu-id="ad775-112">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="ad775-113">fornecedor</span><span class="sxs-lookup"><span data-stu-id="ad775-113">vendors</span></span>|<span data-ttu-id="ad775-114">Cria um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-114">Creates a vendor object.</span></span>|
|[<span data-ttu-id="ad775-115">Fornecedores de patch</span><span class="sxs-lookup"><span data-stu-id="ad775-115">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="ad775-116">fornecedor</span><span class="sxs-lookup"><span data-stu-id="ad775-116">vendors</span></span>|<span data-ttu-id="ad775-117">Atualiza um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-117">Updates a vendor object.</span></span>|
|[<span data-ttu-id="ad775-118">Excluir fornecedor</span><span class="sxs-lookup"><span data-stu-id="ad775-118">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="ad775-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ad775-119">none</span></span>|<span data-ttu-id="ad775-120">Exclui um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-120">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ad775-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad775-121">Properties</span></span>
| <span data-ttu-id="ad775-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad775-122">Property</span></span>     | <span data-ttu-id="ad775-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad775-123">Type</span></span>   |<span data-ttu-id="ad775-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad775-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad775-125">id</span><span class="sxs-lookup"><span data-stu-id="ad775-125">id</span></span>|<span data-ttu-id="ad775-126">GUID</span><span class="sxs-lookup"><span data-stu-id="ad775-126">GUID</span></span>|<span data-ttu-id="ad775-127">A ID exclusiva do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-127">The unique ID of the vendor.</span></span> <span data-ttu-id="ad775-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="ad775-128">Non-editable.</span></span>|
|<span data-ttu-id="ad775-129">number</span><span class="sxs-lookup"><span data-stu-id="ad775-129">number</span></span>|<span data-ttu-id="ad775-130">string</span><span class="sxs-lookup"><span data-stu-id="ad775-130">string</span></span>|<span data-ttu-id="ad775-131">O número do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-131">The vendor number.</span></span>|
|<span data-ttu-id="ad775-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ad775-132">displayName</span></span>|<span data-ttu-id="ad775-133">string</span><span class="sxs-lookup"><span data-stu-id="ad775-133">string</span></span>|<span data-ttu-id="ad775-134">O nome de exibição do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-134">The vendor's display name.</span></span>|
|<span data-ttu-id="ad775-135">address</span><span class="sxs-lookup"><span data-stu-id="ad775-135">address</span></span>|[<span data-ttu-id="ad775-136">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="ad775-136">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="ad775-137">O endereço do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-137">The vendor's address.</span></span>|
|<span data-ttu-id="ad775-138">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ad775-138">phoneNumber</span></span>|<span data-ttu-id="ad775-139">string</span><span class="sxs-lookup"><span data-stu-id="ad775-139">string</span></span>|<span data-ttu-id="ad775-140">O número de telefone do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-140">The vendor's telephone number.</span></span>|
|<span data-ttu-id="ad775-141">email</span><span class="sxs-lookup"><span data-stu-id="ad775-141">email</span></span>|<span data-ttu-id="ad775-142">string</span><span class="sxs-lookup"><span data-stu-id="ad775-142">string</span></span>|<span data-ttu-id="ad775-143">O endereço de email do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-143">The vendor's email address.</span></span>|
|<span data-ttu-id="ad775-144">site</span><span class="sxs-lookup"><span data-stu-id="ad775-144">website</span></span>|<span data-ttu-id="ad775-145">string</span><span class="sxs-lookup"><span data-stu-id="ad775-145">string</span></span>|<span data-ttu-id="ad775-146">O endereço do site do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-146">The vendor's website address.</span></span>|
|<span data-ttu-id="ad775-147">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="ad775-147">taxRegistrationNumber</span></span>|<span data-ttu-id="ad775-148">string</span><span class="sxs-lookup"><span data-stu-id="ad775-148">string</span></span>|<span data-ttu-id="ad775-149">O número de registro de imposto do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-149">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="ad775-150">CurrencyID</span><span class="sxs-lookup"><span data-stu-id="ad775-150">currencyId</span></span>|<span data-ttu-id="ad775-151">GUID</span><span class="sxs-lookup"><span data-stu-id="ad775-151">GUID</span></span>|<span data-ttu-id="ad775-152">A ID do código de moeda padrão do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-152">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="ad775-153">currencyCode</span><span class="sxs-lookup"><span data-stu-id="ad775-153">currencyCode</span></span>|<span data-ttu-id="ad775-154">string</span><span class="sxs-lookup"><span data-stu-id="ad775-154">string</span></span>|<span data-ttu-id="ad775-155">O código de moeda padrão do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-155">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="ad775-156">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="ad775-156">irs1099Code</span></span>|<span data-ttu-id="ad775-157">string</span><span class="sxs-lookup"><span data-stu-id="ad775-157">string</span></span>|<span data-ttu-id="ad775-158">Especifica um código 1099 para o fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-158">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="ad775-159">Somente EUA.</span><span class="sxs-lookup"><span data-stu-id="ad775-159">US only.</span></span>|
|<span data-ttu-id="ad775-160">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="ad775-160">paymentTermsId</span></span>|<span data-ttu-id="ad775-161">GUID</span><span class="sxs-lookup"><span data-stu-id="ad775-161">GUID</span></span>|<span data-ttu-id="ad775-162">A ID padrão dos termos de pagamento do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-162">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="ad775-163">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="ad775-163">paymentMethodId</span></span>|<span data-ttu-id="ad775-164">GUID</span><span class="sxs-lookup"><span data-stu-id="ad775-164">GUID</span></span>|<span data-ttu-id="ad775-165">A ID de método de pagamento padrão para o fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-165">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="ad775-166">taxLiable</span><span class="sxs-lookup"><span data-stu-id="ad775-166">taxLiable</span></span>|<span data-ttu-id="ad775-167">booliano</span><span class="sxs-lookup"><span data-stu-id="ad775-167">boolean</span></span>|<span data-ttu-id="ad775-168">Especifica se o fornecedor é responsável por impostos.</span><span class="sxs-lookup"><span data-stu-id="ad775-168">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="ad775-169">bloqueou</span><span class="sxs-lookup"><span data-stu-id="ad775-169">blocked</span></span>|<span data-ttu-id="ad775-170">string</span><span class="sxs-lookup"><span data-stu-id="ad775-170">string</span></span>|<span data-ttu-id="ad775-171">Especifica quais transações com o fornecedor que não podem ser lançados.</span><span class="sxs-lookup"><span data-stu-id="ad775-171">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="ad775-172">Os valores aceitos estão em branco, pagamento ou todos</span><span class="sxs-lookup"><span data-stu-id="ad775-172">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="ad775-173">carga</span><span class="sxs-lookup"><span data-stu-id="ad775-173">balance</span></span>|<span data-ttu-id="ad775-174">dígitos</span><span class="sxs-lookup"><span data-stu-id="ad775-174">decimal</span></span>|<span data-ttu-id="ad775-175">O saldo do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-175">The vendor's balance.</span></span> <span data-ttu-id="ad775-176">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="ad775-176">Read-Only.</span></span>|
|<span data-ttu-id="ad775-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad775-177">lastModifiedDateTime</span></span>|<span data-ttu-id="ad775-178">DateTime</span><span class="sxs-lookup"><span data-stu-id="ad775-178">datetime</span></span>|<span data-ttu-id="ad775-179">O último DateTime que o fornecedor foi modificado.</span><span class="sxs-lookup"><span data-stu-id="ad775-179">The last datetime the vendor was modified.</span></span> <span data-ttu-id="ad775-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad775-180">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="ad775-181">Relações</span><span class="sxs-lookup"><span data-stu-id="ad775-181">Relationships</span></span>
<span data-ttu-id="ad775-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad775-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad775-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad775-183">JSON representation</span></span>

<span data-ttu-id="ad775-184">Veja a seguir uma representação JSON do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="ad775-184">Here is a JSON representation of the vendor.</span></span>

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

