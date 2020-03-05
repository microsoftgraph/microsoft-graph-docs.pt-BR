---
title: tipo de recurso customerPayments
description: Um objeto Customer Payments no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bd990ea9778ada7d43c9b8192d77cf8af618909b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504633"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="eb5d2-103">tipo de recurso customerPayments</span><span class="sxs-lookup"><span data-stu-id="eb5d2-103">customerPayments resource type</span></span>

<span data-ttu-id="eb5d2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eb5d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb5d2-105">Representa um pagamento de cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-105">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="eb5d2-106">Um pagamento de cliente é inserido como uma linha em um diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-106">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="eb5d2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb5d2-107">Methods</span></span>

| <span data-ttu-id="eb5d2-108">Método</span><span class="sxs-lookup"><span data-stu-id="eb5d2-108">Method</span></span>         | <span data-ttu-id="eb5d2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb5d2-109">Return Type</span></span>  |<span data-ttu-id="eb5d2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb5d2-110">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="eb5d2-111">Obter customerPayments</span><span class="sxs-lookup"><span data-stu-id="eb5d2-111">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="eb5d2-112">customerPayments</span><span class="sxs-lookup"><span data-stu-id="eb5d2-112">customerPayments</span></span>|<span data-ttu-id="eb5d2-113">Obtém um pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-113">Gets a customer payment.</span></span>|
|[<span data-ttu-id="eb5d2-114">Postar customerPayments</span><span class="sxs-lookup"><span data-stu-id="eb5d2-114">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="eb5d2-115">customerPayments</span><span class="sxs-lookup"><span data-stu-id="eb5d2-115">customerPayments</span></span>|<span data-ttu-id="eb5d2-116">Cria um pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-116">Creates a customer payment.</span></span>|
|[<span data-ttu-id="eb5d2-117">Patch customerPayments</span><span class="sxs-lookup"><span data-stu-id="eb5d2-117">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="eb5d2-118">customerPayments</span><span class="sxs-lookup"><span data-stu-id="eb5d2-118">customerPayments</span></span>|<span data-ttu-id="eb5d2-119">Atualiza um pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-119">Updates a customer payment.</span></span>|
|[<span data-ttu-id="eb5d2-120">Excluir customerPayments</span><span class="sxs-lookup"><span data-stu-id="eb5d2-120">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="eb5d2-121">nenhuma</span><span class="sxs-lookup"><span data-stu-id="eb5d2-121">none</span></span>|<span data-ttu-id="eb5d2-122">Exclui um pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-122">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb5d2-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb5d2-123">Properties</span></span>
| <span data-ttu-id="eb5d2-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb5d2-124">Property</span></span>     | <span data-ttu-id="eb5d2-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb5d2-125">Type</span></span>    |<span data-ttu-id="eb5d2-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb5d2-126">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="eb5d2-127">id</span><span class="sxs-lookup"><span data-stu-id="eb5d2-127">id</span></span>|<span data-ttu-id="eb5d2-128">GUID</span><span class="sxs-lookup"><span data-stu-id="eb5d2-128">GUID</span></span>|<span data-ttu-id="eb5d2-129">A ID exclusiva do pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-129">The unique ID of the customer payment.</span></span> <span data-ttu-id="eb5d2-130">Não editável.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-130">Non-editable.</span></span>|
|<span data-ttu-id="eb5d2-131">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="eb5d2-131">journalDisplayName</span></span>|<span data-ttu-id="eb5d2-132">string</span><span class="sxs-lookup"><span data-stu-id="eb5d2-132">string</span></span>|<span data-ttu-id="eb5d2-133">O diário de pagamentos do cliente no qual o registro de pagamento é uma linha.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-133">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="eb5d2-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="eb5d2-134">lineNumber</span></span>|<span data-ttu-id="eb5d2-135">inteiro</span><span class="sxs-lookup"><span data-stu-id="eb5d2-135">integer</span></span>|<span data-ttu-id="eb5d2-136">O número do pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-136">The number of the customer payment.</span></span>|
|<span data-ttu-id="eb5d2-137">Box</span><span class="sxs-lookup"><span data-stu-id="eb5d2-137">customerId</span></span>|<span data-ttu-id="eb5d2-138">GUID</span><span class="sxs-lookup"><span data-stu-id="eb5d2-138">GUID</span></span>|<span data-ttu-id="eb5d2-139">A ID exclusiva do cliente ao qual o pagamento está relacionado.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-139">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="eb5d2-140">customerNumber</span><span class="sxs-lookup"><span data-stu-id="eb5d2-140">customerNumber</span></span>|<span data-ttu-id="eb5d2-141">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="eb5d2-141">string, maximum size 20</span></span>|<span data-ttu-id="eb5d2-142">O número do cliente ao qual o pagamento está relacionado.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-142">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="eb5d2-143">ContactID</span><span class="sxs-lookup"><span data-stu-id="eb5d2-143">contactId</span></span>|<span data-ttu-id="eb5d2-144">Cadeia de caracteres, tamanho máximo 250</span><span class="sxs-lookup"><span data-stu-id="eb5d2-144">string, maximum size 250</span></span>|<span data-ttu-id="eb5d2-145">A ID de contato do Exchange para o cliente específico.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-145">The exchange contact id for the given customer.</span></span> <span data-ttu-id="eb5d2-146">Se uma ID de cliente não for especificada, usaremos a ID de contato para encontrá-la.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-146">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="eb5d2-147">postingDate</span><span class="sxs-lookup"><span data-stu-id="eb5d2-147">postingDate</span></span>|<span data-ttu-id="eb5d2-148">data</span><span class="sxs-lookup"><span data-stu-id="eb5d2-148">date</span></span>|<span data-ttu-id="eb5d2-149">A data em que o pagamento do cliente é lançado.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-149">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="eb5d2-150">documentNumber</span><span class="sxs-lookup"><span data-stu-id="eb5d2-150">documentNumber</span></span>|<span data-ttu-id="eb5d2-151">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="eb5d2-151">string, maximum size 20</span></span>|<span data-ttu-id="eb5d2-152">Especifica um número de documento para o pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-152">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="eb5d2-153">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="eb5d2-153">externalDocumentNumber</span></span>|<span data-ttu-id="eb5d2-154">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="eb5d2-154">string, maximum size 20</span></span>|<span data-ttu-id="eb5d2-155">Especifica um número de documento externo para o pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-155">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="eb5d2-156">quantia</span><span class="sxs-lookup"><span data-stu-id="eb5d2-156">amount</span></span>|<span data-ttu-id="eb5d2-157">dígitos</span><span class="sxs-lookup"><span data-stu-id="eb5d2-157">decimal</span></span>|<span data-ttu-id="eb5d2-158">Especifica o valor total (incluindo o IVA) que o pagamento do cliente consiste.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-158">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="eb5d2-159">appliesToInvoiceId</span><span class="sxs-lookup"><span data-stu-id="eb5d2-159">appliesToInvoiceId</span></span>|<span data-ttu-id="eb5d2-160">GUID</span><span class="sxs-lookup"><span data-stu-id="eb5d2-160">GUID</span></span>|<span data-ttu-id="eb5d2-161">A identificação exclusiva da fatura à qual o pagamento está relacionado.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-161">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="eb5d2-162">appliesToInvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="eb5d2-162">appliesToInvoiceNumber</span></span>|<span data-ttu-id="eb5d2-163">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="eb5d2-163">string, maximum size 20</span></span>|<span data-ttu-id="eb5d2-164">O número da fatura à qual o pagamento está relacionado.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-164">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="eb5d2-165">description</span><span class="sxs-lookup"><span data-stu-id="eb5d2-165">description</span></span>|<span data-ttu-id="eb5d2-166">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="eb5d2-166">string, maximum size 50</span></span>|<span data-ttu-id="eb5d2-167">A descrição do pagamento do cliente, fornecida pelo usuário ou pela autocriação.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-167">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="eb5d2-168">comment</span><span class="sxs-lookup"><span data-stu-id="eb5d2-168">comment</span></span>|<span data-ttu-id="eb5d2-169">Cadeia de caracteres, tamanho máximo 250</span><span class="sxs-lookup"><span data-stu-id="eb5d2-169">string, maximum size 250</span></span>|<span data-ttu-id="eb5d2-170">Um comentário especificado pelo usuário no pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-170">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="eb5d2-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb5d2-171">lastModifiedDateTime</span></span>|<span data-ttu-id="eb5d2-172">datetime</span><span class="sxs-lookup"><span data-stu-id="eb5d2-172">datetime</span></span>|<span data-ttu-id="eb5d2-173">O último DateTime que o pagamento do cliente foi modificado.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-173">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="eb5d2-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-174">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="eb5d2-175">Relações</span><span class="sxs-lookup"><span data-stu-id="eb5d2-175">Relationships</span></span>
<span data-ttu-id="eb5d2-176">Um pagamento de cliente é uma subpágina de um diário de pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-176">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="eb5d2-177">Ele não pode ser acessado diretamente.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-177">It cannot be accessed directly.</span></span>

<span data-ttu-id="eb5d2-178">Um pagamento de cliente pode ser uma "entidade pai" das linhas de dimensão.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-178">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="eb5d2-179">Um cliente (customerId) deve existir na tabela Customers.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-179">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="eb5d2-180">Uma fatura (appliesToInvoiceId) deve existir na tabela faturas de vendas.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-180">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="eb5d2-181">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb5d2-181">JSON representation</span></span>

<span data-ttu-id="eb5d2-182">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb5d2-182">Here is a JSON representation of the resource.</span></span>

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

