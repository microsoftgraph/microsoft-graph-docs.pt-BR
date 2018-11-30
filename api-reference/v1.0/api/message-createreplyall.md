---
title: 'message: createReplyAll'
description: Crie um rascunho para responder ao remetente e a todos os destinatários da mensagem especificada. Você pode atualizar o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente enviar o rascunho.
ms.openlocfilehash: a48e5bf7f3ae330ff31a2b8d2827259798186c64
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007320"
---
# <a name="message-createreplyall"></a><span data-ttu-id="003df-104">message: createReplyAll</span><span class="sxs-lookup"><span data-stu-id="003df-104">message: createReplyAll</span></span>

<span data-ttu-id="003df-105">Crie um rascunho para responder ao remetente e a todos os destinatários da [mensagem](../resources/message.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="003df-105">Create a draft to reply to the sender and all the recipients of the specified [message](../resources/message.md).</span></span> <span data-ttu-id="003df-106">Você pode [atualizar](../api/message-update.md) o rascunho para adicionar conteúdo de resposta ao **corpo** ou alterar outras propriedades da mensagem, ou, simplesmente [enviar](../api/message-send.md) o rascunho.</span><span class="sxs-lookup"><span data-stu-id="003df-106">You can then [update](../api/message-update.md) the draft to add reply content to the **body** or change other message properties, or, simply [send](../api/message-send.md) the draft.</span></span>

## <a name="permissions"></a><span data-ttu-id="003df-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="003df-107">Permissions</span></span>
<span data-ttu-id="003df-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="003df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="003df-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="003df-110">Permission type</span></span>      | <span data-ttu-id="003df-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="003df-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="003df-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="003df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="003df-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003df-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="003df-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="003df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="003df-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003df-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="003df-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="003df-116">Application</span></span> | <span data-ttu-id="003df-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="003df-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="003df-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="003df-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/messages/{id}/createReplyAll
POST /me/mailFolders/{id}/messages/{id}/createReplyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/createReplyAll
```
## <a name="request-headers"></a><span data-ttu-id="003df-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="003df-119">Request headers</span></span>
| <span data-ttu-id="003df-120">Nome</span><span class="sxs-lookup"><span data-stu-id="003df-120">Name</span></span>       | <span data-ttu-id="003df-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="003df-121">Type</span></span> | <span data-ttu-id="003df-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="003df-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="003df-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="003df-123">Authorization</span></span>  | <span data-ttu-id="003df-124">string</span><span class="sxs-lookup"><span data-stu-id="003df-124">string</span></span>  | <span data-ttu-id="003df-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="003df-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="003df-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="003df-127">Request body</span></span>
<span data-ttu-id="003df-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="003df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="003df-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="003df-129">Response</span></span>

<span data-ttu-id="003df-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="003df-130">If successful, this method returns `201 Created` response code and [Message](../resources/message.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="003df-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="003df-131">Example</span></span>
<span data-ttu-id="003df-132">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="003df-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="003df-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="003df-133">Request</span></span>
<span data-ttu-id="003df-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="003df-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_createreplyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/createReplyAll
```

##### <a name="response"></a><span data-ttu-id="003df-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="003df-135">Response</span></span>
<span data-ttu-id="003df-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="003df-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
