---
title: Create threatAssessmentRequest
description: Criar uma nova solicitação de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0818b495c209fcd264d1ddcc2a8c9f146f2983c7
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "42446391"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="7fe94-103">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="7fe94-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="7fe94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fe94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fe94-105">Criar uma nova solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="7fe94-105">Create a new threat assessment request.</span></span>

<span data-ttu-id="7fe94-106">Uma solicitação de avaliação de ameaça pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="7fe94-106">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="7fe94-107">Email</span><span class="sxs-lookup"><span data-stu-id="7fe94-107">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="7fe94-108">Arquivo de email</span><span class="sxs-lookup"><span data-stu-id="7fe94-108">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="7fe94-109">Arquivo</span><span class="sxs-lookup"><span data-stu-id="7fe94-109">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="7fe94-110">URL</span><span class="sxs-lookup"><span data-stu-id="7fe94-110">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="7fe94-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fe94-111">Permissions</span></span>

<span data-ttu-id="7fe94-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fe94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7fe94-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fe94-114">Permission type</span></span>                        | <span data-ttu-id="7fe94-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fe94-115">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7fe94-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fe94-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fe94-117">ThreatAssessment. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="7fe94-117">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="7fe94-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fe94-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fe94-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe94-119">Not supported.</span></span>                              |
| <span data-ttu-id="7fe94-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fe94-120">Application</span></span>                            | <span data-ttu-id="7fe94-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7fe94-121">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="7fe94-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe94-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="7fe94-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe94-123">Request headers</span></span>

| <span data-ttu-id="7fe94-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7fe94-124">Name</span></span>          | <span data-ttu-id="7fe94-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7fe94-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7fe94-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fe94-126">Authorization</span></span> | <span data-ttu-id="7fe94-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fe94-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7fe94-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe94-129">Request body</span></span>

<span data-ttu-id="7fe94-130">No corpo da solicitação, forneça uma representação JSON do objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="7fe94-130">In the request body, supply a JSON representation of [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7fe94-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe94-131">Response</span></span>

<span data-ttu-id="7fe94-132">Se tiver êxito, este método retornará `201, Created` um código de resposta e um novo objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe94-132">If successful, this method returns a `201, Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7fe94-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7fe94-133">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="7fe94-134">Exemplo 1: criar uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="7fe94-134">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="7fe94-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe94-135">Request</span></span>

<span data-ttu-id="7fe94-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe94-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fe94-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe94-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7fe94-138">C#</span><span class="sxs-lookup"><span data-stu-id="7fe94-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-mailassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fe94-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fe94-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-mailassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fe94-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fe94-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-mailassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7fe94-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe94-141">Response</span></span>

<span data-ttu-id="7fe94-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe94-142">The following is an example of the response.</span></span>

> <span data-ttu-id="7fe94-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe94-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="7fe94-145">Exemplo 2: criar uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="7fe94-145">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="7fe94-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe94-146">Request</span></span>

<span data-ttu-id="7fe94-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe94-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fe94-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe94-148">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7fe94-149">C#</span><span class="sxs-lookup"><span data-stu-id="7fe94-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailfileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fe94-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fe94-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailfileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fe94-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fe94-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailfileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7fe94-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe94-152">Response</span></span>

<span data-ttu-id="7fe94-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe94-153">The following is an example of the response.</span></span>

> <span data-ttu-id="7fe94-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe94-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="7fe94-156">Exemplo 3: criar uma solicitação de avaliação de arquivo</span><span class="sxs-lookup"><span data-stu-id="7fe94-156">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="7fe94-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe94-157">Request</span></span>

<span data-ttu-id="7fe94-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe94-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fe94-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe94-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7fe94-160">C#</span><span class="sxs-lookup"><span data-stu-id="7fe94-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-fileassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fe94-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fe94-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-fileassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fe94-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fe94-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-fileassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7fe94-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe94-163">Response</span></span>

<span data-ttu-id="7fe94-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe94-164">The following is an example of the response.</span></span>

> <span data-ttu-id="7fe94-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe94-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="7fe94-167">Exemplo 4: criar uma solicitação de avaliação de URL</span><span class="sxs-lookup"><span data-stu-id="7fe94-167">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="7fe94-168">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe94-168">Request</span></span>

<span data-ttu-id="7fe94-169">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7fe94-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7fe94-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe94-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7fe94-171">C#</span><span class="sxs-lookup"><span data-stu-id="7fe94-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-urlassessmentrequest-from-informationprotection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7fe94-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7fe94-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-urlassessmentrequest-from-informationprotection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7fe94-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7fe94-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-urlassessmentrequest-from-informationprotection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7fe94-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe94-174">Response</span></span>

<span data-ttu-id="7fe94-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7fe94-175">The following is an example of the response.</span></span>

> <span data-ttu-id="7fe94-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7fe94-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
