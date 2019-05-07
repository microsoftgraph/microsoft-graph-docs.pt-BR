---
title: 'message: copy'
description: Copie uma mensagem para uma pasta.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 82e3670347da4616f0e41c3645d61d762eb1e252
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612770"
---
# <a name="message-copy"></a><span data-ttu-id="2e36c-103">message: copy</span><span class="sxs-lookup"><span data-stu-id="2e36c-103">message: copy</span></span>

<span data-ttu-id="2e36c-104">Copie uma mensagem para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="2e36c-104">Copy a message to a folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e36c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e36c-105">Permissions</span></span>

<span data-ttu-id="2e36c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e36c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e36c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e36c-108">Permission type</span></span> | <span data-ttu-id="2e36c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e36c-109">Permissions (from least to most privileged)</span></span> |
|:----------------|:--------------------------------------------|
|<span data-ttu-id="2e36c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e36c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2e36c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e36c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2e36c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e36c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e36c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e36c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2e36c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e36c-114">Application</span></span> | <span data-ttu-id="2e36c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2e36c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e36c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e36c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/copy
POST /users/{id | userPrincipalName}/messages/{id}/copy
POST /me/mailFolders/{id}/messages/{id}/copy
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/copy
```

## <a name="request-headers"></a><span data-ttu-id="2e36c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e36c-117">Request headers</span></span>

| <span data-ttu-id="2e36c-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e36c-118">Header</span></span> | <span data-ttu-id="2e36c-119">Valor</span><span class="sxs-lookup"><span data-stu-id="2e36c-119">Value</span></span> |
|:-------|:------|
| <span data-ttu-id="2e36c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e36c-120">Authorization</span></span> | <span data-ttu-id="2e36c-121">`Bearer {token}`.</span><span class="sxs-lookup"><span data-stu-id="2e36c-121"></span></span> <span data-ttu-id="2e36c-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e36c-122">Required.</span></span> |
| <span data-ttu-id="2e36c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2e36c-123">Content-Type</span></span> | <span data-ttu-id="2e36c-124">`application/json`.</span><span class="sxs-lookup"><span data-stu-id="2e36c-124"></span></span> <span data-ttu-id="2e36c-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e36c-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e36c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e36c-126">Request body</span></span>

<span data-ttu-id="2e36c-127">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e36c-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e36c-128">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2e36c-128">Parameter</span></span> | <span data-ttu-id="2e36c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e36c-129">Type</span></span> | <span data-ttu-id="2e36c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e36c-130">Description</span></span> |
|:----------|:-----|:------------|
|<span data-ttu-id="2e36c-131">destinationId</span><span class="sxs-lookup"><span data-stu-id="2e36c-131">destinationId</span></span>|<span data-ttu-id="2e36c-132">String</span><span class="sxs-lookup"><span data-stu-id="2e36c-132">String</span></span>|<span data-ttu-id="2e36c-133">A ID da pasta de destino ou um nome de pasta bem conhecido.</span><span class="sxs-lookup"><span data-stu-id="2e36c-133">The destination folder ID, or a well-known folder name.</span></span> <span data-ttu-id="2e36c-134">Confira uma lista de nomes de pasta comuns com suporte em [Tipo de recurso mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="2e36c-134">For a list of supported well-known folder names, see [mailFolder resource type](../resources/mailfolder.md).</span></span>|

## <a name="response"></a><span data-ttu-id="2e36c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e36c-135">Response</span></span>

<span data-ttu-id="2e36c-136">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o recurso [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e36c-136">If successful, this method returns `201 Created` response code and a [message](../resources/message.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e36c-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e36c-137">Example</span></span>

<span data-ttu-id="2e36c-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2e36c-138">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="2e36c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e36c-139">Request</span></span>
<span data-ttu-id="2e36c-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e36c-140">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2e36c-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e36c-141">Response</span></span>

<span data-ttu-id="2e36c-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e36c-142">Here is an example of the response.</span></span>

> <span data-ttu-id="2e36c-143">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2e36c-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2e36c-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e36c-144">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2e36c-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2e36c-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2e36c-146">Basic</span><span class="sxs-lookup"><span data-stu-id="2e36c-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_copy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2e36c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e36c-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_copy-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: copy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-copy.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
