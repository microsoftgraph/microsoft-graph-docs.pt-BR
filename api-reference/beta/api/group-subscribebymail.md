---
title: 'group: subscribeByMail'
description: Chamar esse método permitirá que o usuário atual receber notificações de email para esse grupo, sobre novas postagens, eventos e arquivos nesse grupo. Suporte para Office 365 apenas para grupos.
localization_priority: Normal
ms.openlocfilehash: 5cbb5d461f5e3cc71790f6546c6ebf638ffa31d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813164"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="0a3e2-104">group: subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="0a3e2-104">group: subscribeByMail</span></span>

> <span data-ttu-id="0a3e2-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a3e2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a3e2-107">Chamar esse método permitirá que o usuário atual receber notificações de email para esse grupo, sobre novas postagens, eventos e arquivos nesse grupo.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-107">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="0a3e2-108">Suporte para Office 365 apenas para grupos.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a3e2-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="0a3e2-109">Permissions</span></span>
<span data-ttu-id="0a3e2-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3e2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3e2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0a3e2-112">Permission type</span></span>      | <span data-ttu-id="0a3e2-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0a3e2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a3e2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0a3e2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0a3e2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3e2-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a3e2-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0a3e2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a3e2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-117">Not supported.</span></span>    |
|<span data-ttu-id="0a3e2-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0a3e2-118">Application</span></span> | <span data-ttu-id="0a3e2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a3e2-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0a3e2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="0a3e2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3e2-121">Request headers</span></span>
| <span data-ttu-id="0a3e2-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0a3e2-122">Header</span></span>       | <span data-ttu-id="0a3e2-123">Valor</span><span class="sxs-lookup"><span data-stu-id="0a3e2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a3e2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0a3e2-124">Authorization</span></span>  | <span data-ttu-id="0a3e2-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a3e2-127">Preferir</span><span class="sxs-lookup"><span data-stu-id="0a3e2-127">Prefer</span></span> | <span data-ttu-id="0a3e2-128">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-128">return=minimal.</span></span> <span data-ttu-id="0a3e2-129">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="0a3e2-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="0a3e2-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3e2-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0a3e2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a3e2-132">Response</span></span>
<span data-ttu-id="0a3e2-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a3e2-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0a3e2-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0a3e2-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0a3e2-136">Request</span></span>
<span data-ttu-id="0a3e2-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="0a3e2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0a3e2-138">Response</span></span>
<span data-ttu-id="0a3e2-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0a3e2-139">The following is an example of the response.</span></span> 
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
