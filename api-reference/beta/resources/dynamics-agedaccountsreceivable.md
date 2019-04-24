---
title: tipo de recurso agedAccountsReceivable
description: Um objeto de contas a receber antiga no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ce5d010c08f956468398082821040e30b4ef2ace
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507613"
---
# <a name="agedaccountsreceivable-resource-type"></a><span data-ttu-id="68768-103">tipo de recurso agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="68768-103">agedAccountsReceivable resource type</span></span>
<span data-ttu-id="68768-104">Representa um objeto agedAccountsReceivable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de cliente.</span><span class="sxs-lookup"><span data-stu-id="68768-104">Represents an agedAccountsReceivable object in Dynamics 365 Business Central, which is showing the aging of a customer account.</span></span>

## <a name="methods"></a><span data-ttu-id="68768-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="68768-105">Methods</span></span>

| <span data-ttu-id="68768-106">Método</span><span class="sxs-lookup"><span data-stu-id="68768-106">Method</span></span>         | <span data-ttu-id="68768-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="68768-107">Return Type</span></span>  |<span data-ttu-id="68768-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="68768-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="68768-109">Obter agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="68768-109">Get agedAccountsReceivable</span></span>](../api/dynamics-agedaccountsreceivable-get.md)|<span data-ttu-id="68768-110">agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="68768-110">agedAccountsReceivable</span></span>|<span data-ttu-id="68768-111">Obter o objeto agedAccountsReceivable</span><span class="sxs-lookup"><span data-stu-id="68768-111">Get agedAccountsReceivable object</span></span>|

## <a name="properties"></a><span data-ttu-id="68768-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68768-112">Properties</span></span>
| <span data-ttu-id="68768-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68768-113">Property</span></span>       | <span data-ttu-id="68768-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="68768-114">Type</span></span>    |<span data-ttu-id="68768-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="68768-115">Description</span></span>                                  |
|:---------------|:--------|:--------------------------------------------|
|<span data-ttu-id="68768-116">Box</span><span class="sxs-lookup"><span data-stu-id="68768-116">customerId</span></span>      |<span data-ttu-id="68768-117">GUID</span><span class="sxs-lookup"><span data-stu-id="68768-117">GUID</span></span>     |<span data-ttu-id="68768-118">A ID exclusiva do cliente.</span><span class="sxs-lookup"><span data-stu-id="68768-118">The unique ID of customer.</span></span>                   |
|<span data-ttu-id="68768-119">customerNumber</span><span class="sxs-lookup"><span data-stu-id="68768-119">customerNumber</span></span>  |<span data-ttu-id="68768-120">string</span><span class="sxs-lookup"><span data-stu-id="68768-120">string</span></span>   |<span data-ttu-id="68768-121">Especifica o número do cliente.</span><span class="sxs-lookup"><span data-stu-id="68768-121">Specifies customer's number.</span></span>                 |
|<span data-ttu-id="68768-122">nome</span><span class="sxs-lookup"><span data-stu-id="68768-122">name</span></span>            |<span data-ttu-id="68768-123">string</span><span class="sxs-lookup"><span data-stu-id="68768-123">string</span></span>   |<span data-ttu-id="68768-124">Especifica o nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="68768-124">Specifies customer's name.</span></span>                   |
|<span data-ttu-id="68768-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="68768-125">currencyCode</span></span>    |<span data-ttu-id="68768-126">string</span><span class="sxs-lookup"><span data-stu-id="68768-126">string</span></span>   |<span data-ttu-id="68768-127">Especifica a moeda.</span><span class="sxs-lookup"><span data-stu-id="68768-127">Specifies the currency.</span></span>                      |
|<span data-ttu-id="68768-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="68768-128">balanceDue</span></span>      |<span data-ttu-id="68768-129">numéricos</span><span class="sxs-lookup"><span data-stu-id="68768-129">numeric</span></span>  |<span data-ttu-id="68768-130">Especifica o saldo total do cliente.</span><span class="sxs-lookup"><span data-stu-id="68768-130">Specifies the customer's total balance.</span></span>      |
|<span data-ttu-id="68768-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="68768-131">currentAmount</span></span>   |<span data-ttu-id="68768-132">numéricos</span><span class="sxs-lookup"><span data-stu-id="68768-132">numeric</span></span>  |<span data-ttu-id="68768-133">Especifica o saldo para o período de envelhecimento atual.</span><span class="sxs-lookup"><span data-stu-id="68768-133">Specifies balance for the current aging period.</span></span>|
|<span data-ttu-id="68768-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="68768-134">period1Amount</span></span>   |<span data-ttu-id="68768-135">numéricos</span><span class="sxs-lookup"><span data-stu-id="68768-135">numeric</span></span>  |<span data-ttu-id="68768-136">Especifica o saldo no primeiro período de classificação por vencimento.</span><span class="sxs-lookup"><span data-stu-id="68768-136">Specifies balance in the first aging period.</span></span> |
|<span data-ttu-id="68768-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="68768-137">period2Amount</span></span>   |<span data-ttu-id="68768-138">numéricos</span><span class="sxs-lookup"><span data-stu-id="68768-138">numeric</span></span>  |<span data-ttu-id="68768-139">Especifica o saldo no segundo período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="68768-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="68768-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="68768-140">period3Amount</span></span>   |<span data-ttu-id="68768-141">numéricos</span><span class="sxs-lookup"><span data-stu-id="68768-141">numeric</span></span>  |<span data-ttu-id="68768-142">Especifica o saldo no terceiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="68768-142">Specifies balance in the third aging period.</span></span> |
|<span data-ttu-id="68768-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="68768-143">agedAsOfDate</span></span>    |<span data-ttu-id="68768-144">data</span><span class="sxs-lookup"><span data-stu-id="68768-144">date</span></span>     |<span data-ttu-id="68768-145">Especifica a data de início do período usada para calcular os períodos de expiração.</span><span class="sxs-lookup"><span data-stu-id="68768-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="68768-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="68768-146">periodLengthFilter</span></span>|<span data-ttu-id="68768-147">string</span><span class="sxs-lookup"><span data-stu-id="68768-147">string</span></span> |<span data-ttu-id="68768-148">Especifica o comprimento dos períodos.</span><span class="sxs-lookup"><span data-stu-id="68768-148">Specifies the length of the periods.</span></span> <span data-ttu-id="68768-149">As unidades de tempo aceitáveis incluem: D, WD, W, M, Q e Y. C, o que significa a unidade de tempo atual com base na data, pode ser especificada como um prefixo para a unidade de tempo.</span><span class="sxs-lookup"><span data-stu-id="68768-149">Acceptable time units include: D, WD, W, M, Q, and Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="68768-150">Relações</span><span class="sxs-lookup"><span data-stu-id="68768-150">Relationships</span></span>
<span data-ttu-id="68768-151">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="68768-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68768-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68768-152">JSON representation</span></span>

<span data-ttu-id="68768-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68768-153">Here is a JSON representation of the resource.</span></span>


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


