---
title: 'message: send'
description: Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um novo rascunho de mensagem, rascunho de resposta, responder-todos os rascunhos ou
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 5e7689e2b0bdd07c1739b4d3f640eb71b8dd0a35
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540412"
---
# <a name="message-send"></a><span data-ttu-id="d44ce-104">message: send</span><span class="sxs-lookup"><span data-stu-id="d44ce-104">message: send</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d44ce-p102">Envie uma mensagem na pasta de rascunho. A mensagem de rascunho pode ser um rascunho de mensagem nova, rascunho de resposta, rascunho de resposta a todos ou rascunho de encaminhamento. A mensagem é salva na pasta Itens Enviados.</span><span class="sxs-lookup"><span data-stu-id="d44ce-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="d44ce-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d44ce-108">Permissions</span></span>

<span data-ttu-id="d44ce-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d44ce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d44ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d44ce-111">Permission type</span></span>      | <span data-ttu-id="d44ce-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d44ce-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d44ce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d44ce-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d44ce-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d44ce-114">Mail.Send</span></span>    |
|<span data-ttu-id="d44ce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d44ce-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d44ce-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d44ce-116">Mail.Send</span></span>    |
|<span data-ttu-id="d44ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d44ce-117">Application</span></span> | <span data-ttu-id="d44ce-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d44ce-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d44ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d44ce-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="d44ce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d44ce-120">Request headers</span></span>

| <span data-ttu-id="d44ce-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d44ce-121">Name</span></span>       | <span data-ttu-id="d44ce-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d44ce-122">Type</span></span> | <span data-ttu-id="d44ce-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d44ce-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d44ce-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d44ce-124">Authorization</span></span>  | <span data-ttu-id="d44ce-125">string</span><span class="sxs-lookup"><span data-stu-id="d44ce-125">string</span></span>  | <span data-ttu-id="d44ce-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d44ce-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d44ce-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="d44ce-128">Content-Length</span></span> | <span data-ttu-id="d44ce-129">number</span><span class="sxs-lookup"><span data-stu-id="d44ce-129">number</span></span> | <span data-ttu-id="d44ce-130">0. Required.</span><span class="sxs-lookup"><span data-stu-id="d44ce-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d44ce-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d44ce-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="d44ce-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="d44ce-132">Response</span></span>

<span data-ttu-id="d44ce-p105">Se bem-sucedido, este método retorna um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d44ce-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d44ce-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d44ce-135">Example</span></span>

<span data-ttu-id="d44ce-136">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="d44ce-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d44ce-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d44ce-137">Request</span></span>

<span data-ttu-id="d44ce-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d44ce-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="d44ce-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d44ce-139">Response</span></span>

<span data-ttu-id="d44ce-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d44ce-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-send.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
