---
title: Listar threatAssessmentRequests
description: Recupere uma lista de objetos threatassessmentrequest.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: f1e3a49218dc8a920e9a11517bd9d6d6bb9f197e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956467"
---
# <a name="list-threatassessmentrequests"></a><span data-ttu-id="cd3df-103">Listar threatAssessmentRequests</span><span class="sxs-lookup"><span data-stu-id="cd3df-103">List threatAssessmentRequests</span></span>

<span data-ttu-id="cd3df-104">Recupere uma lista [de objetos threatAssessmentRequest.](../resources/threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="cd3df-104">Retrieve a list of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects.</span></span>

<span data-ttu-id="cd3df-105">Uma solicitação de avaliação de ameaças pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="cd3df-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="cd3df-106">Email</span><span class="sxs-lookup"><span data-stu-id="cd3df-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="cd3df-107">Arquivo de email</span><span class="sxs-lookup"><span data-stu-id="cd3df-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="cd3df-108">Arquivo</span><span class="sxs-lookup"><span data-stu-id="cd3df-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="cd3df-109">URL</span><span class="sxs-lookup"><span data-stu-id="cd3df-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="cd3df-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd3df-110">Permissions</span></span>

<span data-ttu-id="cd3df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd3df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cd3df-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd3df-113">Permission type</span></span>                        | <span data-ttu-id="cd3df-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd3df-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cd3df-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd3df-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd3df-116">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd3df-116">ThreatAssessment.ReadWrite.All</span></span>             |
| <span data-ttu-id="cd3df-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd3df-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd3df-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd3df-118">Not supported.</span></span>                              |
| <span data-ttu-id="cd3df-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd3df-119">Application</span></span>                            | <span data-ttu-id="cd3df-120">ThreatAssessment.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd3df-120">ThreatAssessment.Read.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="cd3df-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd3df-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd3df-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cd3df-122">Optional query parameters</span></span>

<span data-ttu-id="cd3df-123">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cd3df-123">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="cd3df-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cd3df-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="cd3df-125">Nome</span><span class="sxs-lookup"><span data-stu-id="cd3df-125">Name</span></span>            |<span data-ttu-id="cd3df-126">Valor</span><span class="sxs-lookup"><span data-stu-id="cd3df-126">Value</span></span>    |<span data-ttu-id="cd3df-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd3df-127">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="cd3df-128">$filter</span><span class="sxs-lookup"><span data-stu-id="cd3df-128">$filter</span></span>         |<span data-ttu-id="cd3df-129">string</span><span class="sxs-lookup"><span data-stu-id="cd3df-129">string</span></span>   |<span data-ttu-id="cd3df-130">Limita a resposta apenas aos objetos que contêm os critérios especificados.</span><span class="sxs-lookup"><span data-stu-id="cd3df-130">Limits the response to only those objects which contain the specified criteria.</span></span>                                                                                             |
|<span data-ttu-id="cd3df-131">$orderby</span><span class="sxs-lookup"><span data-stu-id="cd3df-131">$orderby</span></span>        |<span data-ttu-id="cd3df-132">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd3df-132">string</span></span>   |<span data-ttu-id="cd3df-133">Por padrão, os objetos na resposta são decrescentes ordenados pelo **valor createdDateTime.**</span><span class="sxs-lookup"><span data-stu-id="cd3df-133">By default, the objects in the response are descending ordered by their **createdDateTime** value.</span></span>                                                                          |
|<span data-ttu-id="cd3df-134">$select</span><span class="sxs-lookup"><span data-stu-id="cd3df-134">$select</span></span>         |<span data-ttu-id="cd3df-135">string</span><span class="sxs-lookup"><span data-stu-id="cd3df-135">string</span></span>   |<span data-ttu-id="cd3df-p103">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="cd3df-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |
|<span data-ttu-id="cd3df-138">$skipToken</span><span class="sxs-lookup"><span data-stu-id="cd3df-138">$skipToken</span></span>      |<span data-ttu-id="cd3df-139">string</span><span class="sxs-lookup"><span data-stu-id="cd3df-139">string</span></span>   |<span data-ttu-id="cd3df-140">Recupera a próxima página de resultados de conjuntos de resultados que abrangem várias páginas.</span><span class="sxs-lookup"><span data-stu-id="cd3df-140">Retrieves the next page of results from result sets that span multiple pages.</span></span>                                                                                               |

## <a name="request-headers"></a><span data-ttu-id="cd3df-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd3df-141">Request headers</span></span>

| <span data-ttu-id="cd3df-142">Nome</span><span class="sxs-lookup"><span data-stu-id="cd3df-142">Name</span></span>      |<span data-ttu-id="cd3df-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd3df-143">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cd3df-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd3df-144">Authorization</span></span> | <span data-ttu-id="cd3df-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd3df-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd3df-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd3df-147">Request body</span></span>

<span data-ttu-id="cd3df-148">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd3df-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd3df-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd3df-149">Response</span></span>

<span data-ttu-id="cd3df-150">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção [de objetos threatAssessmentRequest](../resources/threatassessmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd3df-150">If successful, this method returns a `200 OK` response code and a collection of [threatAssessmentRequest](../resources/threatassessmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd3df-151">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cd3df-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cd3df-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd3df-152">Request</span></span>

<span data-ttu-id="cd3df-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd3df-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd3df-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd3df-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
```
# <a name="c"></a>[<span data-ttu-id="cd3df-155">C#</span><span class="sxs-lookup"><span data-stu-id="cd3df-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd3df-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd3df-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd3df-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd3df-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd3df-158">Java</span><span class="sxs-lookup"><span data-stu-id="cd3df-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd3df-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd3df-159">Response</span></span>

<span data-ttu-id="cd3df-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd3df-160">The following is an example of the response.</span></span>

> <span data-ttu-id="cd3df-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cd3df-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests?$skiptoken=eyJQYWdlQ29va2llIjoiPHJvdyBpZF9JZGVudGl0",
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailAssessmentRequest",
      "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
      "createdDateTime": "2019-11-27T03:30:18.6890937Z",
      "contentType": "mail",
      "expectedAssessment": "block",
      "category": "spam",
      "status": "pending",
      "requestSource": "administrator",
      "recipientEmail": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com",
      "destinationRoutingReason": "notJunk",
      "messageUri": "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
      "id": "ab2ad9b3-2213-4091-ae0c-08d76ddbcacf",
      "createdDateTime": "2019-11-20T17:05:06.4088076Z",
      "contentType": "mail",
      "expectedAssessment": "block",
      "category": "malware",
      "status": "completed",
      "requestSource": "administrator",
      "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
      "destinationRoutingReason": "notJunk",
      "contentData": "",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.fileAssessmentRequest",
      "id": "18406a56-7209-4720-a250-08d772fccdaa",
      "createdDateTime": "2019-11-27T05:44:00.4051536Z",
      "contentType": "file",
      "expectedAssessment": "block",
      "category": "malware",
      "status": "completed",
      "requestSource": "administrator",
      "fileName": "b3d5b715-4b88-4bbb-b0ae-9a9281a3f18a.csv",
      "contentData": "",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    },
    {
      "@odata.type": "#microsoft.graph.urlAssessmentRequest",
      "id": "723c35be-8b5a-47ae-29c0-08d76ddb7f5b",
      "createdDateTime": "2019-11-20T17:02:59.8160832Z",
      "contentType": "url",
      "expectedAssessment": "unblock",
      "category": "phishing",
      "status": "completed",
      "requestSource": "administrator",
      "url": "http://test.com",
      "createdBy": {
        "user": {
          "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
          "displayName": "Ronald Admin"
        }
      }
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threatAssessmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

