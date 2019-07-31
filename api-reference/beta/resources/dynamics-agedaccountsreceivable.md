---
title: tipo de recurso agedAccountsReceivable
description: Um objeto de contas a receber antiga no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: f9589cbb4cb380eececdcc7adf7bd5dd682269f6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012669"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="4ad56-103">tipo de recurso agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="4ad56-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="4ad56-104">Representa um objeto agedAccountsReceivable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de cliente.</span><span class="sxs-lookup"><span data-stu-id="4ad56-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="4ad56-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4ad56-105">Methods</span></span>

| <span data-ttu-id="4ad56-106">Método</span><span class="sxs-lookup"><span data-stu-id="4ad56-106">Method</span></span>         | <span data-ttu-id="4ad56-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4ad56-107">Return Type</span></span>  |<span data-ttu-id="4ad56-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ad56-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="4ad56-109">Obter agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="4ad56-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="4ad56-110">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="4ad56-110">agedAccountsReceivable</span></span>|<span data-ttu-id="4ad56-111">Obter o objeto agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="4ad56-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="4ad56-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ad56-112">Properties</span></span>
| <span data-ttu-id="4ad56-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ad56-113">Property</span></span>       | <span data-ttu-id="4ad56-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ad56-114">Type</span></span>    |<span data-ttu-id="4ad56-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ad56-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="4ad56-116">Box</span><span class="sxs-lookup"><span data-stu-id="4ad56-116">customerId</span></span>      |<span data-ttu-id="4ad56-117">GUID</span><span class="sxs-lookup"><span data-stu-id="4ad56-117">GUID</span></span>     |<span data-ttu-id="4ad56-118">A ID exclusiva do cliente.</span><span class="sxs-lookup"><span data-stu-id="4ad56-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="4ad56-119">customerNumber</span><span class="sxs-lookup"><span data-stu-id="4ad56-119">customerNumber</span></span>  |<span data-ttu-id="4ad56-120">string</span><span class="sxs-lookup"><span data-stu-id="4ad56-120">string</span></span>   |<span data-ttu-id="4ad56-121">Especifica o número do cliente.</span><span class="sxs-lookup"><span data-stu-id="4ad56-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="4ad56-122">name</span><span class="sxs-lookup"><span data-stu-id="4ad56-122">name</span></span>            |<span data-ttu-id="4ad56-123">string</span><span class="sxs-lookup"><span data-stu-id="4ad56-123">string</span></span>   |<span data-ttu-id="4ad56-124">Especifica o nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="4ad56-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="4ad56-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="4ad56-125">currencyCode</span></span>    |<span data-ttu-id="4ad56-126">string</span><span class="sxs-lookup"><span data-stu-id="4ad56-126">string</span></span>   |<span data-ttu-id="4ad56-127">Especifica a moeda.</span><span class="sxs-lookup"><span data-stu-id="4ad56-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="4ad56-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="4ad56-128">balanceDue</span></span>      |<span data-ttu-id="4ad56-129">numéricos</span><span class="sxs-lookup"><span data-stu-id="4ad56-129">numeric</span></span>  |<span data-ttu-id="4ad56-130">Especifica o saldo total do cliente.</span><span class="sxs-lookup"><span data-stu-id="4ad56-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="4ad56-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="4ad56-131">currentAmount</span></span>   |<span data-ttu-id="4ad56-132">numéricos</span><span class="sxs-lookup"><span data-stu-id="4ad56-132">numeric</span></span>  |<span data-ttu-id="4ad56-133">Especifica o saldo para o período de envelhecimento atual.</span><span class="sxs-lookup"><span data-stu-id="4ad56-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="4ad56-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="4ad56-134">period1Amount</span></span>   |<span data-ttu-id="4ad56-135">numéricos</span><span class="sxs-lookup"><span data-stu-id="4ad56-135">numeric</span></span>  |<span data-ttu-id="4ad56-136">Especifica o saldo no primeiro período de classificação por vencimento.</span><span class="sxs-lookup"><span data-stu-id="4ad56-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="4ad56-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="4ad56-137">period2Amount</span></span>   |<span data-ttu-id="4ad56-138">numéricos</span><span class="sxs-lookup"><span data-stu-id="4ad56-138">numeric</span></span>  |<span data-ttu-id="4ad56-139">Especifica o saldo no segundo período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="4ad56-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="4ad56-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="4ad56-140">period3Amount</span></span>   |<span data-ttu-id="4ad56-141">numéricos</span><span class="sxs-lookup"><span data-stu-id="4ad56-141">numeric</span></span>  |<span data-ttu-id="4ad56-142">Especifica o saldo no terceiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="4ad56-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="4ad56-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="4ad56-143">agedAsOfDate</span></span>    |<span data-ttu-id="4ad56-144">data</span><span class="sxs-lookup"><span data-stu-id="4ad56-144">date</span></span>     |<span data-ttu-id="4ad56-145">Especifica a data de início do período usada para calcular os períodos de expiração.</span><span class="sxs-lookup"><span data-stu-id="4ad56-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="4ad56-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="4ad56-146">periodLengthFilter</span></span>|<span data-ttu-id="4ad56-147">string</span><span class="sxs-lookup"><span data-stu-id="4ad56-147">string</span></span> |<span data-ttu-id="4ad56-148">Especifica o comprimento dos períodos.</span><span class="sxs-lookup"><span data-stu-id="4ad56-148">Specifies the length of the periods.</span></span> <span data-ttu-id="4ad56-149">As unidades de tempo aceitáveis incluem: D, WD, W, M, Q e Y. C, o que significa a unidade de tempo atual com base na data, pode ser especificada como um prefixo para a unidade de tempo.</span><span class="sxs-lookup"><span data-stu-id="4ad56-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="4ad56-150">Relações</span><span class="sxs-lookup"><span data-stu-id="4ad56-150">Relationships</span></span>
<span data-ttu-id="4ad56-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ad56-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ad56-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ad56-152">JSON representation</span></span>

<span data-ttu-id="4ad56-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ad56-153">Here is a JSON representation of the resource.</span></span>


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


