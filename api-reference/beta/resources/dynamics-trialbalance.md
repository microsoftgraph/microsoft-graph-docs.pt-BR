---
title: tipo de recurso trialBalance
description: Um objeto de balancete no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1a7e906e50ddf39e4c9e2d3d9dde11226c7ec662
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534847"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="7b03b-103">tipo de recurso trialBalance</span><span class="sxs-lookup"><span data-stu-id="7b03b-103">trialBalance resource type</span></span>
<span data-ttu-id="7b03b-104">Representa um balancete no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="7b03b-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="7b03b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b03b-105">Methods</span></span>

| <span data-ttu-id="7b03b-106">Método</span><span class="sxs-lookup"><span data-stu-id="7b03b-106">Method</span></span>       | <span data-ttu-id="7b03b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b03b-107">Return Type</span></span>  |<span data-ttu-id="7b03b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b03b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b03b-109">Obter trialBalance</span><span class="sxs-lookup"><span data-stu-id="7b03b-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="7b03b-110">trialBalance</span><span class="sxs-lookup"><span data-stu-id="7b03b-110">trialBalance</span></span>|<span data-ttu-id="7b03b-111">Obtém um objeto de saldo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="7b03b-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b03b-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b03b-112">Properties</span></span>
| <span data-ttu-id="7b03b-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b03b-113">Property</span></span>     | <span data-ttu-id="7b03b-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b03b-114">Type</span></span>   |<span data-ttu-id="7b03b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b03b-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b03b-116">number</span><span class="sxs-lookup"><span data-stu-id="7b03b-116">number</span></span>|<span data-ttu-id="7b03b-117">string</span><span class="sxs-lookup"><span data-stu-id="7b03b-117">string</span></span>|<span data-ttu-id="7b03b-118">O número da conta de G/L do item trialBalance</span><span class="sxs-lookup"><span data-stu-id="7b03b-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="7b03b-119">accountId</span><span class="sxs-lookup"><span data-stu-id="7b03b-119">accountId</span></span>|<span data-ttu-id="7b03b-120">GUID</span><span class="sxs-lookup"><span data-stu-id="7b03b-120">GUID</span></span>|<span data-ttu-id="7b03b-121">O identificador exclusivo da conta de G/L do registro.</span><span class="sxs-lookup"><span data-stu-id="7b03b-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="7b03b-122">accountType</span><span class="sxs-lookup"><span data-stu-id="7b03b-122">accountType</span></span>|<span data-ttu-id="7b03b-123">string</span><span class="sxs-lookup"><span data-stu-id="7b03b-123">string</span></span>|<span data-ttu-id="7b03b-124">O tipo de conta da conta G/L do registro.</span><span class="sxs-lookup"><span data-stu-id="7b03b-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="7b03b-125">Exiba</span><span class="sxs-lookup"><span data-stu-id="7b03b-125">display</span></span>|<span data-ttu-id="7b03b-126">string</span><span class="sxs-lookup"><span data-stu-id="7b03b-126">string</span></span>|<span data-ttu-id="7b03b-127">O nome da conta do G/L para o item trialBalance.</span><span class="sxs-lookup"><span data-stu-id="7b03b-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="7b03b-128">totalDebit</span><span class="sxs-lookup"><span data-stu-id="7b03b-128">totalDebit</span></span>|<span data-ttu-id="7b03b-129">string</span><span class="sxs-lookup"><span data-stu-id="7b03b-129">string</span></span>|<span data-ttu-id="7b03b-130">Representa o valor total de débito na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="7b03b-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="7b03b-131">totalCredit</span><span class="sxs-lookup"><span data-stu-id="7b03b-131">totalCredit</span></span>|<span data-ttu-id="7b03b-132">string</span><span class="sxs-lookup"><span data-stu-id="7b03b-132">string</span></span>|<span data-ttu-id="7b03b-133">Representa o valor total de crédito na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="7b03b-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="7b03b-134">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="7b03b-134">balanceAtDateDebit</span></span>|<span data-ttu-id="7b03b-135">string</span><span class="sxs-lookup"><span data-stu-id="7b03b-135">string</span></span>|<span data-ttu-id="7b03b-136">Representa o saldo positivo no valor da data na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="7b03b-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="7b03b-137">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="7b03b-137">balanceAtDateCredit</span></span>|<span data-ttu-id="7b03b-138">string</span><span class="sxs-lookup"><span data-stu-id="7b03b-138">string</span></span>|<span data-ttu-id="7b03b-139">Representa o saldo negativo no valor da data na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="7b03b-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="7b03b-140">dateFilter</span><span class="sxs-lookup"><span data-stu-id="7b03b-140">dateFilter</span></span>|<span data-ttu-id="7b03b-141">data</span><span class="sxs-lookup"><span data-stu-id="7b03b-141">date</span></span>|<span data-ttu-id="7b03b-142">O filtro de data usado para calcular os itens do trialBalance.</span><span class="sxs-lookup"><span data-stu-id="7b03b-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7b03b-143">Relações</span><span class="sxs-lookup"><span data-stu-id="7b03b-143">Relationships</span></span>
<span data-ttu-id="7b03b-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b03b-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b03b-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b03b-145">JSON representation</span></span>

<span data-ttu-id="7b03b-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b03b-146">Here is a JSON representation of the resource.</span></span>


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

