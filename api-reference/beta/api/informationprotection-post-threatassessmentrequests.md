---
title: Criar threatAssessmentRequest
description: Criar uma nova solicitação de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3c62ef964acc7d67fb31b0df7dfb840c73fb5b9f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871724"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="60818-103">Criar threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="60818-103">Create threatAssessmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60818-104">Criar uma nova solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="60818-104">Create a new threat assessment request.</span></span>

<span data-ttu-id="60818-105">Uma solicitação de avaliação de ameaça pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="60818-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="60818-106">Email</span><span class="sxs-lookup"><span data-stu-id="60818-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="60818-107">Arquivo de email</span><span class="sxs-lookup"><span data-stu-id="60818-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="60818-108">Arquivo</span><span class="sxs-lookup"><span data-stu-id="60818-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="60818-109">URL</span><span class="sxs-lookup"><span data-stu-id="60818-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="60818-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="60818-110">Permissions</span></span>

<span data-ttu-id="60818-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="60818-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60818-113">Permission type</span></span>                        | <span data-ttu-id="60818-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60818-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="60818-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60818-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="60818-116">ThreatAssessment. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="60818-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="60818-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60818-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60818-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60818-118">Not supported.</span></span>                              |
| <span data-ttu-id="60818-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60818-119">Application</span></span>                            | <span data-ttu-id="60818-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60818-120">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="60818-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60818-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="60818-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60818-122">Request headers</span></span>

| <span data-ttu-id="60818-123">Nome</span><span class="sxs-lookup"><span data-stu-id="60818-123">Name</span></span>          | <span data-ttu-id="60818-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="60818-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="60818-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="60818-125">Authorization</span></span> | <span data-ttu-id="60818-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60818-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60818-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60818-128">Request body</span></span>

<span data-ttu-id="60818-129">No corpo da solicitação, forneça uma representação JSON do objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="60818-129">In the request body, supply a JSON representation of [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="60818-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="60818-130">Response</span></span>

<span data-ttu-id="60818-131">Se tiver êxito, este método retornará `201, Created` um código de resposta e um novo objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60818-131">If successful, this method returns a `201, Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60818-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="60818-132">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="60818-133">Exemplo 1: criar uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="60818-133">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="60818-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60818-134">Request</span></span>

<span data-ttu-id="60818-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60818-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60818-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="60818-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_mailassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "spam",
  "messageUri": "https://graph.microsoft.com/beta/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60818-137">C#</span><span class="sxs-lookup"><span data-stu-id="60818-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60818-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60818-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60818-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60818-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60818-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="60818-140">Response</span></span>

<span data-ttu-id="60818-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60818-141">The following is an example of the response.</span></span>

> <span data-ttu-id="60818-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60818-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="60818-144">Exemplo 2: criar uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="60818-144">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="60818-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60818-145">Request</span></span>

<span data-ttu-id="60818-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60818-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60818-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="60818-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailfileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "malware",
  "contentData": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60818-148">C#</span><span class="sxs-lookup"><span data-stu-id="60818-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailfileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60818-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60818-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailfileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60818-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60818-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailfileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60818-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="60818-151">Response</span></span>

<span data-ttu-id="60818-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60818-152">The following is an example of the response.</span></span>

> <span data-ttu-id="60818-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60818-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="60818-155">Exemplo 3: criar uma solicitação de avaliação de arquivo</span><span class="sxs-lookup"><span data-stu-id="60818-155">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="60818-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60818-156">Request</span></span>

<span data-ttu-id="60818-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60818-157">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60818-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="60818-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_fileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.fileAssessmentRequest",
  "expectedAssessment": "block",
  "category": "malware",
  "fileName": "test.txt",
  "contentData": "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60818-159">C#</span><span class="sxs-lookup"><span data-stu-id="60818-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-fileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60818-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60818-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-fileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60818-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60818-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-fileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60818-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="60818-162">Response</span></span>

<span data-ttu-id="60818-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60818-163">The following is an example of the response.</span></span>

> <span data-ttu-id="60818-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60818-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="60818-166">Exemplo 4: criar uma solicitação de avaliação de URL</span><span class="sxs-lookup"><span data-stu-id="60818-166">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="60818-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60818-167">Request</span></span>

<span data-ttu-id="60818-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60818-168">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="60818-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="60818-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_urlassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "url": "http://test.com",
  "expectedAssessment": "block",
  "category": "phishing"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60818-170">C#</span><span class="sxs-lookup"><span data-stu-id="60818-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-urlassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60818-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60818-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-urlassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60818-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60818-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-urlassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60818-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="60818-173">Response</span></span>

<span data-ttu-id="60818-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60818-174">The following is an example of the response.</span></span>

> <span data-ttu-id="60818-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60818-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#informationProtection/threatAssessmentRequests/$entity",
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "id": "8d87d2b2-ca4d-422c-f8df-08d774a5c9ac",
  "createdDateTime": "2019-11-29T08:26:09.8196703Z",
  "contentType": "url",
  "expectedAssessment": "block",
  "category": "phishing",
  "status": "pending",
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create threatAssessmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
