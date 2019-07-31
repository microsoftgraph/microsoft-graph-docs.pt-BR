---
title: tipo de recurso agedAccountsPayable
description: Um objeto de contas a pagar antigo no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a135627804e2d6c5be4203c0ee0c229642c70c65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973741"
---
# <a name="agedaccountspayable-resource-type"></a><span data-ttu-id="8261b-103">tipo de recurso agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="8261b-103">agedAccountsPayable resource type</span></span>
<span data-ttu-id="8261b-104">Representa um objeto agedAccountsPayable no Dynamics 365 Business central, que está mostrando o envelhecimento de uma conta de fornecedor.</span><span class="sxs-lookup"><span data-stu-id="8261b-104">Represents an agedAccountsPayable object in Dynamics 365 Business Central, which is showing the aging of a vendor account.</span></span>

## <a name="methods"></a><span data-ttu-id="8261b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8261b-105">Methods</span></span>

| <span data-ttu-id="8261b-106">Método</span><span class="sxs-lookup"><span data-stu-id="8261b-106">Method</span></span>         | <span data-ttu-id="8261b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8261b-107">Return Type</span></span>  |<span data-ttu-id="8261b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8261b-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="8261b-109">Obter agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="8261b-109">Get agedAccountsPayable</span></span>](../api/dynamics-agedaccountspayable-get.md)|<span data-ttu-id="8261b-110">agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="8261b-110">agedAccountsPayable</span></span>|<span data-ttu-id="8261b-111">Obter o objeto agedAccountsPayable</span><span class="sxs-lookup"><span data-stu-id="8261b-111">Get agedAccountsPayable object</span></span>|

## <a name="properties"></a><span data-ttu-id="8261b-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8261b-112">Properties</span></span>
| <span data-ttu-id="8261b-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8261b-113">Property</span></span>      | <span data-ttu-id="8261b-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="8261b-114">Type</span></span>     |<span data-ttu-id="8261b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="8261b-115">Description</span></span>                                 |
|:--------------|:---------|:-------------------------------------------|
|<span data-ttu-id="8261b-116">VendorID</span><span class="sxs-lookup"><span data-stu-id="8261b-116">vendorId</span></span>       |<span data-ttu-id="8261b-117">GUID</span><span class="sxs-lookup"><span data-stu-id="8261b-117">GUID</span></span>      |<span data-ttu-id="8261b-118">A ID exclusiva do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="8261b-118">The unique ID of vendor.</span></span>                    |
|<span data-ttu-id="8261b-119">vendorNumber</span><span class="sxs-lookup"><span data-stu-id="8261b-119">vendorNumber</span></span>   |<span data-ttu-id="8261b-120">string</span><span class="sxs-lookup"><span data-stu-id="8261b-120">string</span></span>    |<span data-ttu-id="8261b-121">Especifica o número do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="8261b-121">Specifies vendor's number.</span></span>                  |
|<span data-ttu-id="8261b-122">name</span><span class="sxs-lookup"><span data-stu-id="8261b-122">name</span></span>           |<span data-ttu-id="8261b-123">string</span><span class="sxs-lookup"><span data-stu-id="8261b-123">string</span></span>    |<span data-ttu-id="8261b-124">Especifica o nome do fornecedor.</span><span class="sxs-lookup"><span data-stu-id="8261b-124">Specifies vendor's name.</span></span>                    |
|<span data-ttu-id="8261b-125">currencyCode</span><span class="sxs-lookup"><span data-stu-id="8261b-125">currencyCode</span></span>   |<span data-ttu-id="8261b-126">string</span><span class="sxs-lookup"><span data-stu-id="8261b-126">string</span></span>    |<span data-ttu-id="8261b-127">Especifica a moeda.</span><span class="sxs-lookup"><span data-stu-id="8261b-127">Specifies the currency.</span></span>                     |
|<span data-ttu-id="8261b-128">balanceDue</span><span class="sxs-lookup"><span data-stu-id="8261b-128">balanceDue</span></span>     |<span data-ttu-id="8261b-129">numéricos</span><span class="sxs-lookup"><span data-stu-id="8261b-129">numeric</span></span>   |<span data-ttu-id="8261b-130">Especifica o saldo total devido ao fornecedor.</span><span class="sxs-lookup"><span data-stu-id="8261b-130">Specifies the total balance due to the vendor.</span></span>|
|<span data-ttu-id="8261b-131">currentAmount</span><span class="sxs-lookup"><span data-stu-id="8261b-131">currentAmount</span></span>  |<span data-ttu-id="8261b-132">numéricos</span><span class="sxs-lookup"><span data-stu-id="8261b-132">numeric</span></span>   |<span data-ttu-id="8261b-133">Especifica o saldo antes do primeiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="8261b-133">Specifies balance before first aging period.</span></span>|
|<span data-ttu-id="8261b-134">period1Amount</span><span class="sxs-lookup"><span data-stu-id="8261b-134">period1Amount</span></span>  |<span data-ttu-id="8261b-135">numéricos</span><span class="sxs-lookup"><span data-stu-id="8261b-135">numeric</span></span>   |<span data-ttu-id="8261b-136">Especifica o saldo no primeiro período de classificação por vencimento.</span><span class="sxs-lookup"><span data-stu-id="8261b-136">Specifies balance in the first aging period.</span></span>|
|<span data-ttu-id="8261b-137">period2Amount</span><span class="sxs-lookup"><span data-stu-id="8261b-137">period2Amount</span></span>  |<span data-ttu-id="8261b-138">numéricos</span><span class="sxs-lookup"><span data-stu-id="8261b-138">numeric</span></span>   |<span data-ttu-id="8261b-139">Especifica o saldo no segundo período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="8261b-139">Specifies balance in the second aging period.</span></span>|
|<span data-ttu-id="8261b-140">period3Amount</span><span class="sxs-lookup"><span data-stu-id="8261b-140">period3Amount</span></span>  |<span data-ttu-id="8261b-141">numéricos</span><span class="sxs-lookup"><span data-stu-id="8261b-141">numeric</span></span>   |<span data-ttu-id="8261b-142">Especifica o saldo no terceiro período de envelhecimento.</span><span class="sxs-lookup"><span data-stu-id="8261b-142">Specifies balance in the third aging period.</span></span>|
|<span data-ttu-id="8261b-143">agedAsOfDate</span><span class="sxs-lookup"><span data-stu-id="8261b-143">agedAsOfDate</span></span>   |<span data-ttu-id="8261b-144">data</span><span class="sxs-lookup"><span data-stu-id="8261b-144">date</span></span>|<span data-ttu-id="8261b-145">Especifica a data de início do período usada para calcular os períodos de expiração.</span><span class="sxs-lookup"><span data-stu-id="8261b-145">Specifies period start date used to calculate aging periods.</span></span>|
|<span data-ttu-id="8261b-146">periodLengthFilter</span><span class="sxs-lookup"><span data-stu-id="8261b-146">periodLengthFilter</span></span>|<span data-ttu-id="8261b-147">string</span><span class="sxs-lookup"><span data-stu-id="8261b-147">string</span></span> |<span data-ttu-id="8261b-148">Especifica o comprimento dos períodos.</span><span class="sxs-lookup"><span data-stu-id="8261b-148">Specifies the length of the periods.</span></span> <span data-ttu-id="8261b-149">Os valores aceitáveis para as unidades de tempo são: D, WD, W, M, Q ou Y. C, o que significa unidade de tempo atual com base na data, pode ser especificado como um prefixo para a unidade de tempo.</span><span class="sxs-lookup"><span data-stu-id="8261b-149">Acceptable values for the time units are: D, WD, W, M, Q, or Y. C, meaning current time unit based on date, can be specified as a prefix to the time unit.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8261b-150">Relações</span><span class="sxs-lookup"><span data-stu-id="8261b-150">Relationships</span></span>
<span data-ttu-id="8261b-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8261b-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8261b-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8261b-152">JSON representation</span></span>

<span data-ttu-id="8261b-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8261b-153">Here is a JSON representation of the resource.</span></span>


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
