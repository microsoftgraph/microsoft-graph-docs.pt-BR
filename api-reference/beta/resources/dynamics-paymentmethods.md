---
title: tipo de recurso paymentMethods
description: Um objeto de método de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: b30f97166625d45eba1a78342c219cbb74f42a8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013741"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="73a7d-103">tipo de recurso paymentMethods</span><span class="sxs-lookup"><span data-stu-id="73a7d-103">paymentMethods resource type</span></span>

<span data-ttu-id="73a7d-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="73a7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73a7d-105">Representa um método de pagamento no Dynamics 365 Business central, como PayPal, cartão de crédito e conta bancária.</span><span class="sxs-lookup"><span data-stu-id="73a7d-105">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="73a7d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="73a7d-106">Methods</span></span>

| <span data-ttu-id="73a7d-107">Método</span><span class="sxs-lookup"><span data-stu-id="73a7d-107">Method</span></span>                                                          | <span data-ttu-id="73a7d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73a7d-108">Return Type</span></span>  |<span data-ttu-id="73a7d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="73a7d-109">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="73a7d-110">Obter paymentMethods</span><span class="sxs-lookup"><span data-stu-id="73a7d-110">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="73a7d-111">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="73a7d-111">paymentMethods</span></span>|<span data-ttu-id="73a7d-112">Obtém um objeto de método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="73a7d-112">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="73a7d-113">Postar paymentMethods</span><span class="sxs-lookup"><span data-stu-id="73a7d-113">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="73a7d-114">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="73a7d-114">paymentMethods</span></span>|<span data-ttu-id="73a7d-115">Cria um objeto de método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="73a7d-115">Creates a payment method object.</span></span>|
|[<span data-ttu-id="73a7d-116">Patch paymentMethods</span><span class="sxs-lookup"><span data-stu-id="73a7d-116">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="73a7d-117">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="73a7d-117">paymentMethods</span></span>|<span data-ttu-id="73a7d-118">Atualiza um objeto de método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="73a7d-118">Updates a payment method object.</span></span>|
|[<span data-ttu-id="73a7d-119">Excluir paymentMethods</span><span class="sxs-lookup"><span data-stu-id="73a7d-119">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="73a7d-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="73a7d-120">none</span></span>          |<span data-ttu-id="73a7d-121">Exclui um objeto de método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="73a7d-121">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73a7d-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73a7d-122">Properties</span></span>
| <span data-ttu-id="73a7d-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73a7d-123">Property</span></span>           | <span data-ttu-id="73a7d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="73a7d-124">Type</span></span>   |<span data-ttu-id="73a7d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="73a7d-125">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="73a7d-126">id</span><span class="sxs-lookup"><span data-stu-id="73a7d-126">id</span></span>                  |<span data-ttu-id="73a7d-127">GUID</span><span class="sxs-lookup"><span data-stu-id="73a7d-127">GUID</span></span>    |<span data-ttu-id="73a7d-128">A ID exclusiva do paymentMethods.</span><span class="sxs-lookup"><span data-stu-id="73a7d-128">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="73a7d-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="73a7d-129">Non-editable.</span></span>           |
|<span data-ttu-id="73a7d-130">código</span><span class="sxs-lookup"><span data-stu-id="73a7d-130">code</span></span>                |<span data-ttu-id="73a7d-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73a7d-131">string</span></span>  |<span data-ttu-id="73a7d-132">Especifica o código do método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="73a7d-132">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="73a7d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="73a7d-133">displayName</span></span>         |<span data-ttu-id="73a7d-134">string</span><span class="sxs-lookup"><span data-stu-id="73a7d-134">string</span></span>  |<span data-ttu-id="73a7d-135">Especifica o nome de exibição do método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="73a7d-135">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="73a7d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73a7d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="73a7d-137">datetime</span><span class="sxs-lookup"><span data-stu-id="73a7d-137">datetime</span></span>|<span data-ttu-id="73a7d-138">A última data/hora em que o método de pagamento foi modificado.</span><span class="sxs-lookup"><span data-stu-id="73a7d-138">The last datetime the payment method was modified.</span></span> <span data-ttu-id="73a7d-139">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73a7d-139">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="73a7d-140">Relações</span><span class="sxs-lookup"><span data-stu-id="73a7d-140">Relationships</span></span>
<span data-ttu-id="73a7d-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73a7d-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73a7d-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73a7d-142">JSON representation</span></span>

<span data-ttu-id="73a7d-143">Veja a seguir uma representação JSON do paymentMethods.</span><span class="sxs-lookup"><span data-stu-id="73a7d-143">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


