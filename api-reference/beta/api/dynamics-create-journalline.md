---
title: Criar journalLines
description: Cria uma linha de diário no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 38feb577f11f482fe00c5d44d883e1b0995ff562
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473263"
---
# <a name="create-journallines"></a><span data-ttu-id="bb7c6-103">Criar journalLines</span><span class="sxs-lookup"><span data-stu-id="bb7c6-103">Create journalLines</span></span>

<span data-ttu-id="bb7c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb7c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb7c6-105">Cria um objeto de linha de diário no Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="bb7c6-105">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb7c6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb7c6-106">Permissions</span></span>
<span data-ttu-id="bb7c6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb7c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb7c6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb7c6-109">Permission type</span></span> |<span data-ttu-id="bb7c6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb7c6-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="bb7c6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb7c6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb7c6-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb7c6-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="bb7c6-113">Delegada (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="bb7c6-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bb7c6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb7c6-114">Not supported.</span></span>|
|<span data-ttu-id="bb7c6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb7c6-115">Application</span></span>|<span data-ttu-id="bb7c6-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb7c6-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb7c6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb7c6-117">HTTP request</span></span>

```http
POST /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb7c6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bb7c6-118">Optional query parameters</span></span>
<span data-ttu-id="bb7c6-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bb7c6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb7c6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb7c6-120">Request headers</span></span>
|<span data-ttu-id="bb7c6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bb7c6-121">Header</span></span>        |<span data-ttu-id="bb7c6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bb7c6-122">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="bb7c6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb7c6-123">Authorization</span></span> |<span data-ttu-id="bb7c6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb7c6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bb7c6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bb7c6-126">Content-Type</span></span>  |<span data-ttu-id="bb7c6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bb7c6-127">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="bb7c6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb7c6-128">Request body</span></span>
<span data-ttu-id="bb7c6-129">No corpo da solicitação, fornece uma representação JSON do **objeto journalLines.**</span><span class="sxs-lookup"><span data-stu-id="bb7c6-129">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="bb7c6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb7c6-130">Response</span></span>
<span data-ttu-id="bb7c6-131">Se tiver êxito, este método retornará o código de resposta e o ```201 Created``` **objeto journalLines** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb7c6-131">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb7c6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb7c6-132">Example</span></span>

<span data-ttu-id="bb7c6-133">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="bb7c6-133">**Request**</span></span>

<span data-ttu-id="bb7c6-134">Aqui está um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb7c6-134">Here is an example of a request.</span></span>

```http
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
<span data-ttu-id="bb7c6-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="bb7c6-135">**Response**</span></span>

```http
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




