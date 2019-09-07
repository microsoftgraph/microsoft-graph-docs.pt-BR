---
title: Criar journalLines
description: Cria uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: c0d047840143c87618eb33fc1ee9d0bc074f3f7e
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791950"
---
# <a name="create-journallines"></a><span data-ttu-id="4791a-103">Criar journalLines</span><span class="sxs-lookup"><span data-stu-id="4791a-103">Create journalLines</span></span>
<span data-ttu-id="4791a-104">Cria um objeto de linha de diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="4791a-104">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="4791a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4791a-105">Permissions</span></span>
<span data-ttu-id="4791a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4791a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4791a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4791a-108">Permission type</span></span> |<span data-ttu-id="4791a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4791a-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="4791a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4791a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4791a-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4791a-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="4791a-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="4791a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4791a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4791a-113">Not supported.</span></span>|
|<span data-ttu-id="4791a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4791a-114">Application</span></span>|<span data-ttu-id="4791a-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4791a-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4791a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4791a-116">HTTP request</span></span>

```
POST /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4791a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4791a-117">Optional query parameters</span></span>
<span data-ttu-id="4791a-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4791a-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4791a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4791a-119">Request headers</span></span>
|<span data-ttu-id="4791a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4791a-120">Header</span></span>        |<span data-ttu-id="4791a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4791a-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="4791a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4791a-122">Authorization</span></span> |<span data-ttu-id="4791a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4791a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4791a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4791a-125">Content-Type</span></span>  |<span data-ttu-id="4791a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4791a-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="4791a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4791a-127">Request body</span></span>
<span data-ttu-id="4791a-128">No corpo da solicitação, forneça uma representação JSON do objeto **journalLines** .</span><span class="sxs-lookup"><span data-stu-id="4791a-128">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="4791a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4791a-129">Response</span></span>
<span data-ttu-id="4791a-130">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e o objeto **journalLines** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4791a-130">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4791a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4791a-131">Example</span></span>

<span data-ttu-id="4791a-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="4791a-132">**Request**</span></span>

<span data-ttu-id="4791a-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="4791a-133">Here is an example of a request.</span></span>

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
<span data-ttu-id="4791a-134">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="4791a-134">**Response**</span></span>

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


