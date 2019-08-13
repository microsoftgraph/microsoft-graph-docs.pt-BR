---
title: 'message: copy'
description: Copie uma mensagem para uma pasta.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b7754de960036c38f0c0f5689b8a4a8cf2ed6f6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374880"
---
# <a name="message-copy"></a><span data-ttu-id="7066a-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="7066a-103">message: copy</span></span>

<span data-ttu-id="7066a-104">Copie uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="7066a-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="7066a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7066a-105">Permissions</span></span>

<span data-ttu-id="7066a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7066a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7066a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7066a-108">Permission type</span></span> | <span data-ttu-id="7066a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7066a-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="7066a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7066a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7066a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7066a-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7066a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7066a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7066a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7066a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="7066a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7066a-114">Application</span></span> | <span data-ttu-id="7066a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7066a-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7066a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7066a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="7066a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7066a-117">Request headers</span></span>

| <span data-ttu-id="7066a-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7066a-118">Header</span></span> | <span data-ttu-id="7066a-119">Valor</span><span class="sxs-lookup"><span data-stu-id="7066a-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="7066a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7066a-120">Authorization</span></span> | <span data-ttu-id="7066a-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="7066a-121"></span></span> <span data-ttu-id="7066a-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7066a-122">Required.</span></span> |
| <span data-ttu-id="7066a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7066a-123">Content-Type</span></span> | <span data-ttu-id="7066a-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="7066a-124"></span></span> <span data-ttu-id="7066a-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7066a-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7066a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7066a-126">Request body</span></span>

<span data-ttu-id="7066a-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7066a-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7066a-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7066a-128">Parameter</span></span> | <span data-ttu-id="7066a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="7066a-129">Type</span></span> | <span data-ttu-id="7066a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="7066a-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="7066a-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="7066a-131">destinationId</span></span>|<span data-ttu-id="7066a-132">String</span><span class="sxs-lookup"><span data-stu-id="7066a-132">String</span></span>|<span data-ttu-id="7066a-133">A ID da pasta de destino ou um nome de pasta bem conhecido.</span><span class="sxs-lookup"><span data-stu-id="7066a-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="7066a-134">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="7066a-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="7066a-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7066a-135">Response</span></span>

<span data-ttu-id="7066a-136">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o recurso [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7066a-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7066a-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7066a-137">Example</span></span>

<span data-ttu-id="7066a-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7066a-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="7066a-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7066a-139">Request</span></span>
<span data-ttu-id="7066a-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7066a-140">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7066a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="7066a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_copy"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/copy
Content-type: application/json
Content-length: 44

{
  "destinationId": "destinationId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7066a-142">C#</span><span class="sxs-lookup"><span data-stu-id="7066a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-copy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7066a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7066a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-copy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7066a-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7066a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-copy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7066a-145">Java</span><span class="sxs-lookup"><span data-stu-id="7066a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-copy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7066a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7066a-146">Response</span></span>

<span data-ttu-id="7066a-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7066a-147">Here is an example of the response.</span></span>

> <span data-ttu-id="7066a-148">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7066a-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7066a-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7066a-149">All the properties will be returned from an actual call.</span></span>
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
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
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
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
