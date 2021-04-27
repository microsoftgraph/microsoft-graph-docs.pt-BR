---
title: 'message: copy'
description: Copie uma mensagem para uma pasta.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: dff98e9e10cf8e909b1785c94c86797467c795d9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053654"
---
# <a name="message-copy"></a><span data-ttu-id="5c5e6-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="5c5e6-103">message: copy</span></span>

<span data-ttu-id="5c5e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c5e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c5e6-105">Copie uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-105">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5e6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c5e6-106">Permissions</span></span>

<span data-ttu-id="5c5e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c5e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c5e6-109">Permission type</span></span> | <span data-ttu-id="5c5e6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c5e6-110">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="5c5e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c5e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5c5e6-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c5e6-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5c5e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c5e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c5e6-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c5e6-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="5c5e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c5e6-115">Application</span></span> | <span data-ttu-id="5c5e6-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c5e6-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c5e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c5e6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="5c5e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5e6-118">Request headers</span></span>

| <span data-ttu-id="5c5e6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5c5e6-119">Header</span></span> | <span data-ttu-id="5c5e6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="5c5e6-120">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="5c5e6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c5e6-121">Authorization</span></span> | <span data-ttu-id="5c5e6-122">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-122">`Bearer {token}`.</span></span> <span data-ttu-id="5c5e6-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-123">Required.</span></span> |
| <span data-ttu-id="5c5e6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5c5e6-124">Content-Type</span></span> | <span data-ttu-id="5c5e6-125">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-125">`application/json`.</span></span> <span data-ttu-id="5c5e6-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c5e6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5e6-127">Request body</span></span>

<span data-ttu-id="5c5e6-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5c5e6-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5c5e6-129">Parameter</span></span> | <span data-ttu-id="5c5e6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c5e6-130">Type</span></span> | <span data-ttu-id="5c5e6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c5e6-131">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="5c5e6-132">destinationId</span><span class="sxs-lookup"><span data-stu-id="5c5e6-132">destinationId</span></span>|<span data-ttu-id="5c5e6-133">String</span><span class="sxs-lookup"><span data-stu-id="5c5e6-133">String</span></span>|<span data-ttu-id="5c5e6-134">A ID da pasta de destino ou um nome de pasta bem conhecido.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-134">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="5c5e6-135">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="5c5e6-135">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="5c5e6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c5e6-136">Response</span></span>

<span data-ttu-id="5c5e6-137">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o recurso [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-137">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c5e6-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c5e6-138">Example</span></span>

<span data-ttu-id="5c5e6-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-139">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="5c5e6-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5e6-140">Request</span></span>

<span data-ttu-id="5c5e6-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c5e6-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c5e6-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="c"></a>[<span data-ttu-id="5c5e6-143">C#</span><span class="sxs-lookup"><span data-stu-id="5c5e6-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c5e6-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c5e6-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c5e6-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c5e6-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c5e6-146">Java</span><span class="sxs-lookup"><span data-stu-id="5c5e6-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5c5e6-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c5e6-147">Response</span></span>

<span data-ttu-id="5c5e6-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-148">Here is an example of the response.</span></span>

> <span data-ttu-id="5c5e6-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c5e6-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "2016-10-19T10:37:00Z",
  "sentDateTime": "2016-10-19T10:37:00Z",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


