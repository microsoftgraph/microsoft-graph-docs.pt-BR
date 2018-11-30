---
title: 'group: resetUnseenCount'
description: Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.
ms.openlocfilehash: 9747c0676a140abbab0bef66733dba7730fc397c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007159"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="56d45-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="56d45-104">group: resetUnseenCount</span></span>
<span data-ttu-id="56d45-p102">Redefina a unseenCount de todas as postagens que o usuário atual não viu desde sua última visita. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="56d45-p102">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="56d45-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="56d45-107">Permissions</span></span>
<span data-ttu-id="56d45-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d45-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d45-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56d45-110">Permission type</span></span>      | <span data-ttu-id="56d45-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56d45-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56d45-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56d45-112">Delegated (work or school account)</span></span> | <span data-ttu-id="56d45-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56d45-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="56d45-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56d45-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d45-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56d45-115">Not supported.</span></span>    |
|<span data-ttu-id="56d45-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56d45-116">Application</span></span> | <span data-ttu-id="56d45-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56d45-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56d45-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56d45-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="56d45-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56d45-119">Request headers</span></span>
| <span data-ttu-id="56d45-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56d45-120">Header</span></span>       | <span data-ttu-id="56d45-121">Valor</span><span class="sxs-lookup"><span data-stu-id="56d45-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="56d45-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="56d45-122">Authorization</span></span>  | <span data-ttu-id="56d45-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56d45-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="56d45-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="56d45-125">Prefer</span></span> | <span data-ttu-id="56d45-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="56d45-126">return=minimal.</span></span> <span data-ttu-id="56d45-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="56d45-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="56d45-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="56d45-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="56d45-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56d45-129">Request body</span></span>
<span data-ttu-id="56d45-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56d45-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56d45-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="56d45-131">Response</span></span>
<span data-ttu-id="56d45-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56d45-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56d45-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56d45-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="56d45-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56d45-135">Request</span></span>
<span data-ttu-id="56d45-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="56d45-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="56d45-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="56d45-137">Response</span></span>
<span data-ttu-id="56d45-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="56d45-138">The following is an example of the response.</span></span> 
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
