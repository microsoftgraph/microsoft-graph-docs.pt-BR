---
title: tipo de recurso companyInformation
description: Informações da empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0f8671cbade11cc9db6bf797c39eb17acf286ef7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507270"
---
# <a name="companyinformation-resource-type"></a><span data-ttu-id="1b8a2-103">tipo de recurso companyInformation</span><span class="sxs-lookup"><span data-stu-id="1b8a2-103">companyInformation resource type</span></span>
<span data-ttu-id="1b8a2-104">Representa as informações especificadas para a empresa atual no Dynamics 365 Business central, como nome, endereço, endereço de email e endereço do site.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-104">Represents the information specified for the current company in Dynamics 365 Business Central, such as name, address, email address, and website address.</span></span>

## <a name="methods"></a><span data-ttu-id="1b8a2-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b8a2-105">Methods</span></span>

| <span data-ttu-id="1b8a2-106">Método</span><span class="sxs-lookup"><span data-stu-id="1b8a2-106">Method</span></span>         | <span data-ttu-id="1b8a2-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b8a2-107">Return Type</span></span>  |<span data-ttu-id="1b8a2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b8a2-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="1b8a2-109">Obter companyInformation</span><span class="sxs-lookup"><span data-stu-id="1b8a2-109">Get companyInformation</span></span>](../api/dynamics-companyinformation-get.md)|<span data-ttu-id="1b8a2-110">companyInformation</span><span class="sxs-lookup"><span data-stu-id="1b8a2-110">companyInformation</span></span>|<span data-ttu-id="1b8a2-111">Obtém informações da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-111">Gets a company information.</span></span>|
|[<span data-ttu-id="1b8a2-112">Patch companyInformation</span><span class="sxs-lookup"><span data-stu-id="1b8a2-112">Patch companyInformation</span></span>](../api/dynamics-companyinformation-update.md)|<span data-ttu-id="1b8a2-113">companyInformation</span><span class="sxs-lookup"><span data-stu-id="1b8a2-113">companyInformation</span></span>|<span data-ttu-id="1b8a2-114">Atualiza as informações da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-114">Updates a company information.</span></span>|


## <a name="properties"></a><span data-ttu-id="1b8a2-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b8a2-115">Properties</span></span>
| <span data-ttu-id="1b8a2-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b8a2-116">Property</span></span>     | <span data-ttu-id="1b8a2-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b8a2-117">Type</span></span>      |<span data-ttu-id="1b8a2-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b8a2-118">Description</span></span>                           |
|:-------------|:--------|:-------------------------------------|
|<span data-ttu-id="1b8a2-119">id</span><span class="sxs-lookup"><span data-stu-id="1b8a2-119">id</span></span>            |<span data-ttu-id="1b8a2-120">GUID</span><span class="sxs-lookup"><span data-stu-id="1b8a2-120">GUID</span></span>|<span data-ttu-id="1b8a2-121">A identificação exclusiva da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-121">The unique ID of the company.</span></span> <span data-ttu-id="1b8a2-122">Não editável.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-122">Non-editable.</span></span>|
|<span data-ttu-id="1b8a2-123">displayName</span><span class="sxs-lookup"><span data-stu-id="1b8a2-123">displayName</span></span>   |<span data-ttu-id="1b8a2-124">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-124">string</span></span>   |<span data-ttu-id="1b8a2-125">O nome de exibição da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-125">The company's display name.</span></span>           |
|<span data-ttu-id="1b8a2-126">address</span><span class="sxs-lookup"><span data-stu-id="1b8a2-126">address</span></span>       |[<span data-ttu-id="1b8a2-127">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="1b8a2-127">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="1b8a2-128">O endereço da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-128">The company's address.</span></span> <span data-ttu-id="1b8a2-129">Exiba o tipo complexo para obter detalhes adicionais.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-129">View the complex type for additional detail.</span></span>|
|<span data-ttu-id="1b8a2-130">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="1b8a2-130">phoneNumber</span></span>   |<span data-ttu-id="1b8a2-131">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-131">string</span></span>   |<span data-ttu-id="1b8a2-132">O número de telefone da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-132">The company's telephone number.</span></span>       |
|<span data-ttu-id="1b8a2-133">FaxNumber</span><span class="sxs-lookup"><span data-stu-id="1b8a2-133">faxNumber</span></span>     |<span data-ttu-id="1b8a2-134">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-134">string</span></span>   |<span data-ttu-id="1b8a2-135">O número de fax da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-135">The company's fax number.</span></span>             |
|<span data-ttu-id="1b8a2-136">email</span><span class="sxs-lookup"><span data-stu-id="1b8a2-136">email</span></span>         |<span data-ttu-id="1b8a2-137">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-137">string</span></span>   |<span data-ttu-id="1b8a2-138">O endereço de email da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-138">The company's email address.</span></span>          |
|<span data-ttu-id="1b8a2-139">site</span><span class="sxs-lookup"><span data-stu-id="1b8a2-139">website</span></span>       |<span data-ttu-id="1b8a2-140">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-140">string</span></span>   |<span data-ttu-id="1b8a2-141">O endereço do site da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-141">The company's website address.</span></span>        |
|<span data-ttu-id="1b8a2-142">taxRegistrationNumber</span><span class="sxs-lookup"><span data-stu-id="1b8a2-142">taxRegistrationNumber</span></span>|<span data-ttu-id="1b8a2-143">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-143">string</span></span>|<span data-ttu-id="1b8a2-144">O número de registro de imposto da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-144">The company's tax registration number.</span></span>|
|<span data-ttu-id="1b8a2-145">currencyCode</span><span class="sxs-lookup"><span data-stu-id="1b8a2-145">currencyCode</span></span>  |<span data-ttu-id="1b8a2-146">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-146">string</span></span>   |<span data-ttu-id="1b8a2-147">A moeda na qual a empresa faz negócios.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-147">The currency the company does business in.</span></span> <span data-ttu-id="1b8a2-148">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-148">Read-Only.</span></span>|
|<span data-ttu-id="1b8a2-149">currentFiscalYearStartDate</span><span class="sxs-lookup"><span data-stu-id="1b8a2-149">currentFiscalYearStartDate</span></span>|<span data-ttu-id="1b8a2-150">data</span><span class="sxs-lookup"><span data-stu-id="1b8a2-150">date</span></span>|<span data-ttu-id="1b8a2-151">A data de início do ano fiscal atual da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-151">The company's current fiscal year start date.</span></span> <span data-ttu-id="1b8a2-152">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-152">Read-Only.</span></span>|
|<span data-ttu-id="1b8a2-153">indústria</span><span class="sxs-lookup"><span data-stu-id="1b8a2-153">industry</span></span>      |<span data-ttu-id="1b8a2-154">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-154">string</span></span>   |<span data-ttu-id="1b8a2-155">O setor do qual a empresa faz parte.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-155">The industry the company is part of.</span></span>  |
|<span data-ttu-id="1b8a2-156">Panorama</span><span class="sxs-lookup"><span data-stu-id="1b8a2-156">picture</span></span>       |<span data-ttu-id="1b8a2-157">stream</span><span class="sxs-lookup"><span data-stu-id="1b8a2-157">stream</span></span>   |<span data-ttu-id="1b8a2-158">O logotipo da empresa.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-158">The company logo.</span></span> <span data-ttu-id="1b8a2-159">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-159">Read-Only.</span></span>          |
|<span data-ttu-id="1b8a2-160">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="1b8a2-160">businessProfileId</span></span>|<span data-ttu-id="1b8a2-161">string</span><span class="sxs-lookup"><span data-stu-id="1b8a2-161">string</span></span>|<span data-ttu-id="1b8a2-162">A ID do perfil de negócios vinculada à empresa financeira.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-162">The business profile ID linked to the Financials company.</span></span> <span data-ttu-id="1b8a2-163">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-163">Read-Only.</span></span>|
|<span data-ttu-id="1b8a2-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b8a2-164">lastModifiedDateTime</span></span>|<span data-ttu-id="1b8a2-165">DateTime</span><span class="sxs-lookup"><span data-stu-id="1b8a2-165">datetime</span></span>|<span data-ttu-id="1b8a2-166">O último DateTime que a empresa foi modificada.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-166">The last datetime the company was modified.</span></span> <span data-ttu-id="1b8a2-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b8a2-167">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="1b8a2-168">Relações</span><span class="sxs-lookup"><span data-stu-id="1b8a2-168">Relationships</span></span>
<span data-ttu-id="1b8a2-169">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1b8a2-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b8a2-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b8a2-170">JSON representation</span></span>

<span data-ttu-id="1b8a2-171">Veja a seguir uma representação JSON do companyInformation</span><span class="sxs-lookup"><span data-stu-id="1b8a2-171">Here is a JSON representation of the companyInformation</span></span>
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

