---
title: Criar rejectedSender
description: Adiciona um novo usuário ou grupo à lista rejectedSender.
author: dkershaw10
ms.openlocfilehash: 08156823a8a7e7ad6075afee49ff979c3955e70a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350075"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="8f00e-103">Criar rejectedSender</span><span class="sxs-lookup"><span data-stu-id="8f00e-103">Create rejectedSender</span></span>

> <span data-ttu-id="8f00e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f00e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f00e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f00e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f00e-106">Adiciona um novo usuário ou grupo à lista rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="8f00e-106">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="8f00e-p102">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação POST). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="8f00e-p102">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f00e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="8f00e-110">Permissions</span></span>
<span data-ttu-id="8f00e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f00e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f00e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f00e-113">Permission type</span></span>      | <span data-ttu-id="8f00e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8f00e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f00e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f00e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="8f00e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f00e-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8f00e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f00e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f00e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f00e-118">Not supported.</span></span>    |
|<span data-ttu-id="8f00e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f00e-119">Application</span></span> | <span data-ttu-id="8f00e-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f00e-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f00e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f00e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8f00e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f00e-122">Request headers</span></span>
| <span data-ttu-id="8f00e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f00e-123">Header</span></span>       | <span data-ttu-id="8f00e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="8f00e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8f00e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f00e-125">Authorization</span></span>  | <span data-ttu-id="8f00e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f00e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8f00e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f00e-128">Request body</span></span>
<span data-ttu-id="8f00e-129">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="8f00e-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="8f00e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f00e-130">Response</span></span>
<span data-ttu-id="8f00e-131">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f00e-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f00e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f00e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8f00e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f00e-133">Request</span></span>
<span data-ttu-id="8f00e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f00e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rejectedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="8f00e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f00e-135">Response</span></span>
<span data-ttu-id="8f00e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8f00e-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
