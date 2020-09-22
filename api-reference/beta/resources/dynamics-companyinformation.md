---
title: tipo de recurso companyInformation
description: Informações da empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 05a42bfb00cb56cd560151976bc8b7c7d6ed59ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081763"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="20e5b-103">tipo de recurso companyInformation</span><span class="sxs-lookup"><span data-stu-id="20e5b-103">companyInformation resource type</span></span>

<span data-ttu-id="20e5b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20e5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20e5b-105">Representa as informações especificadas para a empresa atual no Dynamics 365 Business central, como nome, endereço, endereço de email e endereço do site.</span><span class="sxs-lookup"><span data-stu-id="20e5b-105">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="20e5b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="20e5b-106">Methods</span></span>

| <span data-ttu-id="20e5b-107">Método</span><span class="sxs-lookup"><span data-stu-id="20e5b-107">Method</span></span>         | <span data-ttu-id="20e5b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="20e5b-108">Return Type</span></span>  |<span data-ttu-id="20e5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e5b-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="20e5b-110">Obter companyInformation</span><span class="sxs-lookup"><span data-stu-id="20e5b-110">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="20e5b-111">companyInformation</span><span class="sxs-lookup"><span data-stu-id="20e5b-111">companyInformation</span></span>|<span data-ttu-id="20e5b-112">Obtém informações da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-112">Gets a company information.</span></span>|
|[<span data-ttu-id="20e5b-113">Patch companyInformation</span><span class="sxs-lookup"><span data-stu-id="20e5b-113">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="20e5b-114">companyInformation</span><span class="sxs-lookup"><span data-stu-id="20e5b-114">companyInformation</span></span>|<span data-ttu-id="20e5b-115">Atualiza as informações da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-115">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="20e5b-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20e5b-116">Properties</span></span>
| <span data-ttu-id="20e5b-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20e5b-117">Property</span></span>     | <span data-ttu-id="20e5b-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="20e5b-118">Type</span></span>      |<span data-ttu-id="20e5b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="20e5b-119">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="20e5b-120">id</span><span class="sxs-lookup"><span data-stu-id="20e5b-120">id</span></span>            |<span data-ttu-id="20e5b-121">GUID</span><span class="sxs-lookup"><span data-stu-id="20e5b-121">GUID</span></span>|<span data-ttu-id="20e5b-122">A identificação exclusiva da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-122">The unique ID of the company.</span></span> <span data-ttu-id="20e5b-123">Não editável.</span><span class="sxs-lookup"><span data-stu-id="20e5b-123">Non-editable.</span></span>|
|<span data-ttu-id="20e5b-124">displayName</span><span class="sxs-lookup"><span data-stu-id="20e5b-124">displayName</span></span>   |<span data-ttu-id="20e5b-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-125">string</span></span>   |<span data-ttu-id="20e5b-126">O nome de exibição da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-126">The company's display name.</span></span>           |
|<span data-ttu-id="20e5b-127">address</span><span class="sxs-lookup"><span data-stu-id="20e5b-127">address</span></span>       |[<span data-ttu-id="20e5b-128">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="20e5b-128">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="20e5b-129">O endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-129">The company's address.</span></span> <span data-ttu-id="20e5b-130">Exiba o tipo complexo para obter detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="20e5b-130">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="20e5b-131">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="20e5b-131">phoneNumber</span></span>   |<span data-ttu-id="20e5b-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-132">string</span></span>   |<span data-ttu-id="20e5b-133">O número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-133">The company's telephone number.</span></span>       |
|<span data-ttu-id="20e5b-134">FaxNumber</span><span class="sxs-lookup"><span data-stu-id="20e5b-134">faxNumber</span></span>     |<span data-ttu-id="20e5b-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-135">string</span></span>   |<span data-ttu-id="20e5b-136">O número de fax da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-136">The company's fax number.</span></span>             |
|<span data-ttu-id="20e5b-137">email</span><span class="sxs-lookup"><span data-stu-id="20e5b-137">email</span></span>         |<span data-ttu-id="20e5b-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-138">string</span></span>   |<span data-ttu-id="20e5b-139">O endereço de email da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-139">The company's email address.</span></span>          |
|<span data-ttu-id="20e5b-140">site</span><span class="sxs-lookup"><span data-stu-id="20e5b-140">website</span></span>       |<span data-ttu-id="20e5b-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-141">string</span></span>   |<span data-ttu-id="20e5b-142">O endereço do site da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-142">The company's website address.</span></span>        |
|<span data-ttu-id="20e5b-143">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="20e5b-143">taxRegistrationNumber</span></span>|<span data-ttu-id="20e5b-144">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-144">string</span></span>|<span data-ttu-id="20e5b-145">O número de registro de imposto da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-145">The company's tax registration number.</span></span>|
|<span data-ttu-id="20e5b-146">currencyCode</span><span class="sxs-lookup"><span data-stu-id="20e5b-146">currencyCode</span></span>  |<span data-ttu-id="20e5b-147">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-147">string</span></span>   |<span data-ttu-id="20e5b-148">A moeda na qual a empresa faz negócios.</span><span class="sxs-lookup"><span data-stu-id="20e5b-148">The currency the company does business in.</span></span> <span data-ttu-id="20e5b-149">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="20e5b-149">Read-Only.</span></span>|
|<span data-ttu-id="20e5b-150">currentFiscalYearStartDate</span><span class="sxs-lookup"><span data-stu-id="20e5b-150">currentFiscalYearStartDate</span></span>|<span data-ttu-id="20e5b-151">data</span><span class="sxs-lookup"><span data-stu-id="20e5b-151">date</span></span>|<span data-ttu-id="20e5b-152">A data de início do ano fiscal atual da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-152">The company's current fiscal year start date.</span></span> <span data-ttu-id="20e5b-153">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="20e5b-153">Read-Only.</span></span>|
|<span data-ttu-id="20e5b-154">indústria</span><span class="sxs-lookup"><span data-stu-id="20e5b-154">industry</span></span>      |<span data-ttu-id="20e5b-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-155">string</span></span>   |<span data-ttu-id="20e5b-156">O setor do qual a empresa faz parte.</span><span class="sxs-lookup"><span data-stu-id="20e5b-156">The industry the company is part of.</span></span>  |
|<span data-ttu-id="20e5b-157">Panorama</span><span class="sxs-lookup"><span data-stu-id="20e5b-157">picture</span></span>       |<span data-ttu-id="20e5b-158">stream</span><span class="sxs-lookup"><span data-stu-id="20e5b-158">stream</span></span>   |<span data-ttu-id="20e5b-159">O logotipo da empresa.</span><span class="sxs-lookup"><span data-stu-id="20e5b-159">The company logo.</span></span> <span data-ttu-id="20e5b-160">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="20e5b-160">Read-Only.</span></span>          |
|<span data-ttu-id="20e5b-161">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="20e5b-161">businessProfileId</span></span>|<span data-ttu-id="20e5b-162">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="20e5b-162">string</span></span>|<span data-ttu-id="20e5b-163">A ID do perfil de negócios vinculada à empresa financeira.</span><span class="sxs-lookup"><span data-stu-id="20e5b-163">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="20e5b-164">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="20e5b-164">Read-Only.</span></span>|
|<span data-ttu-id="20e5b-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20e5b-165">lastModifiedDateTime</span></span>|<span data-ttu-id="20e5b-166">datetime</span><span class="sxs-lookup"><span data-stu-id="20e5b-166">datetime</span></span>|<span data-ttu-id="20e5b-167">O último DateTime que a empresa foi modificada.</span><span class="sxs-lookup"><span data-stu-id="20e5b-167">The last datetime the company was modified.</span></span> <span data-ttu-id="20e5b-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="20e5b-168">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="20e5b-169">Relações</span><span class="sxs-lookup"><span data-stu-id="20e5b-169">Relationships</span></span>
<span data-ttu-id="20e5b-170">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20e5b-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20e5b-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20e5b-171">JSON representation</span></span>

<span data-ttu-id="20e5b-172">Veja a seguir uma representação JSON do companyInformation</span><span class="sxs-lookup"><span data-stu-id="20e5b-172">Here is a JSON representation of the companyInformation</span></span>
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```



