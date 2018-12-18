---
title: 'group: resetUnseenCount'
description: Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.
author: dkershaw10
ms.openlocfilehash: 6cb7533dc44ff86b2e1dbec5c99f4038ed03d224
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337454"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="01a1b-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="01a1b-104">group: resetUnseenCount</span></span>
<span data-ttu-id="01a1b-p102">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="01a1b-p102">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="01a1b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="01a1b-107">Permissions</span></span>
<span data-ttu-id="01a1b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01a1b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a1b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01a1b-110">Permission type</span></span>      | <span data-ttu-id="01a1b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01a1b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01a1b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01a1b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01a1b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01a1b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="01a1b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01a1b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01a1b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01a1b-115">Not supported.</span></span>    |
|<span data-ttu-id="01a1b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01a1b-116">Application</span></span> | <span data-ttu-id="01a1b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01a1b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01a1b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01a1b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="01a1b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01a1b-119">Request headers</span></span>
| <span data-ttu-id="01a1b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01a1b-120">Header</span></span>       | <span data-ttu-id="01a1b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="01a1b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01a1b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="01a1b-122">Authorization</span></span>  | <span data-ttu-id="01a1b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01a1b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01a1b-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="01a1b-125">Prefer</span></span> | <span data-ttu-id="01a1b-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="01a1b-126">return=minimal.</span></span> <span data-ttu-id="01a1b-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="01a1b-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="01a1b-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="01a1b-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="01a1b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01a1b-129">Request body</span></span>
<span data-ttu-id="01a1b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01a1b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01a1b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="01a1b-131">Response</span></span>
<span data-ttu-id="01a1b-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01a1b-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01a1b-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01a1b-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="01a1b-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01a1b-135">Request</span></span>
<span data-ttu-id="01a1b-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="01a1b-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="01a1b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="01a1b-137">Response</span></span>
<span data-ttu-id="01a1b-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="01a1b-138">The following is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
