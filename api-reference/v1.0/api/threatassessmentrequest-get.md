---
title: Get threatAssessmentRequest
description: Recupere as propriedades e as relações de um objeto threatassessmentrequest especificado.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: b21b7d69d241c5d986713b9e905822faf879147a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053801"
---
# <a name="get-threatassessmentrequest"></a><span data-ttu-id="6f54e-103">Get threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6f54e-103">Get threatAssessmentRequest</span></span>

<span data-ttu-id="6f54e-104">Recupere as propriedades e as relações de um objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="6f54e-104">Retrieve the properties and relationships of a specified [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

<span data-ttu-id="6f54e-105">Uma solicitação de avaliação de ameaças pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="6f54e-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="6f54e-106">Email</span><span class="sxs-lookup"><span data-stu-id="6f54e-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="6f54e-107">Arquivo de email</span><span class="sxs-lookup"><span data-stu-id="6f54e-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="6f54e-108">Arquivo</span><span class="sxs-lookup"><span data-stu-id="6f54e-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="6f54e-109">URL</span><span class="sxs-lookup"><span data-stu-id="6f54e-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="6f54e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f54e-110">Permissions</span></span>

<span data-ttu-id="6f54e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f54e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6f54e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f54e-113">Permission type</span></span>                        | <span data-ttu-id="6f54e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f54e-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6f54e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f54e-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f54e-116">ThreatAssessment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f54e-116">ThreatAssessment.ReadWrite.All</span></span>             |
| <span data-ttu-id="6f54e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f54e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f54e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f54e-118">Not supported.</span></span>                              |
| <span data-ttu-id="6f54e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f54e-119">Application</span></span>                            | <span data-ttu-id="6f54e-120">ThreatAssessment.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f54e-120">ThreatAssessment.Read.All</span></span>                  |

## <a name="http-request"></a><span data-ttu-id="6f54e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f54e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /informationProtection/threatAssessmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f54e-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6f54e-122">Optional query parameters</span></span>

<span data-ttu-id="6f54e-123">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6f54e-123">This method supports the following OData query parameters to help customize the response.</span></span> <span data-ttu-id="6f54e-124">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6f54e-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

|<span data-ttu-id="6f54e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="6f54e-125">Name</span></span>            |<span data-ttu-id="6f54e-126">Valor</span><span class="sxs-lookup"><span data-stu-id="6f54e-126">Value</span></span>    |<span data-ttu-id="6f54e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f54e-127">Description</span></span>                                                                                                                                                                 |
|:---------------|:--------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6f54e-128">$expand</span><span class="sxs-lookup"><span data-stu-id="6f54e-128">$expand</span></span>         |<span data-ttu-id="6f54e-129">string</span><span class="sxs-lookup"><span data-stu-id="6f54e-129">string</span></span>   |<span data-ttu-id="6f54e-130">Usando `$expand=results` na consulta para recuperar o resultado da avaliação de ameaças.</span><span class="sxs-lookup"><span data-stu-id="6f54e-130">Using `$expand=results` in the query to retrieve the threat assessment result.</span></span>                                                                                              |
|<span data-ttu-id="6f54e-131">$select</span><span class="sxs-lookup"><span data-stu-id="6f54e-131">$select</span></span>         |<span data-ttu-id="6f54e-132">string</span><span class="sxs-lookup"><span data-stu-id="6f54e-132">string</span></span>   |<span data-ttu-id="6f54e-p103">Lista separada por vírgulas de propriedades para incluir na resposta. Para um desempenho ideal, selecione apenas o subconjunto de propriedades necessário.</span><span class="sxs-lookup"><span data-stu-id="6f54e-p103">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>                                        |

## <a name="request-headers"></a><span data-ttu-id="6f54e-135">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f54e-135">Request headers</span></span>

| <span data-ttu-id="6f54e-136">Nome</span><span class="sxs-lookup"><span data-stu-id="6f54e-136">Name</span></span>      |<span data-ttu-id="6f54e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f54e-137">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6f54e-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f54e-138">Authorization</span></span> | <span data-ttu-id="6f54e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f54e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f54e-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f54e-141">Request body</span></span>

<span data-ttu-id="6f54e-142">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f54e-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f54e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f54e-143">Response</span></span>

<span data-ttu-id="6f54e-144">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f54e-144">If successful, this method returns a `200 OK` response code and the requested [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span> <span data-ttu-id="6f54e-145">As propriedades desse tipo são retornadas: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="6f54e-145">The properties of that type are returned: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span>

## <a name="examples"></a><span data-ttu-id="6f54e-146">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6f54e-146">Examples</span></span>

### <a name="example-1-get-the-properties-of-a-mail-assessment-request"></a><span data-ttu-id="6f54e-147">Exemplo 1: Obter as propriedades de uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="6f54e-147">Example 1: Get the properties of a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="6f54e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f54e-148">Request</span></span>

<span data-ttu-id="6f54e-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f54e-149">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f54e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f54e-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/49c5ef5b-1f65-444a-e6b9-08d772ea2059
```
# <a name="c"></a>[<span data-ttu-id="6f54e-151">C#</span><span class="sxs-lookup"><span data-stu-id="6f54e-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f54e-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f54e-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f54e-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f54e-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f54e-154">Java</span><span class="sxs-lookup"><span data-stu-id="6f54e-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f54e-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f54e-155">Response</span></span>

<span data-ttu-id="6f54e-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f54e-156">The following is an example of the response.</span></span>

> <span data-ttu-id="6f54e-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f54e-157">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
}
```

### <a name="example-2-get-the-properties-of-an-email-file-assessment-request"></a><span data-ttu-id="6f54e-158">Exemplo 2: Obter as propriedades de uma solicitação de avaliação de arquivo de email</span><span class="sxs-lookup"><span data-stu-id="6f54e-158">Example 2: Get the properties of an email file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="6f54e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f54e-159">Request</span></span>

<span data-ttu-id="6f54e-160">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f54e-160">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f54e-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f54e-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailfileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf
```
# <a name="c"></a>[<span data-ttu-id="6f54e-162">C#</span><span class="sxs-lookup"><span data-stu-id="6f54e-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailfileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f54e-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f54e-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailfileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f54e-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f54e-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailfileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f54e-165">Java</span><span class="sxs-lookup"><span data-stu-id="6f54e-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailfileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f54e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f54e-166">Response</span></span>

<span data-ttu-id="6f54e-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f54e-167">The following is an example of the response.</span></span>

> <span data-ttu-id="6f54e-168">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f54e-168">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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

### <a name="example-3-get-the-properties-of-a-file-assessment-request"></a><span data-ttu-id="6f54e-169">Exemplo 3: Obter as propriedades de uma solicitação de avaliação de arquivo</span><span class="sxs-lookup"><span data-stu-id="6f54e-169">Example 3: Get the properties of a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="6f54e-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f54e-170">Request</span></span>

<span data-ttu-id="6f54e-171">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f54e-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f54e-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f54e-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/18406a56-7209-4720-a250-08d772fccdaa
```
# <a name="c"></a>[<span data-ttu-id="6f54e-173">C#</span><span class="sxs-lookup"><span data-stu-id="6f54e-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fileassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f54e-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f54e-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fileassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f54e-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f54e-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fileassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f54e-176">Java</span><span class="sxs-lookup"><span data-stu-id="6f54e-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fileassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f54e-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f54e-177">Response</span></span>

<span data-ttu-id="6f54e-178">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f54e-178">The following is an example of the response.</span></span>

> <span data-ttu-id="6f54e-179">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f54e-179">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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

### <a name="example-4-get-the-properties-of-an-url-assessment-request"></a><span data-ttu-id="6f54e-180">Exemplo 4: Obter as propriedades de uma solicitação de avaliação de url</span><span class="sxs-lookup"><span data-stu-id="6f54e-180">Example 4: Get the properties of an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="6f54e-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f54e-181">Request</span></span>

<span data-ttu-id="6f54e-182">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f54e-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f54e-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f54e-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_urlassessmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/723c35be-8b5a-47ae-29c0-08d76ddb7f5b
```
# <a name="c"></a>[<span data-ttu-id="6f54e-184">C#</span><span class="sxs-lookup"><span data-stu-id="6f54e-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-urlassessmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f54e-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f54e-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-urlassessmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f54e-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f54e-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-urlassessmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f54e-187">Java</span><span class="sxs-lookup"><span data-stu-id="6f54e-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-urlassessmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f54e-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f54e-188">Response</span></span>

<span data-ttu-id="6f54e-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f54e-189">The following is an example of the response.</span></span>

> <span data-ttu-id="6f54e-190">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f54e-190">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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

### <a name="example-5-expand-threat-assessment-results-for-a-request"></a><span data-ttu-id="6f54e-191">Exemplo 5: Expandir resultados de avaliação de ameaças para uma solicitação</span><span class="sxs-lookup"><span data-stu-id="6f54e-191">Example 5: Expand threat assessment results for a request</span></span>

#### <a name="request"></a><span data-ttu-id="6f54e-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f54e-192">Request</span></span>

<span data-ttu-id="6f54e-193">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f54e-193">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6f54e-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f54e-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentrequest_expand_results"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/11922306-b25b-4605-ff0d-08d772fcf996?$expand=results
```
# <a name="c"></a>[<span data-ttu-id="6f54e-195">C#</span><span class="sxs-lookup"><span data-stu-id="6f54e-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threatassessmentrequest-expand-results-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f54e-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f54e-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threatassessmentrequest-expand-results-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f54e-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f54e-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threatassessmentrequest-expand-results-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6f54e-198">Java</span><span class="sxs-lookup"><span data-stu-id="6f54e-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-threatassessmentrequest-expand-results-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6f54e-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f54e-199">Response</span></span>

<span data-ttu-id="6f54e-200">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f54e-200">The following is an example of the response.</span></span>

> <span data-ttu-id="6f54e-201">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6f54e-201">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests(results())/$entity",
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
    "results@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests('11922306-b25b-4605-ff0d-08d772fcf996')/microsoft.graph.mailAssessmentRequest/results",
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

