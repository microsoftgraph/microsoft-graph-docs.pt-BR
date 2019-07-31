---
title: Obter journalLines
description: Obtém um objeto de linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 27d7188d8f0443d11ab6799172a04b855cce5261
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35956118"
---
# <a name="get-journallines"></a><span data-ttu-id="8e483-103">Obter journalLines</span><span class="sxs-lookup"><span data-stu-id="8e483-103">Get journalLines</span></span>
<span data-ttu-id="8e483-104">Recupere as propriedades e os relacionamentos de um objeto de linha de diário para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="8e483-104">Retrieve the properties and relationships of a journal line object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e483-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e483-105">Permissions</span></span>
<span data-ttu-id="8e483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e483-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e483-108">Permission type</span></span> |<span data-ttu-id="8e483-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e483-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="8e483-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e483-110">Delegated (work or school account)</span></span>|<span data-ttu-id="8e483-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e483-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="8e483-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8e483-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8e483-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e483-113">Not supported.</span></span>|
|<span data-ttu-id="8e483-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e483-114">Application</span></span>|<span data-ttu-id="8e483-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e483-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e483-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e483-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e483-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e483-117">Optional query parameters</span></span>
<span data-ttu-id="8e483-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e483-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e483-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e483-119">Request headers</span></span>
|<span data-ttu-id="8e483-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e483-120">Header</span></span>       |<span data-ttu-id="8e483-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8e483-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="8e483-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e483-122">Authorization</span></span>|<span data-ttu-id="8e483-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e483-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8e483-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e483-125">Request body</span></span>
<span data-ttu-id="8e483-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e483-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e483-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e483-127">Response</span></span>
<span data-ttu-id="8e483-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **journalLines** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e483-128">If successful, this method returns a `200 OK` response code and a **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e483-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e483-129">Example</span></span>

<span data-ttu-id="8e483-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="8e483-130">**Request**</span></span>

<span data-ttu-id="8e483-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e483-131">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

<span data-ttu-id="8e483-132">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="8e483-132">**Response**</span></span>

<span data-ttu-id="8e483-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e483-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="8e483-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8e483-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8e483-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e483-135">All the properties will be returned from an actual call.</span></span>

```json
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

