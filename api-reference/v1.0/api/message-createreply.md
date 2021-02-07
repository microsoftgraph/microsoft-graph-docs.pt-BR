---
title: 'message: createReply'
description: Crie um rascunho da resposta para a mensagem especificada. Você pode atualizar o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente enviar o rascunho.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f19e393f3816b411f341e6cdba176796a412f24e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130624"
---
# <a name="message-createreply"></a><span data-ttu-id="2c8de-104">message: createReply</span><span class="sxs-lookup"><span data-stu-id="2c8de-104">message: createReply</span></span>

<span data-ttu-id="2c8de-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c8de-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2c8de-106">Crie um rascunho da resposta para a [mensagem](../resources/message.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="2c8de-106">Create a draft of the reply to the specified [message](../resources/message.md).</span></span> <span data-ttu-id="2c8de-107">Você pode [atualizar](../api/message-update.md) o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente [enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="2c8de-107">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c8de-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="2c8de-108">Permissions</span></span>
<span data-ttu-id="2c8de-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c8de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c8de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c8de-111">Permission type</span></span>      | <span data-ttu-id="2c8de-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c8de-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c8de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c8de-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2c8de-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c8de-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2c8de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c8de-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c8de-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c8de-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2c8de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c8de-117">Application</span></span> | <span data-ttu-id="2c8de-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c8de-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c8de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c8de-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReply
POST /users/{id | userPrincipalName}/messages/{id}/createReply
POST /me/mailFolders/{id}/messages/{id}/createReply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReply
```
## <a name="request-headers"></a><span data-ttu-id="2c8de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8de-120">Request headers</span></span>
| <span data-ttu-id="2c8de-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2c8de-121">Name</span></span>       | <span data-ttu-id="2c8de-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c8de-122">Type</span></span> | <span data-ttu-id="2c8de-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8de-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2c8de-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c8de-124">Authorization</span></span>  | <span data-ttu-id="2c8de-125">string</span><span class="sxs-lookup"><span data-stu-id="2c8de-125">string</span></span>  | <span data-ttu-id="2c8de-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c8de-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c8de-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8de-128">Request body</span></span>
<span data-ttu-id="2c8de-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c8de-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c8de-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c8de-130">Response</span></span>

<span data-ttu-id="2c8de-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c8de-131">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c8de-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c8de-132">Example</span></span>
<span data-ttu-id="2c8de-133">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2c8de-133">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2c8de-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c8de-134">Request</span></span>
<span data-ttu-id="2c8de-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c8de-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c8de-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c8de-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReply
```
# <a name="c"></a>[<span data-ttu-id="2c8de-137">C#</span><span class="sxs-lookup"><span data-stu-id="2c8de-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c8de-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c8de-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c8de-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c8de-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c8de-140">Java</span><span class="sxs-lookup"><span data-stu-id="2c8de-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-createreply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2c8de-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c8de-141">Response</span></span>
<span data-ttu-id="2c8de-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c8de-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "message: createReply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

