---
title: tipo de recurso trialBalance
description: Um objeto de balancete no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 43368ace9a47064833aa388dda0a7da31d9e5f0c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040032"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="29534-103">tipo de recurso trialBalance</span><span class="sxs-lookup"><span data-stu-id="29534-103">trialBalance resource type</span></span>

<span data-ttu-id="29534-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29534-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29534-105">Representa um balancete no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="29534-105">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="29534-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="29534-106">Methods</span></span>

| <span data-ttu-id="29534-107">Método</span><span class="sxs-lookup"><span data-stu-id="29534-107">Method</span></span>       | <span data-ttu-id="29534-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="29534-108">Return Type</span></span>  |<span data-ttu-id="29534-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29534-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29534-110">Obter trialBalance</span><span class="sxs-lookup"><span data-stu-id="29534-110">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="29534-111">trialBalance</span><span class="sxs-lookup"><span data-stu-id="29534-111">trialBalance</span></span>|<span data-ttu-id="29534-112">Obtém um objeto de saldo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="29534-112">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29534-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29534-113">Properties</span></span>
| <span data-ttu-id="29534-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29534-114">Property</span></span>     | <span data-ttu-id="29534-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="29534-115">Type</span></span>   |<span data-ttu-id="29534-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="29534-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29534-117">number</span><span class="sxs-lookup"><span data-stu-id="29534-117">number</span></span>|<span data-ttu-id="29534-118">string</span><span class="sxs-lookup"><span data-stu-id="29534-118">string</span></span>|<span data-ttu-id="29534-119">O número da conta de G/L do item trialBalance</span><span class="sxs-lookup"><span data-stu-id="29534-119">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="29534-120">accountId</span><span class="sxs-lookup"><span data-stu-id="29534-120">accountId</span></span>|<span data-ttu-id="29534-121">GUID</span><span class="sxs-lookup"><span data-stu-id="29534-121">GUID</span></span>|<span data-ttu-id="29534-122">O identificador exclusivo da conta de G/L do registro.</span><span class="sxs-lookup"><span data-stu-id="29534-122">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="29534-123">accountType</span><span class="sxs-lookup"><span data-stu-id="29534-123">accountType</span></span>|<span data-ttu-id="29534-124">string</span><span class="sxs-lookup"><span data-stu-id="29534-124">string</span></span>|<span data-ttu-id="29534-125">O tipo de conta da conta G/L do registro.</span><span class="sxs-lookup"><span data-stu-id="29534-125">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="29534-126">Exiba</span><span class="sxs-lookup"><span data-stu-id="29534-126">display</span></span>|<span data-ttu-id="29534-127">string</span><span class="sxs-lookup"><span data-stu-id="29534-127">string</span></span>|<span data-ttu-id="29534-128">O nome da conta do G/L para o item trialBalance.</span><span class="sxs-lookup"><span data-stu-id="29534-128">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="29534-129">totalDebit</span><span class="sxs-lookup"><span data-stu-id="29534-129">totalDebit</span></span>|<span data-ttu-id="29534-130">string</span><span class="sxs-lookup"><span data-stu-id="29534-130">string</span></span>|<span data-ttu-id="29534-131">Representa o valor total de débito na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="29534-131">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="29534-132">totalCredit</span><span class="sxs-lookup"><span data-stu-id="29534-132">totalCredit</span></span>|<span data-ttu-id="29534-133">string</span><span class="sxs-lookup"><span data-stu-id="29534-133">string</span></span>|<span data-ttu-id="29534-134">Representa o valor total de crédito na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="29534-134">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="29534-135">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="29534-135">balanceAtDateDebit</span></span>|<span data-ttu-id="29534-136">string</span><span class="sxs-lookup"><span data-stu-id="29534-136">string</span></span>|<span data-ttu-id="29534-137">Representa o saldo positivo no valor da data na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="29534-137">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="29534-138">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="29534-138">balanceAtDateCredit</span></span>|<span data-ttu-id="29534-139">string</span><span class="sxs-lookup"><span data-stu-id="29534-139">string</span></span>|<span data-ttu-id="29534-140">Representa o saldo negativo no valor da data na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="29534-140">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="29534-141">dateFilter</span><span class="sxs-lookup"><span data-stu-id="29534-141">dateFilter</span></span>|<span data-ttu-id="29534-142">data</span><span class="sxs-lookup"><span data-stu-id="29534-142">date</span></span>|<span data-ttu-id="29534-143">O filtro de data usado para calcular os itens do trialBalance.</span><span class="sxs-lookup"><span data-stu-id="29534-143">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="29534-144">Relações</span><span class="sxs-lookup"><span data-stu-id="29534-144">Relationships</span></span>
<span data-ttu-id="29534-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29534-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29534-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29534-146">JSON representation</span></span>

<span data-ttu-id="29534-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29534-147">Here is a JSON representation of the resource.</span></span>


```json
{
    "number": "string",
    "accountId": "GUID",
    "accountType": "string",
    "display": "string",
    "totalDebit": "string",
    "totalCredit": "string",
    "balanceAtDateDebit": "string",
    "balanceAtDateCredit": "string",
    "dateFilter": "date"
}

```



