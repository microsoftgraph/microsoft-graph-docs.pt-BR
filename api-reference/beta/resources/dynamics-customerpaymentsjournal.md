---
title: tipo de recurso customerPaymentJournals
description: Um diário de pagamentos do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 0791fe2b8c36bdff535f7fc56dea54abe1632647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973629"
---
# <a name="customerpaymentsjournals-resource-type"></a><span data-ttu-id="74669-103">tipo de recurso customerPaymentsJournals</span><span class="sxs-lookup"><span data-stu-id="74669-103">customerPaymentsJournals resource type</span></span>
<span data-ttu-id="74669-104">Representa um diário de pagamento do cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="74669-104">Represents a customer payment journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="74669-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="74669-105">Methods</span></span>

| <span data-ttu-id="74669-106">Método</span><span class="sxs-lookup"><span data-stu-id="74669-106">Method</span></span>               | <span data-ttu-id="74669-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74669-107">Return Type</span></span>             |<span data-ttu-id="74669-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="74669-108">Description</span></span>                      |
|:---------------------|:------------------------|:--------------------------------|
|[<span data-ttu-id="74669-109">Obter customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="74669-109">Get customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-get.md)      |<span data-ttu-id="74669-110">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="74669-110">customerPaymentJournals</span></span>|<span data-ttu-id="74669-111">Obtém um diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="74669-111">Gets a customer payment journal.</span></span>   |
|[<span data-ttu-id="74669-112">Postar customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="74669-112">Post customerPaymentJournals</span></span>](../api/dynamics-create-customerpaymentsjournal.md)  |<span data-ttu-id="74669-113">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="74669-113">customerPaymentJournals</span></span>|<span data-ttu-id="74669-114">Cria um diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="74669-114">Creates a customer payment journal.</span></span>|
|[<span data-ttu-id="74669-115">Patch customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="74669-115">Patch customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-update.md) |<span data-ttu-id="74669-116">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="74669-116">customerPaymentJournals</span></span>|<span data-ttu-id="74669-117">Atualiza um diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="74669-117">Updates a customer payment journal.</span></span>|
|[<span data-ttu-id="74669-118">Excluir customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="74669-118">Delete customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-delete.md)|<span data-ttu-id="74669-119">none</span><span class="sxs-lookup"><span data-stu-id="74669-119">none</span></span>                     |<span data-ttu-id="74669-120">Exclui um diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="74669-120">Deletes a customer payment journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="74669-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74669-121">Properties</span></span>
| <span data-ttu-id="74669-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74669-122">Property</span></span>           | <span data-ttu-id="74669-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="74669-123">Type</span></span>                  |<span data-ttu-id="74669-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="74669-124">Description</span></span>                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|<span data-ttu-id="74669-125">id</span><span class="sxs-lookup"><span data-stu-id="74669-125">id</span></span>                  |<span data-ttu-id="74669-126">GUID</span><span class="sxs-lookup"><span data-stu-id="74669-126">GUID</span></span>                   |<span data-ttu-id="74669-127">A ID exclusiva do diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="74669-127">The unique ID of the customer payment journal.</span></span> <span data-ttu-id="74669-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="74669-128">Non-editable.</span></span>           |
|<span data-ttu-id="74669-129">código</span><span class="sxs-lookup"><span data-stu-id="74669-129">code</span></span>                |<span data-ttu-id="74669-130">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="74669-130">string, maximum size 10</span></span>| <span data-ttu-id="74669-131">O código do diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="74669-131">The code of the customer payment journal.</span></span>                             |
|<span data-ttu-id="74669-132">displayName</span><span class="sxs-lookup"><span data-stu-id="74669-132">displayName</span></span>         |<span data-ttu-id="74669-133">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="74669-133">string, maximum size 50</span></span>| <span data-ttu-id="74669-134">O nome de exibição do diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="74669-134">The display name of the customer payment journal.</span></span>                     |
|<span data-ttu-id="74669-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74669-135">lastModifiedDateTime</span></span>|<span data-ttu-id="74669-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="74669-136">datetime</span></span>               |<span data-ttu-id="74669-137">O último DateTime que o diário de pagamentos do cliente foi modificado.</span><span class="sxs-lookup"><span data-stu-id="74669-137">The last datetime the customer payment journal was modified.</span></span> <span data-ttu-id="74669-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="74669-138">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74669-139">Relações</span><span class="sxs-lookup"><span data-stu-id="74669-139">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="74669-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74669-140">JSON representation</span></span>

<span data-ttu-id="74669-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74669-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

