---
title: 'message: replyAll'
description: Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 8e2d9b2481e4fb0fc4e6e166dae1189baa77b7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884305"
---
# <a name="message-replyall"></a><span data-ttu-id="c3b75-104">message: replyAll</span><span class="sxs-lookup"><span data-stu-id="c3b75-104">message: replyAll</span></span>

<span data-ttu-id="c3b75-p102">Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="c3b75-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3b75-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3b75-107">Permissions</span></span>
<span data-ttu-id="c3b75-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3b75-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3b75-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3b75-110">Permission type</span></span>      | <span data-ttu-id="c3b75-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3b75-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3b75-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3b75-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c3b75-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3b75-113">Mail.Send</span></span>    |
|<span data-ttu-id="c3b75-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3b75-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3b75-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3b75-115">Mail.Send</span></span>    |
|<span data-ttu-id="c3b75-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3b75-116">Application</span></span> | <span data-ttu-id="c3b75-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="c3b75-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3b75-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3b75-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="c3b75-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3b75-119">Request headers</span></span>
| <span data-ttu-id="c3b75-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c3b75-120">Name</span></span>       | <span data-ttu-id="c3b75-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3b75-121">Type</span></span> | <span data-ttu-id="c3b75-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3b75-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3b75-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3b75-123">Authorization</span></span>  | <span data-ttu-id="c3b75-124">string</span><span class="sxs-lookup"><span data-stu-id="c3b75-124">string</span></span>  | <span data-ttu-id="c3b75-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3b75-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c3b75-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3b75-127">Content-Type</span></span> | <span data-ttu-id="c3b75-128">string</span><span class="sxs-lookup"><span data-stu-id="c3b75-128">string</span></span>  | <span data-ttu-id="c3b75-p105">Natureza dos dados no corpo de uma entidade. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3b75-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3b75-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3b75-131">Request body</span></span>
<span data-ttu-id="c3b75-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3b75-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c3b75-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c3b75-133">Parameter</span></span>    | <span data-ttu-id="c3b75-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3b75-134">Type</span></span>   |<span data-ttu-id="c3b75-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3b75-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3b75-136">comment</span><span class="sxs-lookup"><span data-stu-id="c3b75-136">comment</span></span>|<span data-ttu-id="c3b75-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3b75-137">String</span></span>|<span data-ttu-id="c3b75-p106">Um comentário a incluir. Não pode ficar vazio.</span><span class="sxs-lookup"><span data-stu-id="c3b75-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="c3b75-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3b75-140">Response</span></span>

<span data-ttu-id="c3b75-p107">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3b75-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3b75-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3b75-143">Example</span></span>
<span data-ttu-id="c3b75-144">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c3b75-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c3b75-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3b75-145">Request</span></span>
<span data-ttu-id="c3b75-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3b75-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="c3b75-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3b75-147">Response</span></span>
<span data-ttu-id="c3b75-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3b75-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
