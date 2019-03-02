---
title: tipo de recurso customerPaymentJournals
description: Um diário de pagamentos do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a8b01124db732866e1a7b971af57d7e0a2b692e1
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365735"
---
# <a name="customerpaymentsjournals-resource-type"></a><span data-ttu-id="f01c6-103">tipo de recurso customerPaymentsJournals</span><span class="sxs-lookup"><span data-stu-id="f01c6-103">customerPaymentsJournals resource type</span></span>
<span data-ttu-id="f01c6-104">Representa um diário de pagamento do cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="f01c6-104">Represents a customer payment journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f01c6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f01c6-105">Methods</span></span>

| <span data-ttu-id="f01c6-106">Método</span><span class="sxs-lookup"><span data-stu-id="f01c6-106">Method</span></span>               | <span data-ttu-id="f01c6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f01c6-107">Return Type</span></span>             |<span data-ttu-id="f01c6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f01c6-108">Description</span></span>                      |
|:---------------------|:------------------------|:--------------------------------|
|[<span data-ttu-id="f01c6-109">Obter customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="f01c6-109">Get customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-get.md)      |<span data-ttu-id="f01c6-110">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="f01c6-110">customerPaymentJournals</span></span>|<span data-ttu-id="f01c6-111">Obtém um diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="f01c6-111">Gets a customer payment journal.</span></span>   |
|[<span data-ttu-id="f01c6-112">Postar customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="f01c6-112">Post customerPaymentJournals</span></span>](../api/dynamics-create-customerpaymentsjournal.md)  |<span data-ttu-id="f01c6-113">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="f01c6-113">customerPaymentJournals</span></span>|<span data-ttu-id="f01c6-114">Cria um diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="f01c6-114">Creates a customer payment journal.</span></span>|
|[<span data-ttu-id="f01c6-115">Patch customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="f01c6-115">Patch customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-update.md) |<span data-ttu-id="f01c6-116">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="f01c6-116">customerPaymentJournals</span></span>|<span data-ttu-id="f01c6-117">Atualiza um diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="f01c6-117">Updates a customer payment journal.</span></span>|
|[<span data-ttu-id="f01c6-118">Excluir customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="f01c6-118">Delete customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-delete.md)|<span data-ttu-id="f01c6-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f01c6-119">none</span></span>                     |<span data-ttu-id="f01c6-120">Exclui um diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="f01c6-120">Deletes a customer payment journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="f01c6-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f01c6-121">Properties</span></span>
| <span data-ttu-id="f01c6-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f01c6-122">Property</span></span>           | <span data-ttu-id="f01c6-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f01c6-123">Type</span></span>                  |<span data-ttu-id="f01c6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f01c6-124">Description</span></span>                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|<span data-ttu-id="f01c6-125">id</span><span class="sxs-lookup"><span data-stu-id="f01c6-125">id</span></span>                  |<span data-ttu-id="f01c6-126">GUID</span><span class="sxs-lookup"><span data-stu-id="f01c6-126">GUID</span></span>                   |<span data-ttu-id="f01c6-127">A ID exclusiva do diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="f01c6-127">The unique ID of the customer payment journal.</span></span> <span data-ttu-id="f01c6-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="f01c6-128">Non-editable.</span></span>           |
|<span data-ttu-id="f01c6-129">código</span><span class="sxs-lookup"><span data-stu-id="f01c6-129">code</span></span>                |<span data-ttu-id="f01c6-130">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="f01c6-130">string, maximum size 10</span></span>| <span data-ttu-id="f01c6-131">O código do diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="f01c6-131">The code of the customer payment journal.</span></span>                             |
|<span data-ttu-id="f01c6-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f01c6-132">displayName</span></span>         |<span data-ttu-id="f01c6-133">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="f01c6-133">string, maximum size 50</span></span>| <span data-ttu-id="f01c6-134">O nome de exibição do diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="f01c6-134">The display name of the customer payment journal.</span></span>                     |
|<span data-ttu-id="f01c6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f01c6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f01c6-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="f01c6-136">datetime</span></span>               |<span data-ttu-id="f01c6-137">O último DateTime que o diário de pagamentos do cliente foi modificado.</span><span class="sxs-lookup"><span data-stu-id="f01c6-137">The last datetime the customer payment journal was modified.</span></span> <span data-ttu-id="f01c6-138">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="f01c6-138">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f01c6-139">Relações</span><span class="sxs-lookup"><span data-stu-id="f01c6-139">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="f01c6-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f01c6-140">JSON representation</span></span>

<span data-ttu-id="f01c6-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f01c6-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

