---
title: 'group: subscribeByMail'
description: Chamar esse método permitirá que o usuário atual receber notificações de email para esse grupo, sobre novas postagens, eventos e arquivos nesse grupo. Suporte para Office 365 apenas para grupos.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: da277a586a793c07067f793088b15d4570efbf1c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984672"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="0f611-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="0f611-104">group: subscribeByMail</span></span>

> <span data-ttu-id="0f611-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0f611-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f611-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0f611-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0f611-107">Chamar esse método permitirá que o usuário atual receber notificações de email para esse grupo, sobre novas postagens, eventos e arquivos nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="0f611-107">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="0f611-108">Suporte para Office 365 apenas para grupos.</span><span class="sxs-lookup"><span data-stu-id="0f611-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f611-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0f611-109">Permissions</span></span>
<span data-ttu-id="0f611-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f611-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f611-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f611-112">Permission type</span></span>      | <span data-ttu-id="0f611-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0f611-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f611-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f611-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0f611-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f611-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0f611-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f611-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f611-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f611-117">Not supported.</span></span>    |
|<span data-ttu-id="0f611-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f611-118">Application</span></span> | <span data-ttu-id="0f611-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f611-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f611-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f611-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="0f611-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f611-121">Request headers</span></span>
| <span data-ttu-id="0f611-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f611-122">Header</span></span>       | <span data-ttu-id="0f611-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0f611-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0f611-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f611-124">Authorization</span></span>  | <span data-ttu-id="0f611-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f611-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0f611-127">Preferir</span><span class="sxs-lookup"><span data-stu-id="0f611-127">Prefer</span></span> | <span data-ttu-id="0f611-128">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="0f611-128">return=minimal.</span></span> <span data-ttu-id="0f611-129">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0f611-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="0f611-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0f611-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="0f611-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f611-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0f611-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f611-132">Response</span></span>
<span data-ttu-id="0f611-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f611-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f611-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f611-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0f611-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f611-136">Request</span></span>
<span data-ttu-id="0f611-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f611-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="0f611-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f611-138">Response</span></span>
<span data-ttu-id="0f611-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0f611-139">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
