---
title: tipo de recurso trialBalance
description: Um objeto de balancete no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: b7d3fee76df5f60c47639183f7d3e7ce54164f81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503212"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="2a63c-103">tipo de recurso trialBalance</span><span class="sxs-lookup"><span data-stu-id="2a63c-103">trialBalance resource type</span></span>

<span data-ttu-id="2a63c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2a63c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a63c-105">Representa um balancete no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2a63c-105">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="2a63c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2a63c-106">Methods</span></span>

| <span data-ttu-id="2a63c-107">Método</span><span class="sxs-lookup"><span data-stu-id="2a63c-107">Method</span></span>       | <span data-ttu-id="2a63c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2a63c-108">Return Type</span></span>  |<span data-ttu-id="2a63c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a63c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a63c-110">Obter trialBalance</span><span class="sxs-lookup"><span data-stu-id="2a63c-110">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="2a63c-111">trialBalance</span><span class="sxs-lookup"><span data-stu-id="2a63c-111">trialBalance</span></span>|<span data-ttu-id="2a63c-112">Obtém um objeto de saldo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="2a63c-112">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a63c-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a63c-113">Properties</span></span>
| <span data-ttu-id="2a63c-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a63c-114">Property</span></span>     | <span data-ttu-id="2a63c-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a63c-115">Type</span></span>   |<span data-ttu-id="2a63c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a63c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a63c-117">number</span><span class="sxs-lookup"><span data-stu-id="2a63c-117">number</span></span>|<span data-ttu-id="2a63c-118">string</span><span class="sxs-lookup"><span data-stu-id="2a63c-118">string</span></span>|<span data-ttu-id="2a63c-119">O número da conta de G/L do item trialBalance</span><span class="sxs-lookup"><span data-stu-id="2a63c-119">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="2a63c-120">accountId</span><span class="sxs-lookup"><span data-stu-id="2a63c-120">accountId</span></span>|<span data-ttu-id="2a63c-121">GUID</span><span class="sxs-lookup"><span data-stu-id="2a63c-121">GUID</span></span>|<span data-ttu-id="2a63c-122">O identificador exclusivo da conta de G/L do registro.</span><span class="sxs-lookup"><span data-stu-id="2a63c-122">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="2a63c-123">accountType</span><span class="sxs-lookup"><span data-stu-id="2a63c-123">accountType</span></span>|<span data-ttu-id="2a63c-124">string</span><span class="sxs-lookup"><span data-stu-id="2a63c-124">string</span></span>|<span data-ttu-id="2a63c-125">O tipo de conta da conta G/L do registro.</span><span class="sxs-lookup"><span data-stu-id="2a63c-125">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="2a63c-126">Exiba</span><span class="sxs-lookup"><span data-stu-id="2a63c-126">display</span></span>|<span data-ttu-id="2a63c-127">string</span><span class="sxs-lookup"><span data-stu-id="2a63c-127">string</span></span>|<span data-ttu-id="2a63c-128">O nome da conta do G/L para o item trialBalance.</span><span class="sxs-lookup"><span data-stu-id="2a63c-128">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="2a63c-129">totalDebit</span><span class="sxs-lookup"><span data-stu-id="2a63c-129">totalDebit</span></span>|<span data-ttu-id="2a63c-130">string</span><span class="sxs-lookup"><span data-stu-id="2a63c-130">string</span></span>|<span data-ttu-id="2a63c-131">Representa o valor total de débito na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="2a63c-131">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="2a63c-132">totalCredit</span><span class="sxs-lookup"><span data-stu-id="2a63c-132">totalCredit</span></span>|<span data-ttu-id="2a63c-133">string</span><span class="sxs-lookup"><span data-stu-id="2a63c-133">string</span></span>|<span data-ttu-id="2a63c-134">Representa o valor total de crédito na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="2a63c-134">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="2a63c-135">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="2a63c-135">balanceAtDateDebit</span></span>|<span data-ttu-id="2a63c-136">string</span><span class="sxs-lookup"><span data-stu-id="2a63c-136">string</span></span>|<span data-ttu-id="2a63c-137">Representa o saldo positivo no valor da data na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="2a63c-137">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="2a63c-138">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="2a63c-138">balanceAtDateCredit</span></span>|<span data-ttu-id="2a63c-139">string</span><span class="sxs-lookup"><span data-stu-id="2a63c-139">string</span></span>|<span data-ttu-id="2a63c-140">Representa o saldo negativo no valor da data na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="2a63c-140">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="2a63c-141">dateFilter</span><span class="sxs-lookup"><span data-stu-id="2a63c-141">dateFilter</span></span>|<span data-ttu-id="2a63c-142">data</span><span class="sxs-lookup"><span data-stu-id="2a63c-142">date</span></span>|<span data-ttu-id="2a63c-143">O filtro de data usado para calcular os itens do trialBalance.</span><span class="sxs-lookup"><span data-stu-id="2a63c-143">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="2a63c-144">Relações</span><span class="sxs-lookup"><span data-stu-id="2a63c-144">Relationships</span></span>
<span data-ttu-id="2a63c-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2a63c-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a63c-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a63c-146">JSON representation</span></span>

<span data-ttu-id="2a63c-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a63c-147">Here is a JSON representation of the resource.</span></span>


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

