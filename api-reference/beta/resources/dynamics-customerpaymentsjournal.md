---
title: tipo de recurso customerPaymentJournals
description: Um diário de pagamentos do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a8b01124db732866e1a7b971af57d7e0a2b692e1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507249"
---
# <a name="customerpaymentsjournals-resource-type"></a><span data-ttu-id="47f76-103">tipo de recurso customerPaymentsJournals</span><span class="sxs-lookup"><span data-stu-id="47f76-103">customerPaymentsJournals resource type</span></span>
<span data-ttu-id="47f76-104">Representa um diário de pagamento do cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="47f76-104">Represents a customer payment journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="47f76-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="47f76-105">Methods</span></span>

| <span data-ttu-id="47f76-106">Método</span><span class="sxs-lookup"><span data-stu-id="47f76-106">Method</span></span>               | <span data-ttu-id="47f76-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="47f76-107">Return Type</span></span>             |<span data-ttu-id="47f76-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="47f76-108">Description</span></span>                      |
|:---------------------|:------------------------|:--------------------------------|
|[<span data-ttu-id="47f76-109">Obter customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="47f76-109">Get customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-get.md)      |<span data-ttu-id="47f76-110">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="47f76-110">customerPaymentJournals</span></span>|<span data-ttu-id="47f76-111">Obtém um diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="47f76-111">Gets a customer payment journal.</span></span>   |
|[<span data-ttu-id="47f76-112">Postar customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="47f76-112">Post customerPaymentJournals</span></span>](../api/dynamics-create-customerpaymentsjournal.md)  |<span data-ttu-id="47f76-113">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="47f76-113">customerPaymentJournals</span></span>|<span data-ttu-id="47f76-114">Cria um diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="47f76-114">Creates a customer payment journal.</span></span>|
|[<span data-ttu-id="47f76-115">Patch customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="47f76-115">Patch customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-update.md) |<span data-ttu-id="47f76-116">customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="47f76-116">customerPaymentJournals</span></span>|<span data-ttu-id="47f76-117">Atualiza um diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="47f76-117">Updates a customer payment journal.</span></span>|
|[<span data-ttu-id="47f76-118">Excluir customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="47f76-118">Delete customerPaymentJournals</span></span>](../api/dynamics-customerpaymentsjournal-delete.md)|<span data-ttu-id="47f76-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="47f76-119">none</span></span>                     |<span data-ttu-id="47f76-120">Exclui um diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="47f76-120">Deletes a customer payment journal.</span></span>|

## <a name="properties"></a><span data-ttu-id="47f76-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47f76-121">Properties</span></span>
| <span data-ttu-id="47f76-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47f76-122">Property</span></span>           | <span data-ttu-id="47f76-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="47f76-123">Type</span></span>                  |<span data-ttu-id="47f76-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="47f76-124">Description</span></span>                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|<span data-ttu-id="47f76-125">id</span><span class="sxs-lookup"><span data-stu-id="47f76-125">id</span></span>                  |<span data-ttu-id="47f76-126">GUID</span><span class="sxs-lookup"><span data-stu-id="47f76-126">GUID</span></span>                   |<span data-ttu-id="47f76-127">A ID exclusiva do diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="47f76-127">The unique ID of the customer payment journal.</span></span> <span data-ttu-id="47f76-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="47f76-128">Non-editable.</span></span>           |
|<span data-ttu-id="47f76-129">code</span><span class="sxs-lookup"><span data-stu-id="47f76-129">code</span></span>                |<span data-ttu-id="47f76-130">Cadeia de caracteres, tamanho máximo 10</span><span class="sxs-lookup"><span data-stu-id="47f76-130">string, maximum size 10</span></span>| <span data-ttu-id="47f76-131">O código do diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="47f76-131">The code of the customer payment journal.</span></span>                             |
|<span data-ttu-id="47f76-132">displayName</span><span class="sxs-lookup"><span data-stu-id="47f76-132">displayName</span></span>         |<span data-ttu-id="47f76-133">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="47f76-133">string, maximum size 50</span></span>| <span data-ttu-id="47f76-134">O nome de exibição do diário de pagamentos do cliente.</span><span class="sxs-lookup"><span data-stu-id="47f76-134">The display name of the customer payment journal.</span></span>                     |
|<span data-ttu-id="47f76-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47f76-135">lastModifiedDateTime</span></span>|<span data-ttu-id="47f76-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="47f76-136">datetime</span></span>               |<span data-ttu-id="47f76-137">O último DateTime que o diário de pagamentos do cliente foi modificado.</span><span class="sxs-lookup"><span data-stu-id="47f76-137">The last datetime the customer payment journal was modified.</span></span> <span data-ttu-id="47f76-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47f76-138">Read-Only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47f76-139">Relações</span><span class="sxs-lookup"><span data-stu-id="47f76-139">Relationships</span></span>

## <a name="json-representation"></a><span data-ttu-id="47f76-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47f76-140">JSON representation</span></span>

<span data-ttu-id="47f76-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47f76-141">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

