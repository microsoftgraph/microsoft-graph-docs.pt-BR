---
title: Obter customerPaymentJournals
description: Obtém um diário de pagamento do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 63844cd7b18201c47a2ed27480fe9db2bc5bc107
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42430543"
---
# <a name="get-customerpaymentjournals"></a><span data-ttu-id="b6d3f-103">Obter customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="b6d3f-103">Get customerPaymentJournals</span></span>

<span data-ttu-id="b6d3f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6d3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6d3f-105">Recupere as propriedades e os relacionamentos de um objeto de diário de pagamento do cliente para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-105">Retrieve the properties and relationships of a customer payment journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="b6d3f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6d3f-106">Permissions</span></span>
<span data-ttu-id="b6d3f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6d3f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6d3f-109">Permission type</span></span> |<span data-ttu-id="b6d3f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6d3f-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="b6d3f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6d3f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b6d3f-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6d3f-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="b6d3f-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="b6d3f-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b6d3f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-114">Not supported.</span></span>|
|<span data-ttu-id="b6d3f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6d3f-115">Application</span></span>|<span data-ttu-id="b6d3f-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6d3f-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6d3f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6d3f-117">HTTP request</span></span>

```
GET /financials/companies/{id}/customerPaymentJournals/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6d3f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b6d3f-118">Optional query parameters</span></span>
<span data-ttu-id="b6d3f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6d3f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d3f-120">Request headers</span></span>
|<span data-ttu-id="b6d3f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6d3f-121">Header</span></span>       |<span data-ttu-id="b6d3f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6d3f-122">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="b6d3f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6d3f-123">Authorization</span></span>|<span data-ttu-id="b6d3f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6d3f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6d3f-126">Request body</span></span>
<span data-ttu-id="b6d3f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6d3f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6d3f-128">Response</span></span>
<span data-ttu-id="b6d3f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **customerPaymentJournals** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-129">If successful, this method returns a `200 OK` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6d3f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6d3f-130">Example</span></span>

<span data-ttu-id="b6d3f-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="b6d3f-131">**Request**</span></span>

<span data-ttu-id="b6d3f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-132">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/customerPaymentJournals/{id}
```

<span data-ttu-id="b6d3f-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="b6d3f-133">**Response**</span></span>

<span data-ttu-id="b6d3f-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="b6d3f-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b6d3f-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6d3f-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```
