---
title: 'message: createReplyAll'
description: Crie um rascunho para responder ao remetente e a todos os destinatários da mensagem especificada. Você pode atualizar o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente enviar o rascunho.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1e480c17f5891d2e4711ae32af539dc5682d67bc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444152"
---
# <a name="message-createreplyall"></a><span data-ttu-id="33179-104">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="33179-104">message: createReplyAll</span></span>

<span data-ttu-id="33179-105">Crie um rascunho para responder ao remetente e a todos os destinatários da [mensagem](../resources/message.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="33179-105">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="33179-106">Você pode [atualizar](../api/message-update.md) o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente [enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="33179-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="33179-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="33179-107">Permissions</span></span>
<span data-ttu-id="33179-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="33179-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33179-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="33179-110">Permission type</span></span>      | <span data-ttu-id="33179-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="33179-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33179-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="33179-112">Delegated (work or school account)</span></span> | <span data-ttu-id="33179-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33179-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="33179-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="33179-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33179-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33179-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="33179-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="33179-116">Application</span></span> | <span data-ttu-id="33179-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33179-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="33179-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="33179-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="33179-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="33179-119">Request headers</span></span>
| <span data-ttu-id="33179-120">Nome</span><span class="sxs-lookup"><span data-stu-id="33179-120">Name</span></span>       | <span data-ttu-id="33179-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="33179-121">Type</span></span> | <span data-ttu-id="33179-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="33179-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33179-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="33179-123">Authorization</span></span>  | <span data-ttu-id="33179-124">string</span><span class="sxs-lookup"><span data-stu-id="33179-124">string</span></span>  | <span data-ttu-id="33179-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="33179-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33179-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="33179-127">Request body</span></span>
<span data-ttu-id="33179-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="33179-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33179-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="33179-129">Response</span></span>

<span data-ttu-id="33179-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="33179-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33179-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="33179-131">Example</span></span>
<span data-ttu-id="33179-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="33179-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="33179-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="33179-133">Request</span></span>
<span data-ttu-id="33179-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="33179-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="33179-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="33179-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="33179-136">C#</span><span class="sxs-lookup"><span data-stu-id="33179-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-createreplyall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="33179-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="33179-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-createreplyall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="33179-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="33179-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-createreplyall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33179-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="33179-139">Response</span></span>
<span data-ttu-id="33179-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="33179-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
