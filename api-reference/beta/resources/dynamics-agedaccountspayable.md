---
title: tipo de recurso agedAccountsPayable
description: Um objeto de contas a pagar antigo no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 679c24b7ef32ef59b34a5885ea745d8c244376b2
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365903"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="07569-103">tipo de recurso agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="07569-103">agedAccountsPayable resource type</span></span>
<span data-ttu-id="07569-104">Representa um objeto agedAccountsPayable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de fornecedor.</span><span class="sxs-lookup"><span data-stu-id="07569-104">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="07569-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="07569-105">Methods</span></span>

| <span data-ttu-id="07569-106">Método</span><span class="sxs-lookup"><span data-stu-id="07569-106">Method</span></span>         | <span data-ttu-id="07569-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="07569-107">Return Type</span></span>  |<span data-ttu-id="07569-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="07569-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="07569-109">Obter agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="07569-109">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="07569-110">agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="07569-110">agedAccountsPayable</span></span>|<span data-ttu-id="07569-111">Obter o objeto agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="07569-111">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="07569-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07569-112">Properties</span></span>
| <span data-ttu-id="07569-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07569-113">Property</span></span>      | <span data-ttu-id="07569-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="07569-114">Type</span></span>     |<span data-ttu-id="07569-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="07569-115">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="07569-116">VendorID</span><span class="sxs-lookup"><span data-stu-id="07569-116">vendorId</span></span>       |<span data-ttu-id="07569-117">GUID</span><span class="sxs-lookup"><span data-stu-id="07569-117">GUID</span></span>      |<span data-ttu-id="07569-118">A ID exclusiva do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="07569-118">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="07569-119">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="07569-119">vendorNumber</span></span>   |<span data-ttu-id="07569-120">string</span><span class="sxs-lookup"><span data-stu-id="07569-120">string</span></span>    |<span data-ttu-id="07569-121">Especifica o número do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="07569-121">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="07569-122">name</span><span class="sxs-lookup"><span data-stu-id="07569-122">name</span></span>           |<span data-ttu-id="07569-123">string</span><span class="sxs-lookup"><span data-stu-id="07569-123">string</span></span>    |<span data-ttu-id="07569-124">Especifica o nome do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="07569-124">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="07569-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="07569-125">currencyCode</span></span>   |<span data-ttu-id="07569-126">string</span><span class="sxs-lookup"><span data-stu-id="07569-126">string</span></span>    |<span data-ttu-id="07569-127">Especifica a moeda.</span><span class="sxs-lookup"><span data-stu-id="07569-127">Specifies the currency.</span></span>                     |
|<span data-ttu-id="07569-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="07569-128">balanceDue</span></span>     |<span data-ttu-id="07569-129">numéricos</span><span class="sxs-lookup"><span data-stu-id="07569-129">numeric</span></span>   |<span data-ttu-id="07569-130">Especifica o saldo total devido ao fornecedor.</span><span class="sxs-lookup"><span data-stu-id="07569-130">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="07569-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="07569-131">currentAmount</span></span>  |<span data-ttu-id="07569-132">numéricos</span><span class="sxs-lookup"><span data-stu-id="07569-132">numeric</span></span>   |<span data-ttu-id="07569-133">Especifica o saldo antes do primeiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="07569-133">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="07569-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="07569-134">period1Amount</span></span>  |<span data-ttu-id="07569-135">numéricos</span><span class="sxs-lookup"><span data-stu-id="07569-135">numeric</span></span>   |<span data-ttu-id="07569-136">Especifica o saldo no primeiro período de classificação por vencimento.</span><span class="sxs-lookup"><span data-stu-id="07569-136">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="07569-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="07569-137">period2Amount</span></span>  |<span data-ttu-id="07569-138">numéricos</span><span class="sxs-lookup"><span data-stu-id="07569-138">numeric</span></span>   |<span data-ttu-id="07569-139">Especifica o saldo no segundo período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="07569-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="07569-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="07569-140">period3Amount</span></span>  |<span data-ttu-id="07569-141">numéricos</span><span class="sxs-lookup"><span data-stu-id="07569-141">numeric</span></span>   |<span data-ttu-id="07569-142">Especifica o saldo no terceiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="07569-142">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="07569-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="07569-143">agedAsOfDate</span></span>   |<span data-ttu-id="07569-144">data</span><span class="sxs-lookup"><span data-stu-id="07569-144">date</span></span>|<span data-ttu-id="07569-145">Especifica a data de início do período usada para calcular os períodos de expiração.</span><span class="sxs-lookup"><span data-stu-id="07569-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="07569-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="07569-146">periodLengthFilter</span></span>|<span data-ttu-id="07569-147">string</span><span class="sxs-lookup"><span data-stu-id="07569-147">string</span></span> |<span data-ttu-id="07569-148">Especifica o comprimento dos períodos.</span><span class="sxs-lookup"><span data-stu-id="07569-148">Specifies the length of the periods.</span></span> <span data-ttu-id="07569-149">Os valores aceitáveis para as unidades de tempo são: D, WD, W, M, Q ou Y. C, o que significa unidade de tempo atual com base na data, pode ser especificado como um prefixo para a unidade de tempo.</span><span class="sxs-lookup"><span data-stu-id="07569-149">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="07569-150">Relações</span><span class="sxs-lookup"><span data-stu-id="07569-150">Relationships</span></span>
<span data-ttu-id="07569-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07569-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07569-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07569-152">JSON representation</span></span>

<span data-ttu-id="07569-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07569-153">Here is a JSON representation of the resource.</span></span>


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
