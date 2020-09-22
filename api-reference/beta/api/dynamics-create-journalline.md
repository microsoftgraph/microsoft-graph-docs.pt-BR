---
title: Criar journalLines
description: Cria uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: cb188423bbbdcc90a71442f6a0e80ba70dcbc42d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981659"
---
# <a name="create-journallines"></a><span data-ttu-id="cc16b-103">Criar journalLines</span><span class="sxs-lookup"><span data-stu-id="cc16b-103">Create journalLines</span></span>

<span data-ttu-id="cc16b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc16b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc16b-105">Cria um objeto de linha de diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="cc16b-105">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc16b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc16b-106">Permissions</span></span>
<span data-ttu-id="cc16b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc16b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc16b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc16b-109">Permission type</span></span> |<span data-ttu-id="cc16b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc16b-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="cc16b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc16b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cc16b-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc16b-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="cc16b-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="cc16b-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cc16b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc16b-114">Not supported.</span></span>|
|<span data-ttu-id="cc16b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc16b-115">Application</span></span>|<span data-ttu-id="cc16b-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc16b-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc16b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc16b-117">HTTP request</span></span>

```
POST /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc16b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc16b-118">Optional query parameters</span></span>
<span data-ttu-id="cc16b-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc16b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc16b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc16b-120">Request headers</span></span>
|<span data-ttu-id="cc16b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc16b-121">Header</span></span>        |<span data-ttu-id="cc16b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cc16b-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="cc16b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc16b-123">Authorization</span></span> |<span data-ttu-id="cc16b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc16b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cc16b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc16b-126">Content-Type</span></span>  |<span data-ttu-id="cc16b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cc16b-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="cc16b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc16b-128">Request body</span></span>
<span data-ttu-id="cc16b-129">No corpo da solicitação, forneça uma representação JSON do objeto **journalLines** .</span><span class="sxs-lookup"><span data-stu-id="cc16b-129">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="cc16b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc16b-130">Response</span></span>
<span data-ttu-id="cc16b-131">Se bem-sucedido, este método retorna o ```201 Created``` código de resposta e o objeto **journalLines** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc16b-131">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc16b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc16b-132">Example</span></span>

<span data-ttu-id="cc16b-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="cc16b-133">**Request**</span></span>

<span data-ttu-id="cc16b-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc16b-134">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines
Content-type: application/json

{
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": ""
}
```
<span data-ttu-id="cc16b-135">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="cc16b-135">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "id-value",
  "accountNumber": "10400",
  "postingDate": "2015-12-31",
  "documentNumber": "1234",
  "externalDocumentNumber": "",
  "amount": 1500,
  "description": "Accounts Receivable",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```




