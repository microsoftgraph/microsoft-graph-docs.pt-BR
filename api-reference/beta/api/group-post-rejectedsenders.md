---
title: Criar rejectedSender
description: Adiciona um novo usuário ou grupo à lista rejectedSender.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 5fb46567e0fe4f6fe877a9128689611f49bc4f1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823976"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="aba57-103">Criar rejectedSender</span><span class="sxs-lookup"><span data-stu-id="aba57-103">Create rejectedSender</span></span>

> <span data-ttu-id="aba57-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="aba57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aba57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aba57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aba57-106">Adiciona um novo usuário ou grupo à lista rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="aba57-106">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="aba57-p102">Especifique o usuário ou grupo em `@odata.id` no corpo da solicitação. Os usuários na lista de remetentes rejeitados não podem postar em conversas do grupo (identificado na URL da solicitação POST). Certifique-se de não especificar o mesmo usuário ou grupo nas listas de remetentes aceitos e rejeitados, caso contrário você receberá um erro.</span><span class="sxs-lookup"><span data-stu-id="aba57-p102">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="aba57-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="aba57-110">Permissions</span></span>
<span data-ttu-id="aba57-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aba57-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aba57-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aba57-113">Permission type</span></span>      | <span data-ttu-id="aba57-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aba57-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aba57-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aba57-115">Delegated (work or school account)</span></span> | <span data-ttu-id="aba57-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aba57-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="aba57-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aba57-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aba57-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba57-118">Not supported.</span></span>    |
|<span data-ttu-id="aba57-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aba57-119">Application</span></span> | <span data-ttu-id="aba57-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba57-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aba57-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aba57-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="aba57-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aba57-122">Request headers</span></span>
| <span data-ttu-id="aba57-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aba57-123">Header</span></span>       | <span data-ttu-id="aba57-124">Valor</span><span class="sxs-lookup"><span data-stu-id="aba57-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aba57-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="aba57-125">Authorization</span></span>  | <span data-ttu-id="aba57-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aba57-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aba57-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aba57-128">Request body</span></span>
<span data-ttu-id="aba57-129">No corpo da solicitação, forneça a id de um objeto de usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="aba57-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="aba57-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba57-130">Response</span></span>
<span data-ttu-id="aba57-131">Este método retorna o código de resposta `204 No Content` e nenhum corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aba57-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="aba57-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aba57-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="aba57-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aba57-133">Request</span></span>
<span data-ttu-id="aba57-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aba57-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="aba57-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba57-135">Response</span></span>
<span data-ttu-id="aba57-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aba57-136">The following is an example of the response.</span></span>
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
