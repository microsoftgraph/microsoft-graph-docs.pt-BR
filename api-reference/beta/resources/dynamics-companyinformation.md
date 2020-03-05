---
title: tipo de recurso companyInformation
description: Informações da empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ce982e7d03e4b2e5947381173d57706f6cf8f41e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505123"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="6c089-103">tipo de recurso companyInformation</span><span class="sxs-lookup"><span data-stu-id="6c089-103">companyInformation resource type</span></span>

<span data-ttu-id="6c089-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6c089-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c089-105">Representa as informações especificadas para a empresa atual no Dynamics 365 Business central, como nome, endereço, endereço de email e endereço do site.</span><span class="sxs-lookup"><span data-stu-id="6c089-105">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="6c089-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6c089-106">Methods</span></span>

| <span data-ttu-id="6c089-107">Método</span><span class="sxs-lookup"><span data-stu-id="6c089-107">Method</span></span>         | <span data-ttu-id="6c089-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6c089-108">Return Type</span></span>  |<span data-ttu-id="6c089-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c089-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="6c089-110">Obter companyInformation</span><span class="sxs-lookup"><span data-stu-id="6c089-110">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="6c089-111">companyInformation</span><span class="sxs-lookup"><span data-stu-id="6c089-111">companyInformation</span></span>|<span data-ttu-id="6c089-112">Obtém informações da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-112">Gets a company information.</span></span>|
|[<span data-ttu-id="6c089-113">Patch companyInformation</span><span class="sxs-lookup"><span data-stu-id="6c089-113">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="6c089-114">companyInformation</span><span class="sxs-lookup"><span data-stu-id="6c089-114">companyInformation</span></span>|<span data-ttu-id="6c089-115">Atualiza as informações da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-115">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="6c089-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c089-116">Properties</span></span>
| <span data-ttu-id="6c089-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c089-117">Property</span></span>     | <span data-ttu-id="6c089-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c089-118">Type</span></span>      |<span data-ttu-id="6c089-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c089-119">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="6c089-120">id</span><span class="sxs-lookup"><span data-stu-id="6c089-120">id</span></span>            |<span data-ttu-id="6c089-121">GUID</span><span class="sxs-lookup"><span data-stu-id="6c089-121">GUID</span></span>|<span data-ttu-id="6c089-122">A identificação exclusiva da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-122">The unique ID of the company.</span></span> <span data-ttu-id="6c089-123">Não editável.</span><span class="sxs-lookup"><span data-stu-id="6c089-123">Non-editable.</span></span>|
|<span data-ttu-id="6c089-124">displayName</span><span class="sxs-lookup"><span data-stu-id="6c089-124">displayName</span></span>   |<span data-ttu-id="6c089-125">string</span><span class="sxs-lookup"><span data-stu-id="6c089-125">string</span></span>   |<span data-ttu-id="6c089-126">O nome de exibição da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-126">The company's display name.</span></span>           |
|<span data-ttu-id="6c089-127">address</span><span class="sxs-lookup"><span data-stu-id="6c089-127">address</span></span>       |[<span data-ttu-id="6c089-128">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="6c089-128">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="6c089-129">O endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-129">The company's address.</span></span> <span data-ttu-id="6c089-130">Exiba o tipo complexo para obter detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="6c089-130">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="6c089-131">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="6c089-131">phoneNumber</span></span>   |<span data-ttu-id="6c089-132">string</span><span class="sxs-lookup"><span data-stu-id="6c089-132">string</span></span>   |<span data-ttu-id="6c089-133">O número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-133">The company's telephone number.</span></span>       |
|<span data-ttu-id="6c089-134">faxNumber</span><span class="sxs-lookup"><span data-stu-id="6c089-134">faxNumber</span></span>     |<span data-ttu-id="6c089-135">string</span><span class="sxs-lookup"><span data-stu-id="6c089-135">string</span></span>   |<span data-ttu-id="6c089-136">O número de fax da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-136">The company's fax number.</span></span>             |
|<span data-ttu-id="6c089-137">email</span><span class="sxs-lookup"><span data-stu-id="6c089-137">email</span></span>         |<span data-ttu-id="6c089-138">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c089-138">string</span></span>   |<span data-ttu-id="6c089-139">O endereço de email da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-139">The company's email address.</span></span>          |
|<span data-ttu-id="6c089-140">site</span><span class="sxs-lookup"><span data-stu-id="6c089-140">website</span></span>       |<span data-ttu-id="6c089-141">string</span><span class="sxs-lookup"><span data-stu-id="6c089-141">string</span></span>   |<span data-ttu-id="6c089-142">O endereço do site da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-142">The company's website address.</span></span>        |
|<span data-ttu-id="6c089-143">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="6c089-143">taxRegistrationNumber</span></span>|<span data-ttu-id="6c089-144">string</span><span class="sxs-lookup"><span data-stu-id="6c089-144">string</span></span>|<span data-ttu-id="6c089-145">O número de registro de imposto da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-145">The company's tax registration number.</span></span>|
|<span data-ttu-id="6c089-146">currencyCode</span><span class="sxs-lookup"><span data-stu-id="6c089-146">currencyCode</span></span>  |<span data-ttu-id="6c089-147">string</span><span class="sxs-lookup"><span data-stu-id="6c089-147">string</span></span>   |<span data-ttu-id="6c089-148">A moeda na qual a empresa faz negócios.</span><span class="sxs-lookup"><span data-stu-id="6c089-148">The currency the company does business in.</span></span> <span data-ttu-id="6c089-149">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="6c089-149">Read-Only.</span></span>|
|<span data-ttu-id="6c089-150">currentFiscalYearStartDate</span><span class="sxs-lookup"><span data-stu-id="6c089-150">currentFiscalYearStartDate</span></span>|<span data-ttu-id="6c089-151">data</span><span class="sxs-lookup"><span data-stu-id="6c089-151">date</span></span>|<span data-ttu-id="6c089-152">A data de início do ano fiscal atual da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-152">The company's current fiscal year start date.</span></span> <span data-ttu-id="6c089-153">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="6c089-153">Read-Only.</span></span>|
|<span data-ttu-id="6c089-154">indústria</span><span class="sxs-lookup"><span data-stu-id="6c089-154">industry</span></span>      |<span data-ttu-id="6c089-155">string</span><span class="sxs-lookup"><span data-stu-id="6c089-155">string</span></span>   |<span data-ttu-id="6c089-156">O setor do qual a empresa faz parte.</span><span class="sxs-lookup"><span data-stu-id="6c089-156">The industry the company is part of.</span></span>  |
|<span data-ttu-id="6c089-157">Panorama</span><span class="sxs-lookup"><span data-stu-id="6c089-157">picture</span></span>       |<span data-ttu-id="6c089-158">stream</span><span class="sxs-lookup"><span data-stu-id="6c089-158">stream</span></span>   |<span data-ttu-id="6c089-159">O logotipo da empresa.</span><span class="sxs-lookup"><span data-stu-id="6c089-159">The company logo.</span></span> <span data-ttu-id="6c089-160">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="6c089-160">Read-Only.</span></span>          |
|<span data-ttu-id="6c089-161">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="6c089-161">businessProfileId</span></span>|<span data-ttu-id="6c089-162">string</span><span class="sxs-lookup"><span data-stu-id="6c089-162">string</span></span>|<span data-ttu-id="6c089-163">A ID do perfil de negócios vinculada à empresa financeira.</span><span class="sxs-lookup"><span data-stu-id="6c089-163">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="6c089-164">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="6c089-164">Read-Only.</span></span>|
|<span data-ttu-id="6c089-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c089-165">lastModifiedDateTime</span></span>|<span data-ttu-id="6c089-166">datetime</span><span class="sxs-lookup"><span data-stu-id="6c089-166">datetime</span></span>|<span data-ttu-id="6c089-167">O último DateTime que a empresa foi modificada.</span><span class="sxs-lookup"><span data-stu-id="6c089-167">The last datetime the company was modified.</span></span> <span data-ttu-id="6c089-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6c089-168">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="6c089-169">Relações</span><span class="sxs-lookup"><span data-stu-id="6c089-169">Relationships</span></span>
<span data-ttu-id="6c089-170">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c089-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c089-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c089-171">JSON representation</span></span>

<span data-ttu-id="6c089-172">Veja a seguir uma representação JSON do companyInformation</span><span class="sxs-lookup"><span data-stu-id="6c089-172">Here is a JSON representation of the companyInformation</span></span>
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

