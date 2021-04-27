---
title: Get threatAssessmentRequest
description: Recupere as propriedades e as relações de um objeto threatassessmentrequest especificado.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 7a0eeedc76e9a155d62fdf3018badafbe6382269
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050798"
---
# <a name="get-threatassessmentrequest"></a><span data-ttu-id="3c14b-103">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3c14b-103">Get threatAssessmentRequest</span></span>

<span data-ttu-id="3c14b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c14b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c14b-105">Recupere as propriedades e as relações de um objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="3c14b-105">Retrieve the properties and relationships of a specified [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

<span data-ttu-id="3c14b-106">Uma solicitação de avaliação de ameaças pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="3c14b-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="3c14b-107">Email</span><span class="sxs-lookup"><span data-stu-id="3c14b-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="3c14b-108">Arquivo de email</span><span class="sxs-lookup"><span data-stu-id="3c14b-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="3c14b-109">Arquivo</span><span class="sxs-lookup"><span data-stu-id="3c14b-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="3c14b-110">URL</span><span class="sxs-lookup"><span data-stu-id="3c14b-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="3c14b-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c14b-111">Permissions</span></span>

<span data-ttu-id="3c14b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c14b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3c14b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c14b-114">Permission type</span></span>                        | <span data-ttu-id="3c14b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c14b-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3c14b-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c14b-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="3c14b-117">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c14b-117">ThreatAssessment.ReadWrite.All</span></span>             |
| <span data-ttu-id="3c14b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c14b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c14b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c14b-119">Not supported.</span></span>                              |
| <span data-ttu-id="3c14b-120">Application</span><span class="sxs-lookup"><span data-stu-id="3c14b-120">Application</span></span>                            | <span data-ttu-id="3c14b-121">ThreatAssessment.Read.All</span><span class="sxs-lookup"><span data-stu-id="3c14b-121">ThreatAssessment.Read.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="3c14b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c14b-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c14b-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c14b-123">Optional query parameters</span></span>

<span data-ttu-id="3c14b-124">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c14b-124">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c14b-125">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c14b-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="3c14b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="3c14b-126">Name</span></span>            |<span data-ttu-id="3c14b-127">Valor</span><span class="sxs-lookup"><span data-stu-id="3c14b-127">Value</span></span>    |<span data-ttu-id="3c14b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c14b-128">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="3c14b-129">$expand</span><span class="sxs-lookup"><span data-stu-id="3c14b-129">$expand</span></span>         |<span data-ttu-id="3c14b-130">string</span><span class="sxs-lookup"><span data-stu-id="3c14b-130">string</span></span>   |<span data-ttu-id="3c14b-131">Usando `$expand=results` na consulta para recuperar o resultado da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="3c14b-131">Using `$expand=results` in the query to retrieve the threat assessment result.</span></span>                                                                                              |
|<span data-ttu-id="3c14b-132">$select</span><span class="sxs-lookup"><span data-stu-id="3c14b-132">$select</span></span>         |<span data-ttu-id="3c14b-133">string</span><span class="sxs-lookup"><span data-stu-id="3c14b-133">string</span></span>   |<span data-ttu-id="3c14b-p103">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="3c14b-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |

## <a name="request-headers"></a><span data-ttu-id="3c14b-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c14b-136">Request headers</span></span>

| <span data-ttu-id="3c14b-137">Nome</span><span class="sxs-lookup"><span data-stu-id="3c14b-137">Name</span></span>      |<span data-ttu-id="3c14b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c14b-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3c14b-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c14b-139">Authorization</span></span> | <span data-ttu-id="3c14b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c14b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c14b-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c14b-142">Request body</span></span>

<span data-ttu-id="3c14b-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3c14b-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c14b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c14b-144">Response</span></span>

<span data-ttu-id="3c14b-145">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c14b-145">If successful, this method returns a `200 OK` response code and the requested [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span> <span data-ttu-id="3c14b-146">As propriedades desse tipo são retornadas: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="3c14b-146">The properties of that type are returned: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span>

## <a name="examples"></a><span data-ttu-id="3c14b-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3c14b-147">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-mail-assessment-request"></a><span data-ttu-id="3c14b-148">Exemplo 1: Obter as propriedades de uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="3c14b-148">Example 1: Get the properties of a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="3c14b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c14b-149">Request</span></span>

<span data-ttu-id="3c14b-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c14b-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c14b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c14b-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059
```
# <a name="c"></a>[<span data-ttu-id="3c14b-152">C#</span><span class="sxs-lookup"><span data-stu-id="3c14b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c14b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c14b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c14b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c14b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c14b-155">Java</span><span class="sxs-lookup"><span data-stu-id="3c14b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c14b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c14b-156">Response</span></span>

<span data-ttu-id="3c14b-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c14b-157">The following is an example of the response.</span></span>

> <span data-ttu-id="3c14b-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c14b-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-properties-of-an-email-file-assessment-request"></a><span data-ttu-id="3c14b-159">Exemplo 2: Obter as propriedades de uma solicitação de avaliação de arquivo de email</span><span class="sxs-lookup"><span data-stu-id="3c14b-159">Example 2: Get the properties of an email file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="3c14b-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c14b-160">Request</span></span>

<span data-ttu-id="3c14b-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c14b-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c14b-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c14b-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailfileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf
```
# <a name="c"></a>[<span data-ttu-id="3c14b-163">C#</span><span class="sxs-lookup"><span data-stu-id="3c14b-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailfileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c14b-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c14b-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailfileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c14b-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c14b-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailfileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c14b-166">Java</span><span class="sxs-lookup"><span data-stu-id="3c14b-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailfileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c14b-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c14b-167">Response</span></span>

<span data-ttu-id="3c14b-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c14b-168">The following is an example of the response.</span></span>

> <span data-ttu-id="3c14b-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c14b-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-the-properties-of-a-file-assessment-request"></a><span data-ttu-id="3c14b-170">Exemplo 3: Obter as propriedades de uma solicitação de avaliação de arquivo</span><span class="sxs-lookup"><span data-stu-id="3c14b-170">Example 3: Get the properties of a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="3c14b-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c14b-171">Request</span></span>

<span data-ttu-id="3c14b-172">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c14b-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c14b-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c14b-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa
```
# <a name="c"></a>[<span data-ttu-id="3c14b-174">C#</span><span class="sxs-lookup"><span data-stu-id="3c14b-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c14b-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c14b-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c14b-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c14b-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c14b-177">Java</span><span class="sxs-lookup"><span data-stu-id="3c14b-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c14b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c14b-178">Response</span></span>

<span data-ttu-id="3c14b-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c14b-179">The following is an example of the response.</span></span>

> <span data-ttu-id="3c14b-180">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c14b-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-get-the-properties-of-an-url-assessment-request"></a><span data-ttu-id="3c14b-181">Exemplo 4: Obter as propriedades de uma solicitação de avaliação de url</span><span class="sxs-lookup"><span data-stu-id="3c14b-181">Example 4: Get the properties of an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="3c14b-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c14b-182">Request</span></span>

<span data-ttu-id="3c14b-183">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c14b-183">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c14b-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c14b-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_urlassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b
```
# <a name="c"></a>[<span data-ttu-id="3c14b-185">C#</span><span class="sxs-lookup"><span data-stu-id="3c14b-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-urlassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c14b-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c14b-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-urlassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c14b-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c14b-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-urlassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c14b-188">Java</span><span class="sxs-lookup"><span data-stu-id="3c14b-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-urlassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c14b-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c14b-189">Response</span></span>

<span data-ttu-id="3c14b-190">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c14b-190">The following is an example of the response.</span></span>

> <span data-ttu-id="3c14b-191">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c14b-191">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-5-expand-threat-assessment-results-for-a-request"></a><span data-ttu-id="3c14b-192">Exemplo 5: Expandir resultados de avaliação de ameaças para uma solicitação</span><span class="sxs-lookup"><span data-stu-id="3c14b-192">Example 5: Expand threat assessment results for a request</span></span>

#### <a name="request"></a><span data-ttu-id="3c14b-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c14b-193">Request</span></span>

<span data-ttu-id="3c14b-194">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3c14b-194">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3c14b-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c14b-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest_expand_results"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996?$expand=results
```
# <a name="c"></a>[<span data-ttu-id="3c14b-196">C#</span><span class="sxs-lookup"><span data-stu-id="3c14b-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequest-expand-results-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c14b-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c14b-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequest-expand-results-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c14b-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c14b-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequest-expand-results-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c14b-199">Java</span><span class="sxs-lookup"><span data-stu-id="3c14b-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequest-expand-results-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3c14b-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c14b-200">Response</span></span>

<span data-ttu-id="3c14b-201">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3c14b-201">The following is an example of the response.</span></span>

> <span data-ttu-id="3c14b-202">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c14b-202">**Note:** The response object shown here might be shortened for readability.</span></span>

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


