---
title: tipo de recurso agedAccountsPayable
description: Um objeto de contas a pagar antigo no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: dfbedf2e3f47d287842773d5da1c4e79ed126695
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058457"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="61068-103">tipo de recurso agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="61068-103">agedAccountsPayable resource type</span></span>

<span data-ttu-id="61068-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61068-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61068-105">Representa um objeto agedAccountsPayable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de fornecedor.</span><span class="sxs-lookup"><span data-stu-id="61068-105">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="61068-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="61068-106">Methods</span></span>

| <span data-ttu-id="61068-107">Método</span><span class="sxs-lookup"><span data-stu-id="61068-107">Method</span></span>         | <span data-ttu-id="61068-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="61068-108">Return Type</span></span>  |<span data-ttu-id="61068-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="61068-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="61068-110">Obter agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="61068-110">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="61068-111">agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="61068-111">agedAccountsPayable</span></span>|<span data-ttu-id="61068-112">Obter o objeto agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="61068-112">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="61068-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61068-113">Properties</span></span>
| <span data-ttu-id="61068-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61068-114">Property</span></span>      | <span data-ttu-id="61068-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="61068-115">Type</span></span>     |<span data-ttu-id="61068-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="61068-116">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="61068-117">VendorID</span><span class="sxs-lookup"><span data-stu-id="61068-117">vendorId</span></span>       |<span data-ttu-id="61068-118">GUID</span><span class="sxs-lookup"><span data-stu-id="61068-118">GUID</span></span>      |<span data-ttu-id="61068-119">A ID exclusiva do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="61068-119">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="61068-120">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="61068-120">vendorNumber</span></span>   |<span data-ttu-id="61068-121">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61068-121">string</span></span>    |<span data-ttu-id="61068-122">Especifica o número do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="61068-122">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="61068-123">name</span><span class="sxs-lookup"><span data-stu-id="61068-123">name</span></span>           |<span data-ttu-id="61068-124">string</span><span class="sxs-lookup"><span data-stu-id="61068-124">string</span></span>    |<span data-ttu-id="61068-125">Especifica o nome do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="61068-125">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="61068-126">currencyCode</span><span class="sxs-lookup"><span data-stu-id="61068-126">currencyCode</span></span>   |<span data-ttu-id="61068-127">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61068-127">string</span></span>    |<span data-ttu-id="61068-128">Especifica a moeda.</span><span class="sxs-lookup"><span data-stu-id="61068-128">Specifies the currency.</span></span>                     |
|<span data-ttu-id="61068-129">balanceDue</span><span class="sxs-lookup"><span data-stu-id="61068-129">balanceDue</span></span>     |<span data-ttu-id="61068-130">numéricos</span><span class="sxs-lookup"><span data-stu-id="61068-130">numeric</span></span>   |<span data-ttu-id="61068-131">Especifica o saldo total devido ao fornecedor.</span><span class="sxs-lookup"><span data-stu-id="61068-131">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="61068-132">currentAmount</span><span class="sxs-lookup"><span data-stu-id="61068-132">currentAmount</span></span>  |<span data-ttu-id="61068-133">numéricos</span><span class="sxs-lookup"><span data-stu-id="61068-133">numeric</span></span>   |<span data-ttu-id="61068-134">Especifica o saldo antes do primeiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="61068-134">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="61068-135">period1Amount</span><span class="sxs-lookup"><span data-stu-id="61068-135">period1Amount</span></span>  |<span data-ttu-id="61068-136">numéricos</span><span class="sxs-lookup"><span data-stu-id="61068-136">numeric</span></span>   |<span data-ttu-id="61068-137">Especifica o saldo no primeiro período de classificação por vencimento.</span><span class="sxs-lookup"><span data-stu-id="61068-137">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="61068-138">period2Amount</span><span class="sxs-lookup"><span data-stu-id="61068-138">period2Amount</span></span>  |<span data-ttu-id="61068-139">numéricos</span><span class="sxs-lookup"><span data-stu-id="61068-139">numeric</span></span>   |<span data-ttu-id="61068-140">Especifica o saldo no segundo período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="61068-140">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="61068-141">period3Amount</span><span class="sxs-lookup"><span data-stu-id="61068-141">period3Amount</span></span>  |<span data-ttu-id="61068-142">numéricos</span><span class="sxs-lookup"><span data-stu-id="61068-142">numeric</span></span>   |<span data-ttu-id="61068-143">Especifica o saldo no terceiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="61068-143">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="61068-144">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="61068-144">agedAsOfDate</span></span>   |<span data-ttu-id="61068-145">data</span><span class="sxs-lookup"><span data-stu-id="61068-145">date</span></span>|<span data-ttu-id="61068-146">Especifica a data de início do período usada para calcular os períodos de expiração.</span><span class="sxs-lookup"><span data-stu-id="61068-146">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="61068-147">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="61068-147">periodLengthFilter</span></span>|<span data-ttu-id="61068-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61068-148">string</span></span> |<span data-ttu-id="61068-149">Especifica o comprimento dos períodos.</span><span class="sxs-lookup"><span data-stu-id="61068-149">Specifies the length of the periods.</span></span> <span data-ttu-id="61068-150">Os valores aceitáveis para as unidades de tempo são: D, WD, W, M, Q ou Y. C, o que significa unidade de tempo atual com base na data, pode ser especificado como um prefixo para a unidade de tempo.</span><span class="sxs-lookup"><span data-stu-id="61068-150">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="61068-151">Relações</span><span class="sxs-lookup"><span data-stu-id="61068-151">Relationships</span></span>
<span data-ttu-id="61068-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61068-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61068-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61068-153">JSON representation</span></span>

<span data-ttu-id="61068-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61068-154">Here is a JSON representation of the resource.</span></span>


```json
{
    "vendorId": "GUID",
    "vendorNumber": "string",
    "name": "string",
    "currencyCode": "string",
    "balanceDue": "decimal",
    "currentAmount": "decimal",
    "period1Amount": "decimal",
    "period2Amount": "decimal",
    "period3Amount": "decimal",
    "agedAsOfDate": "date",
    "periodLengthFilter": "string"
}

```


