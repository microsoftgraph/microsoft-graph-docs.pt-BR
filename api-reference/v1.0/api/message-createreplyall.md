---
title: 'message: createReplyAll'
description: Crie um rascunho para responder ao remetente e a todos os destinatários da mensagem especificada. Você pode atualizar o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente enviar o rascunho.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e343f09768e46378d8ec36a00d4dfa06b7170b0e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275695"
---
# <a name="message-createreplyall"></a><span data-ttu-id="dce9d-104">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="dce9d-104">message: createReplyAll</span></span>

<span data-ttu-id="dce9d-105">Crie um rascunho para responder ao remetente e a todos os destinatários da [mensagem](../resources/message.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="dce9d-105">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="dce9d-106">Você pode [atualizar](../api/message-update.md) o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente [enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="dce9d-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="dce9d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="dce9d-107">Permissions</span></span>
<span data-ttu-id="dce9d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dce9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dce9d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dce9d-110">Permission type</span></span>      | <span data-ttu-id="dce9d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dce9d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dce9d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dce9d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="dce9d-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dce9d-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dce9d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dce9d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dce9d-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dce9d-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="dce9d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dce9d-116">Application</span></span> | <span data-ttu-id="dce9d-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dce9d-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="dce9d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dce9d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="dce9d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dce9d-119">Request headers</span></span>
| <span data-ttu-id="dce9d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dce9d-120">Name</span></span>       | <span data-ttu-id="dce9d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="dce9d-121">Type</span></span> | <span data-ttu-id="dce9d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dce9d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dce9d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dce9d-123">Authorization</span></span>  | <span data-ttu-id="dce9d-124">string</span><span class="sxs-lookup"><span data-stu-id="dce9d-124">string</span></span>  | <span data-ttu-id="dce9d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dce9d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dce9d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dce9d-127">Request body</span></span>
<span data-ttu-id="dce9d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dce9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dce9d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dce9d-129">Response</span></span>

<span data-ttu-id="dce9d-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dce9d-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dce9d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dce9d-131">Example</span></span>
<span data-ttu-id="dce9d-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="dce9d-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dce9d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dce9d-133">Request</span></span>
<span data-ttu-id="dce9d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dce9d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```

##### <a name="response"></a><span data-ttu-id="dce9d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dce9d-135">Response</span></span>
<span data-ttu-id="dce9d-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dce9d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="dce9d-139">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dce9d-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dce9d-140">C#</span><span class="sxs-lookup"><span data-stu-id="dce9d-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_createreplyall-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dce9d-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="dce9d-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_createreplyall-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="dce9d-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="dce9d-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_createreplyall-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: createReplyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-createreplyall.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-createreplyall.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-createreplyall.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
