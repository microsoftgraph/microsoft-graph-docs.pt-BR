---
title: 'message: createForward'
description: Crie um rascunho para encaminhar a mensagem especificada. Você pode atualizar o rascunho para adicionar conteúdo ao **corpo** ou alterar outras propriedades da mensagem ou, simplesmente, enviar o rascunho.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: eaafb6b86dd7392cd041a54247a47535ffc25039
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051344"
---
# <a name="message-createforward"></a><span data-ttu-id="22a11-104">message: createForward</span><span class="sxs-lookup"><span data-stu-id="22a11-104">message: createForward</span></span>

<span data-ttu-id="22a11-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22a11-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22a11-106">Crie um rascunho para encaminhar a [mensagem](../resources/message.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="22a11-106">Create a draft to forward the specified [message](../resources/message.md).</span></span> <span data-ttu-id="22a11-107">Você pode [atualizar](../api/message-update.md) o rascunho para adicionar conteúdo ao **corpo** ou alterar outras propriedades da mensagem ou, simplesmente, [enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="22a11-107">You can then [update](../api/message-update.md) the draft to add content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="22a11-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="22a11-108">Permissions</span></span>

<span data-ttu-id="22a11-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a11-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22a11-111">Permission type</span></span>      | <span data-ttu-id="22a11-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22a11-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22a11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22a11-113">Delegated (work or school account)</span></span> | <span data-ttu-id="22a11-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22a11-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="22a11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22a11-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22a11-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22a11-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="22a11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22a11-117">Application</span></span> | <span data-ttu-id="22a11-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="22a11-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="22a11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22a11-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/createForward
POST /users/{id | userPrincipalName}/messages/{id}/createForward
POST /me/mailFolders/{id}/messages/{id}/createForward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createForward
```

## <a name="request-headers"></a><span data-ttu-id="22a11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22a11-120">Request headers</span></span>

| <span data-ttu-id="22a11-121">Nome</span><span class="sxs-lookup"><span data-stu-id="22a11-121">Name</span></span>       | <span data-ttu-id="22a11-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="22a11-122">Type</span></span> | <span data-ttu-id="22a11-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="22a11-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="22a11-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="22a11-124">Authorization</span></span>  | <span data-ttu-id="22a11-125">string</span><span class="sxs-lookup"><span data-stu-id="22a11-125">string</span></span>  | <span data-ttu-id="22a11-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22a11-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22a11-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22a11-128">Request body</span></span>

<span data-ttu-id="22a11-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22a11-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22a11-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a11-130">Response</span></span>

<span data-ttu-id="22a11-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22a11-131">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a11-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22a11-132">Example</span></span>

<span data-ttu-id="22a11-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="22a11-133">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="22a11-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22a11-134">Request</span></span>

<span data-ttu-id="22a11-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22a11-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22a11-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="22a11-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createforward"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createForward
```
# <a name="c"></a>[<span data-ttu-id="22a11-137">C#</span><span class="sxs-lookup"><span data-stu-id="22a11-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createforward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22a11-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22a11-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createforward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22a11-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22a11-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createforward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22a11-140">Java</span><span class="sxs-lookup"><span data-stu-id="22a11-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createforward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="22a11-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="22a11-141">Response</span></span>

<span data-ttu-id="22a11-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22a11-142">Here is an example of the response.</span></span> <span data-ttu-id="22a11-143">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="22a11-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "message: createForward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

