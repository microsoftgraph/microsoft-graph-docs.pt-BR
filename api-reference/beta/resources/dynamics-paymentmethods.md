---
title: tipo de recurso paymentMethods
description: Um objeto de método de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1e4cd044d4b552a9239b742efb302633524ce22b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507235"
---
# <a name="paymentmethods-resource-type"></a><span data-ttu-id="32c34-103">tipo de recurso paymentMethods</span><span class="sxs-lookup"><span data-stu-id="32c34-103">paymentMethods resource type</span></span>
<span data-ttu-id="32c34-104">Representa um método de pagamento no Dynamics 365 Business central, como PayPal, cartão de crédito e conta bancária.</span><span class="sxs-lookup"><span data-stu-id="32c34-104">Represents a method of payment in Dynamics 365 Business Central, such as PayPal, credit card, and bank account.</span></span>

## <a name="methods"></a><span data-ttu-id="32c34-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="32c34-105">Methods</span></span>

| <span data-ttu-id="32c34-106">Método</span><span class="sxs-lookup"><span data-stu-id="32c34-106">Method</span></span>                                                          | <span data-ttu-id="32c34-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="32c34-107">Return Type</span></span>  |<span data-ttu-id="32c34-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="32c34-108">Description</span></span>             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[<span data-ttu-id="32c34-109">Obter paymentMethods</span><span class="sxs-lookup"><span data-stu-id="32c34-109">Get paymentMethods</span></span>](../api/dynamics-paymentmethods-get.md)      |<span data-ttu-id="32c34-110">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="32c34-110">paymentMethods</span></span>|<span data-ttu-id="32c34-111">Obtém um objeto de método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="32c34-111">Gets a payment method object.</span></span>   |
|[<span data-ttu-id="32c34-112">Postar paymentMethods</span><span class="sxs-lookup"><span data-stu-id="32c34-112">Post paymentMethods</span></span>](../api/dynamics-create-paymentmethods.md)  |<span data-ttu-id="32c34-113">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="32c34-113">paymentMethods</span></span>|<span data-ttu-id="32c34-114">Cria um objeto de método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="32c34-114">Creates a payment method object.</span></span>|
|[<span data-ttu-id="32c34-115">Patch paymentMethods</span><span class="sxs-lookup"><span data-stu-id="32c34-115">Patch paymentMethods</span></span>](../api/dynamics-paymentmethods-update.md) |<span data-ttu-id="32c34-116">paymentMethods</span><span class="sxs-lookup"><span data-stu-id="32c34-116">paymentMethods</span></span>|<span data-ttu-id="32c34-117">Atualiza um objeto de método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="32c34-117">Updates a payment method object.</span></span>|
|[<span data-ttu-id="32c34-118">Excluir paymentMethods</span><span class="sxs-lookup"><span data-stu-id="32c34-118">Delete paymentMethods</span></span>](../api/dynamics-paymentmethods-delete.md)|<span data-ttu-id="32c34-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="32c34-119">none</span></span>          |<span data-ttu-id="32c34-120">Exclui um objeto de método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="32c34-120">Deletes a payment method object.</span></span>|

## <a name="properties"></a><span data-ttu-id="32c34-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32c34-121">Properties</span></span>
| <span data-ttu-id="32c34-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32c34-122">Property</span></span>           | <span data-ttu-id="32c34-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="32c34-123">Type</span></span>   |<span data-ttu-id="32c34-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="32c34-124">Description</span></span>                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|<span data-ttu-id="32c34-125">id</span><span class="sxs-lookup"><span data-stu-id="32c34-125">id</span></span>                  |<span data-ttu-id="32c34-126">GUID</span><span class="sxs-lookup"><span data-stu-id="32c34-126">GUID</span></span>    |<span data-ttu-id="32c34-127">A ID exclusiva do paymentMethods.</span><span class="sxs-lookup"><span data-stu-id="32c34-127">The unique ID of the paymentMethods.</span></span> <span data-ttu-id="32c34-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="32c34-128">Non-editable.</span></span>           |
|<span data-ttu-id="32c34-129">código</span><span class="sxs-lookup"><span data-stu-id="32c34-129">code</span></span>                |<span data-ttu-id="32c34-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32c34-130">string</span></span>  |<span data-ttu-id="32c34-131">Especifica o código do método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="32c34-131">Specifies the payment method code.</span></span>                           |
|<span data-ttu-id="32c34-132">displayName</span><span class="sxs-lookup"><span data-stu-id="32c34-132">displayName</span></span>         |<span data-ttu-id="32c34-133">string</span><span class="sxs-lookup"><span data-stu-id="32c34-133">string</span></span>  |<span data-ttu-id="32c34-134">Especifica o nome de exibição do método de pagamento.</span><span class="sxs-lookup"><span data-stu-id="32c34-134">Specifies the payment method display name.</span></span>                   |
|<span data-ttu-id="32c34-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32c34-135">lastModifiedDateTime</span></span>|<span data-ttu-id="32c34-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="32c34-136">datetime</span></span>|<span data-ttu-id="32c34-137">A última data/hora em que o método de pagamento foi modificado.</span><span class="sxs-lookup"><span data-stu-id="32c34-137">The last datetime the payment method was modified.</span></span> <span data-ttu-id="32c34-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="32c34-138">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="32c34-139">Relações</span><span class="sxs-lookup"><span data-stu-id="32c34-139">Relationships</span></span>
<span data-ttu-id="32c34-140">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="32c34-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32c34-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32c34-141">JSON representation</span></span>

<span data-ttu-id="32c34-142">Veja a seguir uma representação JSON do paymentMethods.</span><span class="sxs-lookup"><span data-stu-id="32c34-142">Here is a JSON representation of the paymentMethods.</span></span>


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```
