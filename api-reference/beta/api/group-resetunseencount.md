---
title: 'group: resetUnseenCount'
description: Redefina o unseenCount das postagens que o usuário atual não observou desde sua última visita. Suporte para Office 365 apenas para grupos.
author: dkershaw10
ms.openlocfilehash: f63a3668bc9059819c09bdc43dd78a138196a241
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350152"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="f5cf6-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="f5cf6-104">group: resetUnseenCount</span></span>

> <span data-ttu-id="f5cf6-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5cf6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5cf6-107">Redefina o unseenCount das postagens que o usuário atual não observou desde sua última visita.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-107">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="f5cf6-108">Suporte para Office 365 apenas para grupos.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5cf6-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5cf6-109">Permissions</span></span>
<span data-ttu-id="f5cf6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5cf6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5cf6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5cf6-112">Permission type</span></span>      | <span data-ttu-id="f5cf6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5cf6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5cf6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5cf6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f5cf6-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5cf6-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f5cf6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5cf6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5cf6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-117">Not supported.</span></span>    |
|<span data-ttu-id="f5cf6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5cf6-118">Application</span></span> | <span data-ttu-id="f5cf6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5cf6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5cf6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="f5cf6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5cf6-121">Request headers</span></span>
| <span data-ttu-id="f5cf6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f5cf6-122">Header</span></span>       | <span data-ttu-id="f5cf6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f5cf6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f5cf6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5cf6-124">Authorization</span></span>  | <span data-ttu-id="f5cf6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5cf6-127">Preferir</span><span class="sxs-lookup"><span data-stu-id="f5cf6-127">Prefer</span></span> | <span data-ttu-id="f5cf6-128">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-128">return=minimal.</span></span> <span data-ttu-id="f5cf6-129">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f5cf6-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f5cf6-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5cf6-131">Request body</span></span>
<span data-ttu-id="f5cf6-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5cf6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5cf6-133">Response</span></span>
<span data-ttu-id="f5cf6-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5cf6-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5cf6-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f5cf6-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5cf6-137">Request</span></span>
<span data-ttu-id="f5cf6-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="f5cf6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5cf6-139">Response</span></span>
<span data-ttu-id="f5cf6-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5cf6-140">The following is an example of the response.</span></span> 
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
