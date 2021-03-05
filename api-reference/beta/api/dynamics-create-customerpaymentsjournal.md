---
title: Criar customerPaymentJournals
description: Cria um objeto de diário de pagamentos do cliente no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 8041463e58ff9d81d04f771d21bea313f6829620
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473333"
---
# <a name="create-customerpaymentjournals"></a><span data-ttu-id="9996e-103">Criar customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="9996e-103">Create customerPaymentJournals</span></span>

<span data-ttu-id="9996e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9996e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9996e-105">Cria um objeto de diário de pagamento do cliente no Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="9996e-105">Creates a customer payment journal object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="9996e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9996e-106">Permissions</span></span>
<span data-ttu-id="9996e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9996e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9996e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9996e-109">Permission type</span></span> |<span data-ttu-id="9996e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9996e-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="9996e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9996e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9996e-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9996e-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="9996e-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="9996e-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9996e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9996e-114">Not supported.</span></span>|
|<span data-ttu-id="9996e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9996e-115">Application</span></span>|<span data-ttu-id="9996e-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9996e-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9996e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9996e-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9996e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9996e-118">Optional query parameters</span></span>
<span data-ttu-id="9996e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9996e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9996e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9996e-120">Request headers</span></span>
|<span data-ttu-id="9996e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9996e-121">Header</span></span>        |<span data-ttu-id="9996e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9996e-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="9996e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9996e-123">Authorization</span></span> |<span data-ttu-id="9996e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9996e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9996e-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9996e-126">Content-Type</span></span>  |<span data-ttu-id="9996e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9996e-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="9996e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9996e-128">Request body</span></span>
<span data-ttu-id="9996e-129">No corpo da solicitação, fornece uma representação JSON do **objeto customerPaymentJournals.**</span><span class="sxs-lookup"><span data-stu-id="9996e-129">In the request body, supply a JSON representation of **customerPaymentJournals** object.</span></span>

## <a name="response"></a><span data-ttu-id="9996e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9996e-130">Response</span></span>
<span data-ttu-id="9996e-131">Se tiver êxito, este método retornará ```201 Created``` o código de resposta e um objeto **customerPaymentJournals** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9996e-131">If successful, this method returns ```201 Created``` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9996e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9996e-132">Example</span></span>

<span data-ttu-id="9996e-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="9996e-133">**Request**</span></span>

<span data-ttu-id="9996e-134">Aqui está um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="9996e-134">Here is an example of a request.</span></span>

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals
Content-type: application/json

{
  "code": "DEFAULT"
}
```

<span data-ttu-id="9996e-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="9996e-135">**Response**</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```




