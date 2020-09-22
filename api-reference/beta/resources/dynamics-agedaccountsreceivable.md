---
title: tipo de recurso agedAccountsReceivable
description: Um objeto de contas a receber antiga no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 4d56e954e39bae22db07e025f9570f1fe7a92280
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040053"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="c0bb8-103">tipo de recurso agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="c0bb8-103">agedAccountsReceivable resource type</span></span>

<span data-ttu-id="c0bb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0bb8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0bb8-105">Representa um objeto agedAccountsReceivable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de cliente.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-105">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="c0bb8-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c0bb8-106">Methods</span></span>

| <span data-ttu-id="c0bb8-107">Método</span><span class="sxs-lookup"><span data-stu-id="c0bb8-107">Method</span></span>         | <span data-ttu-id="c0bb8-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c0bb8-108">Return Type</span></span>  |<span data-ttu-id="c0bb8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0bb8-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="c0bb8-110">Obter agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="c0bb8-110">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="c0bb8-111">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="c0bb8-111">agedAccountsReceivable</span></span>|<span data-ttu-id="c0bb8-112">Obter o objeto agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="c0bb8-112">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="c0bb8-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0bb8-113">Properties</span></span>
| <span data-ttu-id="c0bb8-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0bb8-114">Property</span></span>       | <span data-ttu-id="c0bb8-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0bb8-115">Type</span></span>    |<span data-ttu-id="c0bb8-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0bb8-116">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="c0bb8-117">Box</span><span class="sxs-lookup"><span data-stu-id="c0bb8-117">customerId</span></span>      |<span data-ttu-id="c0bb8-118">GUID</span><span class="sxs-lookup"><span data-stu-id="c0bb8-118">GUID</span></span>     |<span data-ttu-id="c0bb8-119">A ID exclusiva do cliente.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-119">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="c0bb8-120">customerNumber</span><span class="sxs-lookup"><span data-stu-id="c0bb8-120">customerNumber</span></span>  |<span data-ttu-id="c0bb8-121">string</span><span class="sxs-lookup"><span data-stu-id="c0bb8-121">string</span></span>   |<span data-ttu-id="c0bb8-122">Especifica o número do cliente.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-122">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="c0bb8-123">nome</span><span class="sxs-lookup"><span data-stu-id="c0bb8-123">name</span></span>            |<span data-ttu-id="c0bb8-124">string</span><span class="sxs-lookup"><span data-stu-id="c0bb8-124">string</span></span>   |<span data-ttu-id="c0bb8-125">Especifica o nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-125">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="c0bb8-126">currencyCode</span><span class="sxs-lookup"><span data-stu-id="c0bb8-126">currencyCode</span></span>    |<span data-ttu-id="c0bb8-127">string</span><span class="sxs-lookup"><span data-stu-id="c0bb8-127">string</span></span>   |<span data-ttu-id="c0bb8-128">Especifica a moeda.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-128">Specifies the currency.</span></span>                      |
|<span data-ttu-id="c0bb8-129">balanceDue</span><span class="sxs-lookup"><span data-stu-id="c0bb8-129">balanceDue</span></span>      |<span data-ttu-id="c0bb8-130">numéricos</span><span class="sxs-lookup"><span data-stu-id="c0bb8-130">numeric</span></span>  |<span data-ttu-id="c0bb8-131">Especifica o saldo total do cliente.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-131">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="c0bb8-132">currentAmount</span><span class="sxs-lookup"><span data-stu-id="c0bb8-132">currentAmount</span></span>   |<span data-ttu-id="c0bb8-133">numéricos</span><span class="sxs-lookup"><span data-stu-id="c0bb8-133">numeric</span></span>  |<span data-ttu-id="c0bb8-134">Especifica o saldo para o período de envelhecimento atual.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-134">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="c0bb8-135">period1Amount</span><span class="sxs-lookup"><span data-stu-id="c0bb8-135">period1Amount</span></span>   |<span data-ttu-id="c0bb8-136">numéricos</span><span class="sxs-lookup"><span data-stu-id="c0bb8-136">numeric</span></span>  |<span data-ttu-id="c0bb8-137">Especifica o saldo no primeiro período de classificação por vencimento.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-137">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="c0bb8-138">period2Amount</span><span class="sxs-lookup"><span data-stu-id="c0bb8-138">period2Amount</span></span>   |<span data-ttu-id="c0bb8-139">numéricos</span><span class="sxs-lookup"><span data-stu-id="c0bb8-139">numeric</span></span>  |<span data-ttu-id="c0bb8-140">Especifica o saldo no segundo período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-140">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="c0bb8-141">period3Amount</span><span class="sxs-lookup"><span data-stu-id="c0bb8-141">period3Amount</span></span>   |<span data-ttu-id="c0bb8-142">numéricos</span><span class="sxs-lookup"><span data-stu-id="c0bb8-142">numeric</span></span>  |<span data-ttu-id="c0bb8-143">Especifica o saldo no terceiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-143">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="c0bb8-144">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="c0bb8-144">agedAsOfDate</span></span>    |<span data-ttu-id="c0bb8-145">data</span><span class="sxs-lookup"><span data-stu-id="c0bb8-145">date</span></span>     |<span data-ttu-id="c0bb8-146">Especifica a data de início do período usada para calcular os períodos de expiração.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-146">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="c0bb8-147">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="c0bb8-147">periodLengthFilter</span></span>|<span data-ttu-id="c0bb8-148">string</span><span class="sxs-lookup"><span data-stu-id="c0bb8-148">string</span></span> |<span data-ttu-id="c0bb8-149">Especifica o comprimento dos períodos.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-149">Specifies the length of the periods.</span></span> <span data-ttu-id="c0bb8-150">As unidades de tempo aceitáveis incluem: D, WD, W, M, Q e Y. C, o que significa a unidade de tempo atual com base na data, pode ser especificada como um prefixo para a unidade de tempo.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-150">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c0bb8-151">Relações</span><span class="sxs-lookup"><span data-stu-id="c0bb8-151">Relationships</span></span>
<span data-ttu-id="c0bb8-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0bb8-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0bb8-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0bb8-153">JSON representation</span></span>

<span data-ttu-id="c0bb8-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0bb8-154">Here is a JSON representation of the resource.</span></span>


```json
{
    "customerId": "GUID",
    "customerNumber": "string",
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




