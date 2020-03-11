---
title: Create threatAssessmentRequest
description: Criar uma nova solicitação de avaliação de ameaça.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 44a8f786f4b492ae094c9b8ef12b9eff125d7218
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591527"
---
# <a name="create-threatassessmentrequest"></a><span data-ttu-id="68c7c-103">Create threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="68c7c-103">Create threatAssessmentRequest</span></span>

<span data-ttu-id="68c7c-104">Criar uma nova solicitação de avaliação de ameaça.</span><span class="sxs-lookup"><span data-stu-id="68c7c-104">Create a new threat assessment request.</span></span>

<span data-ttu-id="68c7c-105">Uma solicitação de avaliação de ameaça pode ser um dos seguintes tipos:</span><span class="sxs-lookup"><span data-stu-id="68c7c-105">A threat assessment request can be one of the following types:</span></span>

* [<span data-ttu-id="68c7c-106">Email</span><span class="sxs-lookup"><span data-stu-id="68c7c-106">Mail</span></span>](../resources/mailAssessmentRequest.md)
* [<span data-ttu-id="68c7c-107">Arquivo de email</span><span class="sxs-lookup"><span data-stu-id="68c7c-107">Email file</span></span>](../resources/emailFileAssessmentRequest.md)
* [<span data-ttu-id="68c7c-108">Arquivo</span><span class="sxs-lookup"><span data-stu-id="68c7c-108">File</span></span>](../resources/fileAssessmentRequest.md)
* [<span data-ttu-id="68c7c-109">URL</span><span class="sxs-lookup"><span data-stu-id="68c7c-109">URL</span></span>](../resources/urlAssessmentRequest.md)

## <a name="permissions"></a><span data-ttu-id="68c7c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="68c7c-110">Permissions</span></span>

<span data-ttu-id="68c7c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68c7c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68c7c-113">Permission type</span></span>                        | <span data-ttu-id="68c7c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68c7c-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68c7c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68c7c-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="68c7c-116">ThreatAssessment. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="68c7c-116">ThreatAssessment.ReadWrite.All.</span></span>             |
| <span data-ttu-id="68c7c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68c7c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68c7c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68c7c-118">Not supported.</span></span>                              |
| <span data-ttu-id="68c7c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68c7c-119">Application</span></span>                            | <span data-ttu-id="68c7c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68c7c-120">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="68c7c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68c7c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/threatAssessmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="68c7c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68c7c-122">Request headers</span></span>

| <span data-ttu-id="68c7c-123">Nome</span><span class="sxs-lookup"><span data-stu-id="68c7c-123">Name</span></span>          | <span data-ttu-id="68c7c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="68c7c-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="68c7c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="68c7c-125">Authorization</span></span> | <span data-ttu-id="68c7c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68c7c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68c7c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68c7c-128">Request body</span></span>

<span data-ttu-id="68c7c-129">No corpo da solicitação, forneça uma representação JSON de um objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="68c7c-129">In the request body, supply a JSON representation of a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="68c7c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c7c-130">Response</span></span>

<span data-ttu-id="68c7c-131">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [threatAssessmentRequest](../resources/threatassessmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68c7c-131">If successful, this method returns a `201 Created` response code and a new [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="68c7c-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="68c7c-132">Examples</span></span>

### <a name="example-1-create-a-mail-assessment-request"></a><span data-ttu-id="68c7c-133">Exemplo 1: criar uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="68c7c-133">Example 1: Create a mail assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="68c7c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68c7c-134">Request</span></span>

<span data-ttu-id="68c7c-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68c7c-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_mailassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "spam",
  "messageUri": "https://graph.microsoft.com/v1.0/users/c52ce8db-3e4b-4181-93c4-7d6b6bffaf60/messages/AAMkADU3MWUxOTU0LWNlOTEt="
}
```

#### <a name="response"></a><span data-ttu-id="68c7c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c7c-136">Response</span></span>

<span data-ttu-id="68c7c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68c7c-137">The following is an example of the response.</span></span>

> <span data-ttu-id="68c7c-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68c7c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-2-create-an-email-assessment-request"></a><span data-ttu-id="68c7c-140">Exemplo 2: criar uma solicitação de avaliação de email</span><span class="sxs-lookup"><span data-stu-id="68c7c-140">Example 2: Create an email assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="68c7c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68c7c-141">Request</span></span>

<span data-ttu-id="68c7c-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68c7c-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_emailfileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
  "recipientEmail": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "expectedAssessment": "block",
  "category": "malware",
  "contentData": "UmVjZWl2ZWQ6IGZyb20gTVcyUFIwME1CMDMxNC5uYW1wcmQwMC....."
}
```

#### <a name="response"></a><span data-ttu-id="68c7c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c7c-143">Response</span></span>

<span data-ttu-id="68c7c-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68c7c-144">The following is an example of the response.</span></span>

> <span data-ttu-id="68c7c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68c7c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-3-create-a-file-assessment-request"></a><span data-ttu-id="68c7c-147">Exemplo 3: criar uma solicitação de avaliação de arquivo</span><span class="sxs-lookup"><span data-stu-id="68c7c-147">Example 3: Create a file assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="68c7c-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68c7c-148">Request</span></span>

<span data-ttu-id="68c7c-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68c7c-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_fileassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.fileAssessmentRequest",
  "expectedAssessment": "block",
  "category": "malware",
  "fileName": "test.txt",
  "contentData": "VGhpcyBpcyBhIHRlc3QgZmlsZQ=="
}
```

#### <a name="response"></a><span data-ttu-id="68c7c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c7c-150">Response</span></span>

<span data-ttu-id="68c7c-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68c7c-151">The following is an example of the response.</span></span>

> <span data-ttu-id="68c7c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68c7c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
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

### <a name="example-4-create-an-url-assessment-request"></a><span data-ttu-id="68c7c-154">Exemplo 4: criar uma solicitação de avaliação de URL</span><span class="sxs-lookup"><span data-stu-id="68c7c-154">Example 4: Create an url assessment request</span></span>

#### <a name="request"></a><span data-ttu-id="68c7c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68c7c-155">Request</span></span>

<span data-ttu-id="68c7c-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68c7c-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_urlassessmentrequest_from_informationprotection"
}-->

```http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.urlAssessmentRequest",
  "url": "http://test.com",
  "expectedAssessment": "block",
  "category": "phishing"
}
```

#### <a name="response"></a><span data-ttu-id="68c7c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="68c7c-157">Response</span></span>

<span data-ttu-id="68c7c-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68c7c-158">The following is an example of the response.</span></span>

> <span data-ttu-id="68c7c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68c7c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.urlAssessmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#informationProtection/threatAssessmentRequests/$entity",
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
