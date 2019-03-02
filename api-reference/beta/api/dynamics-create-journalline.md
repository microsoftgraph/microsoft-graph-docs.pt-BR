---
title: Criar journalLines
description: Cria uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: c6ed8b1ccbe1f33cad174e1c5e4f9b3832f2a5c9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365420"
---
# <a name="create-journallines"></a><span data-ttu-id="8cec2-103">Criar journalLines</span><span class="sxs-lookup"><span data-stu-id="8cec2-103">Create journalLines</span></span>
<span data-ttu-id="8cec2-104">Cria um objeto de linha de diário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="8cec2-104">Creates a journal line object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cec2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cec2-105">Permissions</span></span>
<span data-ttu-id="8cec2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cec2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cec2-108">Permission type</span></span> |<span data-ttu-id="8cec2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cec2-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="8cec2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cec2-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8cec2-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cec2-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="8cec2-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8cec2-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8cec2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cec2-113">Not supported.</span></span>|
|<span data-ttu-id="8cec2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cec2-114">Application</span></span>|<span data-ttu-id="8cec2-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cec2-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cec2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cec2-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8cec2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8cec2-117">Optional query parameters</span></span>
<span data-ttu-id="8cec2-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8cec2-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cec2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cec2-119">Request headers</span></span>
|<span data-ttu-id="8cec2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cec2-120">Header</span></span>        |<span data-ttu-id="8cec2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8cec2-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="8cec2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cec2-122">Authorization</span></span> |<span data-ttu-id="8cec2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cec2-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8cec2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cec2-125">Content-Type</span></span>  |<span data-ttu-id="8cec2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cec2-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="8cec2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cec2-127">Request body</span></span>
<span data-ttu-id="8cec2-128">No corpo da solicitação, forneça uma representação JSON do objeto **journalLines** .</span><span class="sxs-lookup"><span data-stu-id="8cec2-128">In the request body, supply a JSON representation of **journalLines** object.</span></span>

## <a name="response"></a><span data-ttu-id="8cec2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cec2-129">Response</span></span>
<span data-ttu-id="8cec2-130">Se bem-sucedido, este método retorna ```201 Created``` o código de resposta e o objeto **journalLines** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cec2-130">If successful, this method returns ```201 Created``` response code and **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cec2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cec2-131">Example</span></span>

<span data-ttu-id="8cec2-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="8cec2-132">**Request**</span></span>

<span data-ttu-id="8cec2-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cec2-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines
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
<span data-ttu-id="8cec2-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="8cec2-134">**Response**</span></span>

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


