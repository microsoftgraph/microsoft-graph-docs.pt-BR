---
title: Get threatAssessmentRequest
description: Recupere as propriedades e as relações de um objeto threatassessmentrequest especificado.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0c4f179243f8fa14ee59e22a07fbd643f9ccb850
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962795"
---
# <a name="get-threatassessmentrequest"></a><span data-ttu-id="51acc-103">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="51acc-103">Get threatAssessmentRequest</span></span>

<span data-ttu-id="51acc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51acc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51acc-105">Recupere as propriedades e as relações de um objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="51acc-105">Retrieve the properties and relationships of a specified [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

<span data-ttu-id="51acc-106">Uma solicitação de avaliação de ameaças pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="51acc-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="51acc-107">Email</span><span class="sxs-lookup"><span data-stu-id="51acc-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="51acc-108">Arquivo de email</span><span class="sxs-lookup"><span data-stu-id="51acc-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="51acc-109">Arquivo</span><span class="sxs-lookup"><span data-stu-id="51acc-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="51acc-110">URL</span><span class="sxs-lookup"><span data-stu-id="51acc-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="51acc-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="51acc-111">Permissions</span></span>

<span data-ttu-id="51acc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51acc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51acc-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51acc-114">Permission type</span></span>                        | <span data-ttu-id="51acc-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51acc-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51acc-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51acc-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="51acc-117">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51acc-117">ThreatAssessment.ReadWrite.All</span></span>             |
| <span data-ttu-id="51acc-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51acc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51acc-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51acc-119">Not supported.</span></span>                              |
| <span data-ttu-id="51acc-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51acc-120">Application</span></span>                            | <span data-ttu-id="51acc-121">ThreatAssessment.Read.All</span><span class="sxs-lookup"><span data-stu-id="51acc-121">ThreatAssessment.Read.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="51acc-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51acc-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51acc-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="51acc-123">Optional query parameters</span></span>

<span data-ttu-id="51acc-124">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="51acc-124">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="51acc-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="51acc-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="51acc-126">Name</span><span class="sxs-lookup"><span data-stu-id="51acc-126">Name</span></span>            |<span data-ttu-id="51acc-127">Valor</span><span class="sxs-lookup"><span data-stu-id="51acc-127">Value</span></span>    |<span data-ttu-id="51acc-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="51acc-128">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="51acc-129">$expand</span><span class="sxs-lookup"><span data-stu-id="51acc-129">$expand</span></span>         |<span data-ttu-id="51acc-130">string</span><span class="sxs-lookup"><span data-stu-id="51acc-130">string</span></span>   |<span data-ttu-id="51acc-131">Usando `$expand=results` na consulta para recuperar o resultado da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="51acc-131">Using `$expand=results` in the query to retrieve the threat assessment result.</span></span>                                                                                              |
|<span data-ttu-id="51acc-132">$select</span><span class="sxs-lookup"><span data-stu-id="51acc-132">$select</span></span>         |<span data-ttu-id="51acc-133">string</span><span class="sxs-lookup"><span data-stu-id="51acc-133">string</span></span>   |<span data-ttu-id="51acc-p103">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="51acc-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |

## <a name="request-headers"></a><span data-ttu-id="51acc-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51acc-136">Request headers</span></span>

| <span data-ttu-id="51acc-137">Nome</span><span class="sxs-lookup"><span data-stu-id="51acc-137">Name</span></span>      |<span data-ttu-id="51acc-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="51acc-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51acc-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="51acc-139">Authorization</span></span> | <span data-ttu-id="51acc-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51acc-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51acc-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51acc-142">Request body</span></span>

<span data-ttu-id="51acc-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51acc-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51acc-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="51acc-144">Response</span></span>

<span data-ttu-id="51acc-145">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51acc-145">If successful, this method returns a `200 OK` response code and the requested [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span> <span data-ttu-id="51acc-146">As propriedades desse tipo são retornadas: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="51acc-146">The properties of that type are returned: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span>

## <a name="examples"></a><span data-ttu-id="51acc-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="51acc-147">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-mail-assessment-request"></a><span data-ttu-id="51acc-148">Exemplo 1: Obter as propriedades de uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="51acc-148">Example 1: Get the properties of a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="51acc-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51acc-149">Request</span></span>

<span data-ttu-id="51acc-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51acc-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51acc-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="51acc-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059
```
# <a name="c"></a>[<span data-ttu-id="51acc-152">C#</span><span class="sxs-lookup"><span data-stu-id="51acc-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51acc-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51acc-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51acc-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51acc-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51acc-155">Java</span><span class="sxs-lookup"><span data-stu-id="51acc-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51acc-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="51acc-156">Response</span></span>

<span data-ttu-id="51acc-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51acc-157">The following is an example of the response.</span></span>

> <span data-ttu-id="51acc-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51acc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
  "messageUri": "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt=",
  "createdBy": {
    "user": {
      "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin"
    }
  }
}
```

### <a name="example-2-get-the-properties-of-an-email-file-assessment-request"></a><span data-ttu-id="51acc-160">Exemplo 2: Obter as propriedades de uma solicitação de avaliação de arquivo de email</span><span class="sxs-lookup"><span data-stu-id="51acc-160">Example 2: Get the properties of an email file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="51acc-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51acc-161">Request</span></span>

<span data-ttu-id="51acc-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51acc-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51acc-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="51acc-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailfileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf
```
# <a name="c"></a>[<span data-ttu-id="51acc-164">C#</span><span class="sxs-lookup"><span data-stu-id="51acc-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailfileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51acc-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51acc-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailfileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51acc-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51acc-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailfileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51acc-167">Java</span><span class="sxs-lookup"><span data-stu-id="51acc-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailfileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51acc-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="51acc-168">Response</span></span>

<span data-ttu-id="51acc-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51acc-169">The following is an example of the response.</span></span>

> <span data-ttu-id="51acc-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51acc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
}
```

### <a name="example-3-get-the-properties-of-a-file-assessment-request"></a><span data-ttu-id="51acc-172">Exemplo 3: Obter as propriedades de uma solicitação de avaliação de arquivo</span><span class="sxs-lookup"><span data-stu-id="51acc-172">Example 3: Get the properties of a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="51acc-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51acc-173">Request</span></span>

<span data-ttu-id="51acc-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51acc-174">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51acc-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="51acc-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa
```
# <a name="c"></a>[<span data-ttu-id="51acc-176">C#</span><span class="sxs-lookup"><span data-stu-id="51acc-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51acc-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51acc-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51acc-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51acc-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51acc-179">Java</span><span class="sxs-lookup"><span data-stu-id="51acc-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51acc-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="51acc-180">Response</span></span>

<span data-ttu-id="51acc-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51acc-181">The following is an example of the response.</span></span>

> <span data-ttu-id="51acc-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51acc-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
}
```

### <a name="example-4-get-the-properties-of-an-url-assessment-request"></a><span data-ttu-id="51acc-184">Exemplo 4: Obter as propriedades de uma solicitação de avaliação de url</span><span class="sxs-lookup"><span data-stu-id="51acc-184">Example 4: Get the properties of an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="51acc-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51acc-185">Request</span></span>

<span data-ttu-id="51acc-186">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51acc-186">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51acc-187">HTTP</span><span class="sxs-lookup"><span data-stu-id="51acc-187">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_urlassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b
```
# <a name="c"></a>[<span data-ttu-id="51acc-188">C#</span><span class="sxs-lookup"><span data-stu-id="51acc-188">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-urlassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51acc-189">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51acc-189">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-urlassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51acc-190">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51acc-190">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-urlassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51acc-191">Java</span><span class="sxs-lookup"><span data-stu-id="51acc-191">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-urlassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51acc-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="51acc-192">Response</span></span>

<span data-ttu-id="51acc-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51acc-193">The following is an example of the response.</span></span>

> <span data-ttu-id="51acc-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51acc-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
```

### <a name="example-5-expand-threat-assessment-results-for-a-request"></a><span data-ttu-id="51acc-196">Exemplo 5: Expandir resultados de avaliação de ameaças para uma solicitação</span><span class="sxs-lookup"><span data-stu-id="51acc-196">Example 5: Expand threat assessment results for a request</span></span>

#### <a name="request"></a><span data-ttu-id="51acc-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51acc-197">Request</span></span>

<span data-ttu-id="51acc-198">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51acc-198">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51acc-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="51acc-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest_expand_results"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996?$expand=results
```
# <a name="c"></a>[<span data-ttu-id="51acc-200">C#</span><span class="sxs-lookup"><span data-stu-id="51acc-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequest-expand-results-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51acc-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51acc-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequest-expand-results-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51acc-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51acc-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequest-expand-results-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51acc-203">Java</span><span class="sxs-lookup"><span data-stu-id="51acc-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequest-expand-results-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51acc-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="51acc-204">Response</span></span>

<span data-ttu-id="51acc-205">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51acc-205">The following is an example of the response.</span></span>

> <span data-ttu-id="51acc-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51acc-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests(results())/$entity",
    "@odata.type": "#microsoft.graph.mailAssessmentRequest",
    "id": "11922306-b25b-4605-ff0d-08d772fcf996",
    "createdDateTime": "2019-11-27T05:45:14.0962061Z",
    "contentType": "mail",
    "expectedAssessment": "block",
    "category": "phishing",
    "status": "completed",
    "requestSource": "administrator",
    "recipientEmail": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com",
    "destinationRoutingReason": "notJunk",
    "messageUri": "",
    "createdBy": {
      "user": {
        "id": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
        "displayName": "Ronald Admin"
      }
    },
    "results@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests('11922306-b25b-4605-ff0d-08d772fcf996')/microsoft.graph.mailAssessmentRequest/results",
    "results": [
        {
            "id": "63798129-a62c-4f9e-2c6d-08d772fcfb0e",
            "createdDateTime": "2019-11-27T05:45:16.55Z",
            "resultType": "checkPolicy",
            "message": "No policy was hit."
        },
        {
            "id": "d38c2448-79eb-467e-2495-08d772fdb7d1",
            "createdDateTime": "2019-11-27T05:50:33.243Z",
            "resultType": "rescan",
            "message": "Not Spam"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get threatAssessmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


