---
title: tipo de recurso agedAccountsReceivable
description: Um objeto de contas a receber antiga no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365574"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="7be9b-103">tipo de recurso agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="7be9b-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="7be9b-104">Representa um objeto agedAccountsReceivable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de cliente.</span><span class="sxs-lookup"><span data-stu-id="7be9b-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="7be9b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7be9b-105">Methods</span></span>

| <span data-ttu-id="7be9b-106">Método</span><span class="sxs-lookup"><span data-stu-id="7be9b-106">Method</span></span>         | <span data-ttu-id="7be9b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7be9b-107">Return Type</span></span>  |<span data-ttu-id="7be9b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7be9b-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="7be9b-109">Obter agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="7be9b-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="7be9b-110">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="7be9b-110">agedAccountsReceivable</span></span>|<span data-ttu-id="7be9b-111">Obter o objeto agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="7be9b-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="7be9b-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7be9b-112">Properties</span></span>
| <span data-ttu-id="7be9b-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7be9b-113">Property</span></span>       | <span data-ttu-id="7be9b-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="7be9b-114">Type</span></span>    |<span data-ttu-id="7be9b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="7be9b-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="7be9b-116">customerId</span><span class="sxs-lookup"><span data-stu-id="7be9b-116">customerId</span></span>      |<span data-ttu-id="7be9b-117">GUID</span><span class="sxs-lookup"><span data-stu-id="7be9b-117">GUID</span></span>     |<span data-ttu-id="7be9b-118">A ID exclusiva do cliente.</span><span class="sxs-lookup"><span data-stu-id="7be9b-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="7be9b-119">customerNumber</span><span class="sxs-lookup"><span data-stu-id="7be9b-119">customerNumber</span></span>  |<span data-ttu-id="7be9b-120">string</span><span class="sxs-lookup"><span data-stu-id="7be9b-120">string</span></span>   |<span data-ttu-id="7be9b-121">Especifica o número do cliente.</span><span class="sxs-lookup"><span data-stu-id="7be9b-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="7be9b-122">name</span><span class="sxs-lookup"><span data-stu-id="7be9b-122">name</span></span>            |<span data-ttu-id="7be9b-123">string</span><span class="sxs-lookup"><span data-stu-id="7be9b-123">string</span></span>   |<span data-ttu-id="7be9b-124">Especifica o nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="7be9b-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="7be9b-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="7be9b-125">currencyCode</span></span>    |<span data-ttu-id="7be9b-126">string</span><span class="sxs-lookup"><span data-stu-id="7be9b-126">string</span></span>   |<span data-ttu-id="7be9b-127">Especifica a moeda.</span><span class="sxs-lookup"><span data-stu-id="7be9b-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="7be9b-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="7be9b-128">balanceDue</span></span>      |<span data-ttu-id="7be9b-129">numéricos</span><span class="sxs-lookup"><span data-stu-id="7be9b-129">numeric</span></span>  |<span data-ttu-id="7be9b-130">Especifica o saldo total do cliente.</span><span class="sxs-lookup"><span data-stu-id="7be9b-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="7be9b-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="7be9b-131">currentAmount</span></span>   |<span data-ttu-id="7be9b-132">numéricos</span><span class="sxs-lookup"><span data-stu-id="7be9b-132">numeric</span></span>  |<span data-ttu-id="7be9b-133">Especifica o saldo para o período de envelhecimento atual.</span><span class="sxs-lookup"><span data-stu-id="7be9b-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="7be9b-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="7be9b-134">period1Amount</span></span>   |<span data-ttu-id="7be9b-135">numéricos</span><span class="sxs-lookup"><span data-stu-id="7be9b-135">numeric</span></span>  |<span data-ttu-id="7be9b-136">Especifica o saldo no primeiro período de classificação por vencimento.</span><span class="sxs-lookup"><span data-stu-id="7be9b-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="7be9b-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="7be9b-137">period2Amount</span></span>   |<span data-ttu-id="7be9b-138">numéricos</span><span class="sxs-lookup"><span data-stu-id="7be9b-138">numeric</span></span>  |<span data-ttu-id="7be9b-139">Especifica o saldo no segundo período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="7be9b-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="7be9b-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="7be9b-140">period3Amount</span></span>   |<span data-ttu-id="7be9b-141">numéricos</span><span class="sxs-lookup"><span data-stu-id="7be9b-141">numeric</span></span>  |<span data-ttu-id="7be9b-142">Especifica o saldo no terceiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="7be9b-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="7be9b-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="7be9b-143">agedAsOfDate</span></span>    |<span data-ttu-id="7be9b-144">data</span><span class="sxs-lookup"><span data-stu-id="7be9b-144">date</span></span>     |<span data-ttu-id="7be9b-145">Especifica a data de início do período usada para calcular os períodos de expiração.</span><span class="sxs-lookup"><span data-stu-id="7be9b-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="7be9b-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="7be9b-146">periodLengthFilter</span></span>|<span data-ttu-id="7be9b-147">string</span><span class="sxs-lookup"><span data-stu-id="7be9b-147">string</span></span> |<span data-ttu-id="7be9b-148">Especifica o comprimento dos períodos.</span><span class="sxs-lookup"><span data-stu-id="7be9b-148">Specifies the length of the periods.</span></span> <span data-ttu-id="7be9b-149">As unidades de tempo aceitáveis incluem: D, WD, W, M, Q e Y. C, o que significa a unidade de tempo atual com base na data, pode ser especificada como um prefixo para a unidade de tempo.</span><span class="sxs-lookup"><span data-stu-id="7be9b-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7be9b-150">Relações</span><span class="sxs-lookup"><span data-stu-id="7be9b-150">Relationships</span></span>
<span data-ttu-id="7be9b-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7be9b-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7be9b-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7be9b-152">JSON representation</span></span>

<span data-ttu-id="7be9b-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7be9b-153">Here is a JSON representation of the resource.</span></span>


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


