---
title: Criar journalLines
description: Cria uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 2350bb112b0585e822c4c4c92af5511705b3612c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431379"
---
# <a name="create-journallines"></a><span data-ttu-id="c7e76-103">Criar journalLines</span><span class="sxs-lookup"><span data-stu-id="c7e76-103">Create journalLines</span></span>

<span data-ttu-id="c7e76-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7e76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7e76-105">Cria um objeto de linha de diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="c7e76-105">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7e76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7e76-106">Permissions</span></span>
<span data-ttu-id="c7e76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7e76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7e76-109">Permission type</span></span> |<span data-ttu-id="c7e76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7e76-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c7e76-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7e76-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c7e76-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7e76-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c7e76-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="c7e76-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c7e76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7e76-114">Not supported.</span></span>|
|<span data-ttu-id="c7e76-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7e76-115">Application</span></span>|<span data-ttu-id="c7e76-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7e76-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7e76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7e76-117">HTTP request</span></span>

```
POST /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7e76-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7e76-118">Optional query parameters</span></span>
<span data-ttu-id="c7e76-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7e76-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7e76-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e76-120">Request headers</span></span>
|<span data-ttu-id="c7e76-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7e76-121">Header</span></span>        |<span data-ttu-id="c7e76-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c7e76-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="c7e76-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7e76-123">Authorization</span></span> |<span data-ttu-id="c7e76-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7e76-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c7e76-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c7e76-126">Content-Type</span></span>  |<span data-ttu-id="c7e76-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7e76-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="c7e76-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7e76-128">Request body</span></span>
<span data-ttu-id="c7e76-129">No corpo da solicitação, forneça uma representação JSON do objeto **journalLines** .</span><span class="sxs-lookup"><span data-stu-id="c7e76-129">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="c7e76-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7e76-130">Response</span></span>
<span data-ttu-id="c7e76-131">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e o objeto **journalLines** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7e76-131">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e76-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7e76-132">Example</span></span>

<span data-ttu-id="c7e76-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c7e76-133">**Request**</span></span>

<span data-ttu-id="c7e76-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7e76-134">Here is an example of a request.</span></span>

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
<span data-ttu-id="c7e76-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="c7e76-135">**Response**</span></span>

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


