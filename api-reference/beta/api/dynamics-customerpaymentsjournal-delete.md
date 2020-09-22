---
title: Excluir customerPaymentJournals
description: Exclui um diário de pagamento do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2cdc8058b2a3069695ecc543d07d7fd543eab70a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981405"
---
# <a name="delete-customerpaymentjournals"></a><span data-ttu-id="eaaf0-103">Excluir customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="eaaf0-103">Delete customerPaymentJournals</span></span>

<span data-ttu-id="eaaf0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaaf0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eaaf0-105">Excluir um objeto de diário de pagamento de cliente do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-105">Delete a customer payment journal object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaaf0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eaaf0-106">Permissions</span></span>
<span data-ttu-id="eaaf0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaaf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaaf0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eaaf0-109">Permission type</span></span> |<span data-ttu-id="eaaf0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eaaf0-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="eaaf0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eaaf0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eaaf0-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaaf0-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="eaaf0-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="eaaf0-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="eaaf0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-114">Not supported.</span></span>|
|<span data-ttu-id="eaaf0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eaaf0-115">Application</span></span>|<span data-ttu-id="eaaf0-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaaf0-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaaf0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eaaf0-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eaaf0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eaaf0-118">Optional query parameters</span></span>
<span data-ttu-id="eaaf0-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eaaf0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eaaf0-120">Request headers</span></span>
|<span data-ttu-id="eaaf0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eaaf0-121">Header</span></span>       |<span data-ttu-id="eaaf0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="eaaf0-122">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="eaaf0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eaaf0-123">Authorization</span></span>|<span data-ttu-id="eaaf0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="eaaf0-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="eaaf0-126">If-Match</span></span>     |<span data-ttu-id="eaaf0-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-127">Required.</span></span> <span data-ttu-id="eaaf0-128">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **customerPaymentJournals**, o **customerPaymentJournals** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-128">When this request header is included and the eTag provided does not match the current tag on the **customerPaymentJournals**, the **customerPaymentJournals** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaaf0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eaaf0-129">Request body</span></span>

<span data-ttu-id="eaaf0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eaaf0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="eaaf0-131">Response</span></span>

<span data-ttu-id="eaaf0-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaaf0-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eaaf0-134">Example</span></span>

<span data-ttu-id="eaaf0-135">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="eaaf0-135">**Request**</span></span>

<span data-ttu-id="eaaf0-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}
```

<span data-ttu-id="eaaf0-137">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="eaaf0-137">**Response**</span></span> 

<span data-ttu-id="eaaf0-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eaaf0-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```



