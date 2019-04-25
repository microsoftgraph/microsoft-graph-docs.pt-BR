---
title: tipo de recurso customerPayments
description: Um objeto Customer Payments no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9063a9066c51956596e4f0aa918a2e7a53bf2ab9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543096"
---
# <a name="customerpayments-resource-type"></a><span data-ttu-id="7c2f1-103">tipo de recurso customerPayments</span><span class="sxs-lookup"><span data-stu-id="7c2f1-103">customerPayments resource type</span></span>
<span data-ttu-id="7c2f1-104">Representa um pagamento de cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-104">Represents a customer payment in Dynamics 365 Business Central.</span></span> <span data-ttu-id="7c2f1-105">Um pagamento de cliente é inserido como uma linha em um diário de pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-105">A customer payment is entered as a line in a customer payment journal.</span></span>

## <a name="methods"></a><span data-ttu-id="7c2f1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="7c2f1-106">Methods</span></span>

| <span data-ttu-id="7c2f1-107">Método</span><span class="sxs-lookup"><span data-stu-id="7c2f1-107">Method</span></span>         | <span data-ttu-id="7c2f1-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7c2f1-108">Return Type</span></span>  |<span data-ttu-id="7c2f1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c2f1-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="7c2f1-110">Obter customerPayments</span><span class="sxs-lookup"><span data-stu-id="7c2f1-110">Get customerPayments</span></span>](../api/dynamics-customerpayment-get.md)|<span data-ttu-id="7c2f1-111">customerPayments</span><span class="sxs-lookup"><span data-stu-id="7c2f1-111">customerPayments</span></span>|<span data-ttu-id="7c2f1-112">Obtém um pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-112">Gets a customer payment.</span></span>|
|[<span data-ttu-id="7c2f1-113">Postar customerPayments</span><span class="sxs-lookup"><span data-stu-id="7c2f1-113">Post customerPayments</span></span>](../api/dynamics-create-customerpayment.md)|<span data-ttu-id="7c2f1-114">customerPayments</span><span class="sxs-lookup"><span data-stu-id="7c2f1-114">customerPayments</span></span>|<span data-ttu-id="7c2f1-115">Cria um pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-115">Creates a customer payment.</span></span>|
|[<span data-ttu-id="7c2f1-116">Patch customerPayments</span><span class="sxs-lookup"><span data-stu-id="7c2f1-116">Patch customerPayments</span></span>](../api/dynamics-customerpayment-update.md)|<span data-ttu-id="7c2f1-117">customerPayments</span><span class="sxs-lookup"><span data-stu-id="7c2f1-117">customerPayments</span></span>|<span data-ttu-id="7c2f1-118">Atualiza um pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-118">Updates a customer payment.</span></span>|
|[<span data-ttu-id="7c2f1-119">Excluir customerPayments</span><span class="sxs-lookup"><span data-stu-id="7c2f1-119">Delete customerPayments</span></span>](../api/dynamics-customerpayment-delete.md)|<span data-ttu-id="7c2f1-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7c2f1-120">none</span></span>|<span data-ttu-id="7c2f1-121">Exclui um pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-121">Deletes a customer payment.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c2f1-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c2f1-122">Properties</span></span>
| <span data-ttu-id="7c2f1-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c2f1-123">Property</span></span>     | <span data-ttu-id="7c2f1-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c2f1-124">Type</span></span>    |<span data-ttu-id="7c2f1-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c2f1-125">Description</span></span>|
|:-------------|:--------|:----------|
|<span data-ttu-id="7c2f1-126">id</span><span class="sxs-lookup"><span data-stu-id="7c2f1-126">id</span></span>|<span data-ttu-id="7c2f1-127">GUID</span><span class="sxs-lookup"><span data-stu-id="7c2f1-127">GUID</span></span>|<span data-ttu-id="7c2f1-128">A ID exclusiva do pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-128">The unique ID of the customer payment.</span></span> <span data-ttu-id="7c2f1-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-129">Non-editable.</span></span>|
|<span data-ttu-id="7c2f1-130">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="7c2f1-130">journalDisplayName</span></span>|<span data-ttu-id="7c2f1-131">string</span><span class="sxs-lookup"><span data-stu-id="7c2f1-131">string</span></span>|<span data-ttu-id="7c2f1-132">O diário de pagamentos do cliente no qual o registro de pagamento é uma linha.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-132">The customer payment journal in which the payment record is a line.</span></span>|
|<span data-ttu-id="7c2f1-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="7c2f1-133">lineNumber</span></span>|<span data-ttu-id="7c2f1-134">inteiro</span><span class="sxs-lookup"><span data-stu-id="7c2f1-134">integer</span></span>|<span data-ttu-id="7c2f1-135">O número do pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-135">The number of the customer payment.</span></span>|
|<span data-ttu-id="7c2f1-136">Box</span><span class="sxs-lookup"><span data-stu-id="7c2f1-136">customerId</span></span>|<span data-ttu-id="7c2f1-137">GUID</span><span class="sxs-lookup"><span data-stu-id="7c2f1-137">GUID</span></span>|<span data-ttu-id="7c2f1-138">A ID exclusiva do cliente ao qual o pagamento está relacionado.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-138">The unique ID of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="7c2f1-139">customerNumber</span><span class="sxs-lookup"><span data-stu-id="7c2f1-139">customerNumber</span></span>|<span data-ttu-id="7c2f1-140">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="7c2f1-140">string, maximum size 20</span></span>|<span data-ttu-id="7c2f1-141">O número do cliente ao qual o pagamento está relacionado.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-141">The number of the customer that the payment is related to.</span></span>|
|<span data-ttu-id="7c2f1-142">ContactID</span><span class="sxs-lookup"><span data-stu-id="7c2f1-142">contactId</span></span>|<span data-ttu-id="7c2f1-143">Cadeia de caracteres, tamanho máximo 250</span><span class="sxs-lookup"><span data-stu-id="7c2f1-143">string, maximum size 250</span></span>|<span data-ttu-id="7c2f1-144">A ID de contato do Exchange para o cliente específico.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-144">The exchange contact id for the given customer.</span></span> <span data-ttu-id="7c2f1-145">Se uma ID de cliente não for especificada, usaremos a ID de contato para encontrá-la.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-145">If a customer id is not specified, we will use the contact id to find it.</span></span>|
|<span data-ttu-id="7c2f1-146">postingDate</span><span class="sxs-lookup"><span data-stu-id="7c2f1-146">postingDate</span></span>|<span data-ttu-id="7c2f1-147">data</span><span class="sxs-lookup"><span data-stu-id="7c2f1-147">date</span></span>|<span data-ttu-id="7c2f1-148">A data em que o pagamento do cliente é lançado.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-148">The date that the customer payment is posted.</span></span>|
|<span data-ttu-id="7c2f1-149">documentNumber</span><span class="sxs-lookup"><span data-stu-id="7c2f1-149">documentNumber</span></span>|<span data-ttu-id="7c2f1-150">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="7c2f1-150">string, maximum size 20</span></span>|<span data-ttu-id="7c2f1-151">Especifica um número de documento para o pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-151">Specifies a document number for the customer payment.</span></span>|
|<span data-ttu-id="7c2f1-152">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="7c2f1-152">externalDocumentNumber</span></span>|<span data-ttu-id="7c2f1-153">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="7c2f1-153">string, maximum size 20</span></span>|<span data-ttu-id="7c2f1-154">Especifica um número de documento externo para o pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-154">Specifies an external document number for the customer payment.</span></span>|
|<span data-ttu-id="7c2f1-155">quantia</span><span class="sxs-lookup"><span data-stu-id="7c2f1-155">amount</span></span>|<span data-ttu-id="7c2f1-156">dígitos</span><span class="sxs-lookup"><span data-stu-id="7c2f1-156">decimal</span></span>|<span data-ttu-id="7c2f1-157">Especifica o valor total (incluindo o IVA) que o pagamento do cliente consiste.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-157">Specifies the total amount (including VAT) that the customer payment consists of.</span></span>|
|<span data-ttu-id="7c2f1-158">appliesToInvoiceId</span><span class="sxs-lookup"><span data-stu-id="7c2f1-158">appliesToInvoiceId</span></span>|<span data-ttu-id="7c2f1-159">GUID</span><span class="sxs-lookup"><span data-stu-id="7c2f1-159">GUID</span></span>|<span data-ttu-id="7c2f1-160">A identificação exclusiva da fatura à qual o pagamento está relacionado.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-160">The unique ID of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="7c2f1-161">appliesToInvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="7c2f1-161">appliesToInvoiceNumber</span></span>|<span data-ttu-id="7c2f1-162">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="7c2f1-162">string, maximum size 20</span></span>|<span data-ttu-id="7c2f1-163">O número da fatura à qual o pagamento está relacionado.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-163">The number of the invoice that the payment is related to.</span></span>|
|<span data-ttu-id="7c2f1-164">description</span><span class="sxs-lookup"><span data-stu-id="7c2f1-164">description</span></span>|<span data-ttu-id="7c2f1-165">Cadeia de caracteres, tamanho máximo 50</span><span class="sxs-lookup"><span data-stu-id="7c2f1-165">string, maximum size 50</span></span>|<span data-ttu-id="7c2f1-166">A descrição do pagamento do cliente, fornecida pelo usuário ou pela autocriação.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-166">The description of the customer payment, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="7c2f1-167">comment</span><span class="sxs-lookup"><span data-stu-id="7c2f1-167">comment</span></span>|<span data-ttu-id="7c2f1-168">Cadeia de caracteres, tamanho máximo 250</span><span class="sxs-lookup"><span data-stu-id="7c2f1-168">string, maximum size 250</span></span>|<span data-ttu-id="7c2f1-169">Um comentário especificado pelo usuário no pagamento do cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-169">A user specified comment on the customer payment.</span></span>|
|<span data-ttu-id="7c2f1-170">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c2f1-170">lastModifiedDateTime</span></span>|<span data-ttu-id="7c2f1-171">DateTime</span><span class="sxs-lookup"><span data-stu-id="7c2f1-171">datetime</span></span>|<span data-ttu-id="7c2f1-172">O último DateTime que o pagamento do cliente foi modificado.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-172">The last datetime the customer payment was modified.</span></span> <span data-ttu-id="7c2f1-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-173">Read-Only.</span></span>|


## <a name="relationships"></a><span data-ttu-id="7c2f1-174">Relações</span><span class="sxs-lookup"><span data-stu-id="7c2f1-174">Relationships</span></span>
<span data-ttu-id="7c2f1-175">Um pagamento de cliente é uma subpágina de um diário de pagamento de cliente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-175">A customer payment is a subpage of a customer payment journal.</span></span> <span data-ttu-id="7c2f1-176">Ele não pode ser acessado diretamente.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-176">It cannot be accessed directly.</span></span>

<span data-ttu-id="7c2f1-177">Um pagamento de cliente pode ser uma "entidade pai" das linhas de dimensão.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-177">A customer payment can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="7c2f1-178">Um cliente (customerId) deve existir na tabela Customers.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-178">A Customer (customerId) must exist in the Customers table.</span></span>

<span data-ttu-id="7c2f1-179">Uma fatura (appliesToInvoiceId) deve existir na tabela faturas de vendas.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-179">An Invoice (appliesToInvoiceId) must exist in the Sales Invoices Table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7c2f1-180">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c2f1-180">JSON representation</span></span>

<span data-ttu-id="7c2f1-181">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c2f1-181">Here is a JSON representation of the resource.</span></span>

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

