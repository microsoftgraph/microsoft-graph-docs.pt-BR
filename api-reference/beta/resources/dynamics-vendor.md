---
title: tipo de recurso fornecedores
description: Um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 7c0609d96f6d97503faf5c5251d3641979a4f6e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972849"
---
# <a name="vendors-resource-type"></a><span data-ttu-id="fb09a-103">tipo de recurso fornecedores</span><span class="sxs-lookup"><span data-stu-id="fb09a-103">vendors resource type</span></span>
<span data-ttu-id="fb09a-104">Representa um fornecedor no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="fb09a-104">Represents a vendor in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="fb09a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="fb09a-105">Methods</span></span>

| <span data-ttu-id="fb09a-106">Método</span><span class="sxs-lookup"><span data-stu-id="fb09a-106">Method</span></span>       | <span data-ttu-id="fb09a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fb09a-107">Return Type</span></span>  |<span data-ttu-id="fb09a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb09a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb09a-109">Obter fornecedores</span><span class="sxs-lookup"><span data-stu-id="fb09a-109">Get vendors</span></span>](../api/dynamics-vendor-get.md)|<span data-ttu-id="fb09a-110">fornecedor</span><span class="sxs-lookup"><span data-stu-id="fb09a-110">vendors</span></span>|<span data-ttu-id="fb09a-111">Obtém um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-111">Gets a vendor object.</span></span>|
|[<span data-ttu-id="fb09a-112">Lançar fornecedores</span><span class="sxs-lookup"><span data-stu-id="fb09a-112">Post vendors</span></span>](../api/dynamics-create-vendor.md)|<span data-ttu-id="fb09a-113">fornecedor</span><span class="sxs-lookup"><span data-stu-id="fb09a-113">vendors</span></span>|<span data-ttu-id="fb09a-114">Cria um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-114">Creates a vendor object.</span></span>|
|[<span data-ttu-id="fb09a-115">Fornecedores de patch</span><span class="sxs-lookup"><span data-stu-id="fb09a-115">Patch vendors</span></span>](../api/dynamics-vendor-update.md)|<span data-ttu-id="fb09a-116">fornecedor</span><span class="sxs-lookup"><span data-stu-id="fb09a-116">vendors</span></span>|<span data-ttu-id="fb09a-117">Atualiza um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-117">Updates a vendor object.</span></span>|
|[<span data-ttu-id="fb09a-118">Excluir fornecedor</span><span class="sxs-lookup"><span data-stu-id="fb09a-118">Delete vendor</span></span>](../api/dynamics-vendor-delete.md)|<span data-ttu-id="fb09a-119">none</span><span class="sxs-lookup"><span data-stu-id="fb09a-119">none</span></span>|<span data-ttu-id="fb09a-120">Exclui um objeto fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-120">Deletes a vendor object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fb09a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb09a-121">Properties</span></span>
| <span data-ttu-id="fb09a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb09a-122">Property</span></span>     | <span data-ttu-id="fb09a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb09a-123">Type</span></span>   |<span data-ttu-id="fb09a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb09a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb09a-125">id</span><span class="sxs-lookup"><span data-stu-id="fb09a-125">id</span></span>|<span data-ttu-id="fb09a-126">GUID</span><span class="sxs-lookup"><span data-stu-id="fb09a-126">GUID</span></span>|<span data-ttu-id="fb09a-127">A ID exclusiva do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-127">The unique ID of the vendor.</span></span> <span data-ttu-id="fb09a-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="fb09a-128">Non-editable.</span></span>|
|<span data-ttu-id="fb09a-129">number</span><span class="sxs-lookup"><span data-stu-id="fb09a-129">number</span></span>|<span data-ttu-id="fb09a-130">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-130">string</span></span>|<span data-ttu-id="fb09a-131">O número do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-131">The vendor number.</span></span>|
|<span data-ttu-id="fb09a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="fb09a-132">displayName</span></span>|<span data-ttu-id="fb09a-133">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-133">string</span></span>|<span data-ttu-id="fb09a-134">O nome de exibição do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-134">The vendor's display name.</span></span>|
|<span data-ttu-id="fb09a-135">address</span><span class="sxs-lookup"><span data-stu-id="fb09a-135">address</span></span>|[<span data-ttu-id="fb09a-136">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="fb09a-136">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="fb09a-137">O endereço do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-137">The vendor's address.</span></span>|
|<span data-ttu-id="fb09a-138">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="fb09a-138">phoneNumber</span></span>|<span data-ttu-id="fb09a-139">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-139">string</span></span>|<span data-ttu-id="fb09a-140">O número de telefone do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-140">The vendor's telephone number.</span></span>|
|<span data-ttu-id="fb09a-141">email</span><span class="sxs-lookup"><span data-stu-id="fb09a-141">email</span></span>|<span data-ttu-id="fb09a-142">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-142">string</span></span>|<span data-ttu-id="fb09a-143">O endereço de email do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-143">The vendor's email address.</span></span>|
|<span data-ttu-id="fb09a-144">site</span><span class="sxs-lookup"><span data-stu-id="fb09a-144">website</span></span>|<span data-ttu-id="fb09a-145">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-145">string</span></span>|<span data-ttu-id="fb09a-146">O endereço do site do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-146">The vendor's website address.</span></span>|
|<span data-ttu-id="fb09a-147">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="fb09a-147">taxRegistrationNumber</span></span>|<span data-ttu-id="fb09a-148">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-148">string</span></span>|<span data-ttu-id="fb09a-149">O número de registro de imposto do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-149">The vendor's tax registration number.</span></span>|
|<span data-ttu-id="fb09a-150">CurrencyID</span><span class="sxs-lookup"><span data-stu-id="fb09a-150">currencyId</span></span>|<span data-ttu-id="fb09a-151">GUID</span><span class="sxs-lookup"><span data-stu-id="fb09a-151">GUID</span></span>|<span data-ttu-id="fb09a-152">A ID do código de moeda padrão do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-152">The default currency code ID for the vendor.</span></span>|
|<span data-ttu-id="fb09a-153">currencyCode</span><span class="sxs-lookup"><span data-stu-id="fb09a-153">currencyCode</span></span>|<span data-ttu-id="fb09a-154">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-154">string</span></span>|<span data-ttu-id="fb09a-155">O código de moeda padrão do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-155">The default currency code for the vendor.</span></span>|
|<span data-ttu-id="fb09a-156">irs1099Code</span><span class="sxs-lookup"><span data-stu-id="fb09a-156">irs1099Code</span></span>|<span data-ttu-id="fb09a-157">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-157">string</span></span>|<span data-ttu-id="fb09a-158">Especifica um código 1099 para o fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-158">Specifies a 1099 code for the vendor.</span></span> <span data-ttu-id="fb09a-159">Somente EUA.</span><span class="sxs-lookup"><span data-stu-id="fb09a-159">US only.</span></span>|
|<span data-ttu-id="fb09a-160">paymentTermsId</span><span class="sxs-lookup"><span data-stu-id="fb09a-160">paymentTermsId</span></span>|<span data-ttu-id="fb09a-161">GUID</span><span class="sxs-lookup"><span data-stu-id="fb09a-161">GUID</span></span>|<span data-ttu-id="fb09a-162">A ID padrão dos termos de pagamento do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-162">The default payment terms ID for the vendor.</span></span>|
|<span data-ttu-id="fb09a-163">paymentMethodId</span><span class="sxs-lookup"><span data-stu-id="fb09a-163">paymentMethodId</span></span>|<span data-ttu-id="fb09a-164">GUID</span><span class="sxs-lookup"><span data-stu-id="fb09a-164">GUID</span></span>|<span data-ttu-id="fb09a-165">A ID de método de pagamento padrão para o fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-165">The default payment method ID for the vendor.</span></span>|
|<span data-ttu-id="fb09a-166">taxLiable</span><span class="sxs-lookup"><span data-stu-id="fb09a-166">taxLiable</span></span>|<span data-ttu-id="fb09a-167">booliano</span><span class="sxs-lookup"><span data-stu-id="fb09a-167">boolean</span></span>|<span data-ttu-id="fb09a-168">Especifica se o fornecedor é responsável por impostos.</span><span class="sxs-lookup"><span data-stu-id="fb09a-168">Specifies if the vendor is liable for tax.</span></span>|
|<span data-ttu-id="fb09a-169">bloqueou</span><span class="sxs-lookup"><span data-stu-id="fb09a-169">blocked</span></span>|<span data-ttu-id="fb09a-170">string</span><span class="sxs-lookup"><span data-stu-id="fb09a-170">string</span></span>|<span data-ttu-id="fb09a-171">Especifica quais transações com o fornecedor que não podem ser lançados.</span><span class="sxs-lookup"><span data-stu-id="fb09a-171">Specifies which transactions with the vendor that cannot be posted.</span></span> <span data-ttu-id="fb09a-172">Os valores aceitos estão em branco, pagamento ou todos</span><span class="sxs-lookup"><span data-stu-id="fb09a-172">Accepted values are blank, Payment or All</span></span>|
|<span data-ttu-id="fb09a-173">carga</span><span class="sxs-lookup"><span data-stu-id="fb09a-173">balance</span></span>|<span data-ttu-id="fb09a-174">dígitos</span><span class="sxs-lookup"><span data-stu-id="fb09a-174">decimal</span></span>|<span data-ttu-id="fb09a-175">O saldo do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-175">The vendor's balance.</span></span> <span data-ttu-id="fb09a-176">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="fb09a-176">Read-Only.</span></span>|
|<span data-ttu-id="fb09a-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb09a-177">lastModifiedDateTime</span></span>|<span data-ttu-id="fb09a-178">DateTime</span><span class="sxs-lookup"><span data-stu-id="fb09a-178">datetime</span></span>|<span data-ttu-id="fb09a-179">O último DateTime que o fornecedor foi modificado.</span><span class="sxs-lookup"><span data-stu-id="fb09a-179">The last datetime the vendor was modified.</span></span> <span data-ttu-id="fb09a-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fb09a-180">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="fb09a-181">Relações</span><span class="sxs-lookup"><span data-stu-id="fb09a-181">Relationships</span></span>
<span data-ttu-id="fb09a-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb09a-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb09a-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb09a-183">JSON representation</span></span>

<span data-ttu-id="fb09a-184">Veja a seguir uma representação JSON do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="fb09a-184">Here is a JSON representation of the vendor.</span></span>

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

