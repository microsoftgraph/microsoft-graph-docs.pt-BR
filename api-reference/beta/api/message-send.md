---
title: 'message: send'
description: Envie uma mensagem na pasta rascunho. A mensagem de rascunho pode ser um rascunho da nova mensagem, rascunho de responder, responder a todos com rascunho, ou
ms.openlocfilehash: b295cd5b234bf9dafe1fbba44a03cdc6e9c1842e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038947"
---
# <a name="message-send"></a><span data-ttu-id="cce9f-104">message: send</span><span class="sxs-lookup"><span data-stu-id="cce9f-104">message: send</span></span>

> <span data-ttu-id="cce9f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cce9f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cce9f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cce9f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cce9f-p103">Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="cce9f-p103">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="cce9f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="cce9f-110">Permissions</span></span>

<span data-ttu-id="cce9f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cce9f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cce9f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cce9f-113">Permission type</span></span>      | <span data-ttu-id="cce9f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cce9f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cce9f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cce9f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="cce9f-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cce9f-116">Mail.Send</span></span>    |
|<span data-ttu-id="cce9f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cce9f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cce9f-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cce9f-118">Mail.Send</span></span>    |
|<span data-ttu-id="cce9f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cce9f-119">Application</span></span> | <span data-ttu-id="cce9f-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="cce9f-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="cce9f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cce9f-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="cce9f-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cce9f-122">Request headers</span></span>

| <span data-ttu-id="cce9f-123">Nome</span><span class="sxs-lookup"><span data-stu-id="cce9f-123">Name</span></span>       | <span data-ttu-id="cce9f-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="cce9f-124">Type</span></span> | <span data-ttu-id="cce9f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cce9f-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cce9f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="cce9f-126">Authorization</span></span>  | <span data-ttu-id="cce9f-127">string</span><span class="sxs-lookup"><span data-stu-id="cce9f-127">string</span></span>  | <span data-ttu-id="cce9f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cce9f-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cce9f-130">Tamanho do conteúdo</span><span class="sxs-lookup"><span data-stu-id="cce9f-130">Content-Length</span></span> | <span data-ttu-id="cce9f-131">número</span><span class="sxs-lookup"><span data-stu-id="cce9f-131">number</span></span> | <span data-ttu-id="cce9f-132">0. necessária.</span><span class="sxs-lookup"><span data-stu-id="cce9f-132">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cce9f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cce9f-133">Request body</span></span>

## <a name="response"></a><span data-ttu-id="cce9f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cce9f-134">Response</span></span>

<span data-ttu-id="cce9f-p106">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cce9f-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cce9f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cce9f-137">Example</span></span>

<span data-ttu-id="cce9f-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="cce9f-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cce9f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cce9f-139">Request</span></span>

<span data-ttu-id="cce9f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cce9f-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="cce9f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cce9f-141">Response</span></span>

<span data-ttu-id="cce9f-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cce9f-142">Here is an example of the response.</span></span>
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
