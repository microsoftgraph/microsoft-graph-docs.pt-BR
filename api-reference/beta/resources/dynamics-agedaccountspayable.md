---
title: tipo de recurso agedAccountsPayable
description: Um objeto de contas a pagar antigo no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 9a8dc7eed4bdbcc39a04f55996e11b6d9dc6da1f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505165"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="dbac6-103">tipo de recurso agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="dbac6-103">agedAccountsPayable resource type</span></span>

<span data-ttu-id="dbac6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dbac6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbac6-105">Representa um objeto agedAccountsPayable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dbac6-105">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="dbac6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dbac6-106">Methods</span></span>

| <span data-ttu-id="dbac6-107">Método</span><span class="sxs-lookup"><span data-stu-id="dbac6-107">Method</span></span>         | <span data-ttu-id="dbac6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dbac6-108">Return Type</span></span>  |<span data-ttu-id="dbac6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbac6-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="dbac6-110">Obter agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="dbac6-110">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="dbac6-111">agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="dbac6-111">agedAccountsPayable</span></span>|<span data-ttu-id="dbac6-112">Obter o objeto agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="dbac6-112">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="dbac6-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbac6-113">Properties</span></span>
| <span data-ttu-id="dbac6-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbac6-114">Property</span></span>      | <span data-ttu-id="dbac6-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbac6-115">Type</span></span>     |<span data-ttu-id="dbac6-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbac6-116">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="dbac6-117">VendorID</span><span class="sxs-lookup"><span data-stu-id="dbac6-117">vendorId</span></span>       |<span data-ttu-id="dbac6-118">GUID</span><span class="sxs-lookup"><span data-stu-id="dbac6-118">GUID</span></span>      |<span data-ttu-id="dbac6-119">A ID exclusiva do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dbac6-119">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="dbac6-120">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="dbac6-120">vendorNumber</span></span>   |<span data-ttu-id="dbac6-121">string</span><span class="sxs-lookup"><span data-stu-id="dbac6-121">string</span></span>    |<span data-ttu-id="dbac6-122">Especifica o número do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dbac6-122">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="dbac6-123">nome</span><span class="sxs-lookup"><span data-stu-id="dbac6-123">name</span></span>           |<span data-ttu-id="dbac6-124">string</span><span class="sxs-lookup"><span data-stu-id="dbac6-124">string</span></span>    |<span data-ttu-id="dbac6-125">Especifica o nome do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dbac6-125">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="dbac6-126">currencyCode</span><span class="sxs-lookup"><span data-stu-id="dbac6-126">currencyCode</span></span>   |<span data-ttu-id="dbac6-127">string</span><span class="sxs-lookup"><span data-stu-id="dbac6-127">string</span></span>    |<span data-ttu-id="dbac6-128">Especifica a moeda.</span><span class="sxs-lookup"><span data-stu-id="dbac6-128">Specifies the currency.</span></span>                     |
|<span data-ttu-id="dbac6-129">balanceDue</span><span class="sxs-lookup"><span data-stu-id="dbac6-129">balanceDue</span></span>     |<span data-ttu-id="dbac6-130">numéricos</span><span class="sxs-lookup"><span data-stu-id="dbac6-130">numeric</span></span>   |<span data-ttu-id="dbac6-131">Especifica o saldo total devido ao fornecedor.</span><span class="sxs-lookup"><span data-stu-id="dbac6-131">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="dbac6-132">currentAmount</span><span class="sxs-lookup"><span data-stu-id="dbac6-132">currentAmount</span></span>  |<span data-ttu-id="dbac6-133">numéricos</span><span class="sxs-lookup"><span data-stu-id="dbac6-133">numeric</span></span>   |<span data-ttu-id="dbac6-134">Especifica o saldo antes do primeiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="dbac6-134">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="dbac6-135">period1Amount</span><span class="sxs-lookup"><span data-stu-id="dbac6-135">period1Amount</span></span>  |<span data-ttu-id="dbac6-136">numéricos</span><span class="sxs-lookup"><span data-stu-id="dbac6-136">numeric</span></span>   |<span data-ttu-id="dbac6-137">Especifica o saldo no primeiro período de classificação por vencimento.</span><span class="sxs-lookup"><span data-stu-id="dbac6-137">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="dbac6-138">period2Amount</span><span class="sxs-lookup"><span data-stu-id="dbac6-138">period2Amount</span></span>  |<span data-ttu-id="dbac6-139">numéricos</span><span class="sxs-lookup"><span data-stu-id="dbac6-139">numeric</span></span>   |<span data-ttu-id="dbac6-140">Especifica o saldo no segundo período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="dbac6-140">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="dbac6-141">period3Amount</span><span class="sxs-lookup"><span data-stu-id="dbac6-141">period3Amount</span></span>  |<span data-ttu-id="dbac6-142">numéricos</span><span class="sxs-lookup"><span data-stu-id="dbac6-142">numeric</span></span>   |<span data-ttu-id="dbac6-143">Especifica o saldo no terceiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="dbac6-143">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="dbac6-144">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="dbac6-144">agedAsOfDate</span></span>   |<span data-ttu-id="dbac6-145">data</span><span class="sxs-lookup"><span data-stu-id="dbac6-145">date</span></span>|<span data-ttu-id="dbac6-146">Especifica a data de início do período usada para calcular os períodos de expiração.</span><span class="sxs-lookup"><span data-stu-id="dbac6-146">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="dbac6-147">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="dbac6-147">periodLengthFilter</span></span>|<span data-ttu-id="dbac6-148">string</span><span class="sxs-lookup"><span data-stu-id="dbac6-148">string</span></span> |<span data-ttu-id="dbac6-149">Especifica o comprimento dos períodos.</span><span class="sxs-lookup"><span data-stu-id="dbac6-149">Specifies the length of the periods.</span></span> <span data-ttu-id="dbac6-150">Os valores aceitáveis para as unidades de tempo são: D, WD, W, M, Q ou Y. C, o que significa unidade de tempo atual com base na data, pode ser especificado como um prefixo para a unidade de tempo.</span><span class="sxs-lookup"><span data-stu-id="dbac6-150">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="dbac6-151">Relações</span><span class="sxs-lookup"><span data-stu-id="dbac6-151">Relationships</span></span>
<span data-ttu-id="dbac6-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dbac6-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbac6-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbac6-153">JSON representation</span></span>

<span data-ttu-id="dbac6-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbac6-154">Here is a JSON representation of the resource.</span></span>


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
