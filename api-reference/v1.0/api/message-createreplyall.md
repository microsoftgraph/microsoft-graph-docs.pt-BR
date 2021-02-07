---
title: 'message: createReplyAll'
description: Crie um rascunho para responder ao remetente e a todos os destinatários da mensagem especificada. Você pode atualizar o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente enviar o rascunho.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 629bf42c6d933a33008e40ab23a13a6ec08f233b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130603"
---
# <a name="message-createreplyall"></a><span data-ttu-id="32dd9-104">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="32dd9-104">message: createReplyAll</span></span>

<span data-ttu-id="32dd9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32dd9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="32dd9-106">Crie um rascunho para responder ao remetente e a todos os destinatários da [mensagem](../resources/message.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="32dd9-106">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="32dd9-107">Você pode [atualizar](../api/message-update.md) o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente [enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="32dd9-107">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="32dd9-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="32dd9-108">Permissions</span></span>
<span data-ttu-id="32dd9-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32dd9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32dd9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32dd9-111">Permission type</span></span>      | <span data-ttu-id="32dd9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32dd9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32dd9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32dd9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="32dd9-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32dd9-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32dd9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32dd9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32dd9-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32dd9-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="32dd9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32dd9-117">Application</span></span> | <span data-ttu-id="32dd9-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="32dd9-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="32dd9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32dd9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="32dd9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32dd9-120">Request headers</span></span>
| <span data-ttu-id="32dd9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="32dd9-121">Name</span></span>       | <span data-ttu-id="32dd9-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="32dd9-122">Type</span></span> | <span data-ttu-id="32dd9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="32dd9-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="32dd9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="32dd9-124">Authorization</span></span>  | <span data-ttu-id="32dd9-125">string</span><span class="sxs-lookup"><span data-stu-id="32dd9-125">string</span></span>  | <span data-ttu-id="32dd9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32dd9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="32dd9-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32dd9-128">Request body</span></span>
<span data-ttu-id="32dd9-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32dd9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="32dd9-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="32dd9-130">Response</span></span>

<span data-ttu-id="32dd9-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32dd9-131">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32dd9-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32dd9-132">Example</span></span>
<span data-ttu-id="32dd9-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="32dd9-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="32dd9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32dd9-134">Request</span></span>
<span data-ttu-id="32dd9-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32dd9-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="32dd9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="32dd9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```
# <a name="c"></a>[<span data-ttu-id="32dd9-137">C#</span><span class="sxs-lookup"><span data-stu-id="32dd9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="32dd9-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="32dd9-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="32dd9-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="32dd9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="32dd9-140">Java</span><span class="sxs-lookup"><span data-stu-id="32dd9-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreplyall-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="32dd9-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="32dd9-141">Response</span></span>
<span data-ttu-id="32dd9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32dd9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

