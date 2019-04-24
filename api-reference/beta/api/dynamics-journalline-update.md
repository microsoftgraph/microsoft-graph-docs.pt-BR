---
title: Atualizar journalLines
description: Atualiza uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1f404a4a344f6fddc9759da9808b7c5bec1bc7ef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458520"
---
# <a name="update-journallines"></a><span data-ttu-id="6feb5-103">Atualizar journalLines</span><span class="sxs-lookup"><span data-stu-id="6feb5-103">Update journalLines</span></span>
<span data-ttu-id="6feb5-104">Atualizar as propriedades de um objeto de linhas de diário para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="6feb5-104">Update the properties of a journal lines object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6feb5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6feb5-105">Permissions</span></span>
<span data-ttu-id="6feb5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6feb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6feb5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6feb5-108">Permission type</span></span> |<span data-ttu-id="6feb5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6feb5-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6feb5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6feb5-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6feb5-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6feb5-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6feb5-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="6feb5-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6feb5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6feb5-113">Not supported.</span></span>|
|<span data-ttu-id="6feb5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6feb5-114">Application</span></span>|<span data-ttu-id="6feb5-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6feb5-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6feb5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6feb5-116">HTTP request</span></span>

```
PATCH /financials/companies('{id}')/journals('{id}')/journalLines('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6feb5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6feb5-117">Optional query parameters</span></span>
<span data-ttu-id="6feb5-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6feb5-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6feb5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6feb5-119">Request headers</span></span>
| <span data-ttu-id="6feb5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6feb5-120">Header</span></span>       | <span data-ttu-id="6feb5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6feb5-121">Value</span></span>                    |
|--------------|--------------------------|
|<span data-ttu-id="6feb5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6feb5-122">Authorization</span></span> |<span data-ttu-id="6feb5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6feb5-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="6feb5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6feb5-125">Content-Type</span></span>  |<span data-ttu-id="6feb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6feb5-126">application/json</span></span>          |
|<span data-ttu-id="6feb5-127">If-Match</span><span class="sxs-lookup"><span data-stu-id="6feb5-127">If-Match</span></span>      |<span data-ttu-id="6feb5-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6feb5-128">Required.</span></span> <span data-ttu-id="6feb5-129">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **journalLines**, o **journalLines** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="6feb5-129">When this request header is included and the eTag provided does not match the current tag on the **journalLines**, the **journalLines** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6feb5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6feb5-130">Request body</span></span>
<span data-ttu-id="6feb5-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6feb5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="6feb5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6feb5-134">Response</span></span>
<span data-ttu-id="6feb5-135">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **journalLines** atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6feb5-135">If successful, this method returns a `200 OK` response code and an updated **journalLines** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6feb5-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6feb5-136">Example</span></span>

<span data-ttu-id="6feb5-137">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="6feb5-137">**Request**</span></span>

<span data-ttu-id="6feb5-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6feb5-138">Here is an example of the request.</span></span>
```json
PATCH https://graph.microsoft.com/beta/financials/companies('{id}')/journals('{id}')/journalLines('{id}')
Content-type: application/json

{
  "amount": 2000
}
```

<span data-ttu-id="6feb5-139">**Response**</span><span class="sxs-lookup"><span data-stu-id="6feb5-139">**Response**</span></span>

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "journalDisplayName": "DEFAULT",
  "lineNumber": 10000,
  "accountId": "",
  "accountNumber": "",
  "postingDate": "2015-12-31",
  "documentNumber": "D00001",
  "externalDocumentNumber": "",
  "amount": 2000,
  "description": "",
  "comment": "",
  "lastModifiedDateTime": "2017-03-17T19:02:22.043Z"
}
```


