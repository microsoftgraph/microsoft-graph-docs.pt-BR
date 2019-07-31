---
title: tipo de recurso trialBalance
description: Um objeto de balancete no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 02e4f039411c992cd1d7335fc2463d660b8ff181
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972870"
---
# <a name="trialbalance-resource-type"></a><span data-ttu-id="81053-103">tipo de recurso trialBalance</span><span class="sxs-lookup"><span data-stu-id="81053-103">trialBalance resource type</span></span>
<span data-ttu-id="81053-104">Representa um balancete no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="81053-104">Represents a trial balance in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="81053-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="81053-105">Methods</span></span>

| <span data-ttu-id="81053-106">Método</span><span class="sxs-lookup"><span data-stu-id="81053-106">Method</span></span>       | <span data-ttu-id="81053-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="81053-107">Return Type</span></span>  |<span data-ttu-id="81053-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="81053-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81053-109">Obter trialBalance</span><span class="sxs-lookup"><span data-stu-id="81053-109">Get trialBalance</span></span>](../api/dynamics-trialbalance-get.md)|<span data-ttu-id="81053-110">trialBalance</span><span class="sxs-lookup"><span data-stu-id="81053-110">trialBalance</span></span>|<span data-ttu-id="81053-111">Obtém um objeto de saldo de avaliação.</span><span class="sxs-lookup"><span data-stu-id="81053-111">Gets a trial balance object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81053-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="81053-112">Properties</span></span>
| <span data-ttu-id="81053-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81053-113">Property</span></span>     | <span data-ttu-id="81053-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="81053-114">Type</span></span>   |<span data-ttu-id="81053-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="81053-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81053-116">number</span><span class="sxs-lookup"><span data-stu-id="81053-116">number</span></span>|<span data-ttu-id="81053-117">string</span><span class="sxs-lookup"><span data-stu-id="81053-117">string</span></span>|<span data-ttu-id="81053-118">O número da conta de G/L do item trialBalance</span><span class="sxs-lookup"><span data-stu-id="81053-118">The G/L Account number for the trialBalance item</span></span>|
|<span data-ttu-id="81053-119">accountId</span><span class="sxs-lookup"><span data-stu-id="81053-119">accountId</span></span>|<span data-ttu-id="81053-120">GUID</span><span class="sxs-lookup"><span data-stu-id="81053-120">GUID</span></span>|<span data-ttu-id="81053-121">O identificador exclusivo da conta de G/L do registro.</span><span class="sxs-lookup"><span data-stu-id="81053-121">The unique identifier for the G/L account of the record.</span></span>|
|<span data-ttu-id="81053-122">accountType</span><span class="sxs-lookup"><span data-stu-id="81053-122">accountType</span></span>|<span data-ttu-id="81053-123">string</span><span class="sxs-lookup"><span data-stu-id="81053-123">string</span></span>|<span data-ttu-id="81053-124">O tipo de conta da conta G/L do registro.</span><span class="sxs-lookup"><span data-stu-id="81053-124">The account type of the G/L account of the record.</span></span>|
|<span data-ttu-id="81053-125">Exiba</span><span class="sxs-lookup"><span data-stu-id="81053-125">display</span></span>|<span data-ttu-id="81053-126">string</span><span class="sxs-lookup"><span data-stu-id="81053-126">string</span></span>|<span data-ttu-id="81053-127">O nome da conta do G/L para o item trialBalance.</span><span class="sxs-lookup"><span data-stu-id="81053-127">The G/L Account name for the trialBalance item.</span></span>|
|<span data-ttu-id="81053-128">totalDebit</span><span class="sxs-lookup"><span data-stu-id="81053-128">totalDebit</span></span>|<span data-ttu-id="81053-129">string</span><span class="sxs-lookup"><span data-stu-id="81053-129">string</span></span>|<span data-ttu-id="81053-130">Representa o valor total de débito na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="81053-130">Represents total debit amount in G/L Account.</span></span>|
|<span data-ttu-id="81053-131">totalCredit</span><span class="sxs-lookup"><span data-stu-id="81053-131">totalCredit</span></span>|<span data-ttu-id="81053-132">string</span><span class="sxs-lookup"><span data-stu-id="81053-132">string</span></span>|<span data-ttu-id="81053-133">Representa o valor total de crédito na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="81053-133">Represents total credit amount in G/L Account.</span></span>|
|<span data-ttu-id="81053-134">balanceAtDateDebit</span><span class="sxs-lookup"><span data-stu-id="81053-134">balanceAtDateDebit</span></span>|<span data-ttu-id="81053-135">string</span><span class="sxs-lookup"><span data-stu-id="81053-135">string</span></span>|<span data-ttu-id="81053-136">Representa o saldo positivo no valor da data na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="81053-136">Represents positive Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="81053-137">balanceAtDateCredit</span><span class="sxs-lookup"><span data-stu-id="81053-137">balanceAtDateCredit</span></span>|<span data-ttu-id="81053-138">string</span><span class="sxs-lookup"><span data-stu-id="81053-138">string</span></span>|<span data-ttu-id="81053-139">Representa o saldo negativo no valor da data na conta G/L.</span><span class="sxs-lookup"><span data-stu-id="81053-139">Represents negative Balance at Date amount in G/L Account.</span></span>|
|<span data-ttu-id="81053-140">dateFilter</span><span class="sxs-lookup"><span data-stu-id="81053-140">dateFilter</span></span>|<span data-ttu-id="81053-141">data</span><span class="sxs-lookup"><span data-stu-id="81053-141">date</span></span>|<span data-ttu-id="81053-142">O filtro de data usado para calcular os itens do trialBalance.</span><span class="sxs-lookup"><span data-stu-id="81053-142">The date filter used to calculate the trialBalance items.</span></span>|


## <a name="relationships"></a><span data-ttu-id="81053-143">Relações</span><span class="sxs-lookup"><span data-stu-id="81053-143">Relationships</span></span>
<span data-ttu-id="81053-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="81053-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81053-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81053-145">JSON representation</span></span>

<span data-ttu-id="81053-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81053-146">Here is a JSON representation of the resource.</span></span>


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

