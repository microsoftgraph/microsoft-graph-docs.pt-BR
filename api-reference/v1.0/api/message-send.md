---
title: 'message: send'
description: Envie uma mensagem na pasta rascunho. A mensagem de rascunho pode ser um rascunho da nova mensagem, rascunho de responder, responder a todos com rascunho, ou
ms.openlocfilehash: 8fe04db6a7fe4a469374cd54a00f308e01341274
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007051"
---
# <a name="message-send"></a><span data-ttu-id="cf2b7-104">message: send</span><span class="sxs-lookup"><span data-stu-id="cf2b7-104">message: send</span></span>

<span data-ttu-id="cf2b7-p102">Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="cf2b7-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf2b7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf2b7-108">Permissions</span></span>

<span data-ttu-id="cf2b7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf2b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf2b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf2b7-111">Permission type</span></span>      | <span data-ttu-id="cf2b7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf2b7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf2b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf2b7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cf2b7-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cf2b7-114">Mail.Send</span></span>    |
|<span data-ttu-id="cf2b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf2b7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf2b7-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cf2b7-116">Mail.Send</span></span>    |
|<span data-ttu-id="cf2b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf2b7-117">Application</span></span> | <span data-ttu-id="cf2b7-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cf2b7-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf2b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf2b7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="cf2b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf2b7-120">Request headers</span></span>

| <span data-ttu-id="cf2b7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cf2b7-121">Name</span></span>       | <span data-ttu-id="cf2b7-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf2b7-122">Type</span></span> | <span data-ttu-id="cf2b7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf2b7-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf2b7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf2b7-124">Authorization</span></span>  | <span data-ttu-id="cf2b7-125">string</span><span class="sxs-lookup"><span data-stu-id="cf2b7-125">string</span></span>  | <span data-ttu-id="cf2b7-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf2b7-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf2b7-128">Tamanho do conteúdo</span><span class="sxs-lookup"><span data-stu-id="cf2b7-128">Content-Length</span></span> | <span data-ttu-id="cf2b7-129">número</span><span class="sxs-lookup"><span data-stu-id="cf2b7-129">number</span></span> | <span data-ttu-id="cf2b7-130">0. necessária.</span><span class="sxs-lookup"><span data-stu-id="cf2b7-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf2b7-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf2b7-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="cf2b7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf2b7-132">Response</span></span>

<span data-ttu-id="cf2b7-p105">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf2b7-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf2b7-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf2b7-135">Example</span></span>

<span data-ttu-id="cf2b7-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cf2b7-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="cf2b7-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf2b7-137">Request</span></span>

<span data-ttu-id="cf2b7-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf2b7-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="cf2b7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf2b7-139">Response</span></span>

<span data-ttu-id="cf2b7-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf2b7-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
