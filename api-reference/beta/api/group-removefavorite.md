---
title: 'group: removeFavorite'
description: Remova o grupo da lista de grupos favoritos do usuário atual. Suporte apenas para grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 9ed755add4771b062d004aaa35c55b9afd23a390
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951016"
---
# <a name="group-removefavorite"></a><span data-ttu-id="b8c9f-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="b8c9f-104">group: removeFavorite</span></span>

> <span data-ttu-id="b8c9f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8c9f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8c9f-p103">Remova o grupo da lista de grupos favoritos do usuário atual. Suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-p103">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8c9f-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8c9f-109">Permissions</span></span>
<span data-ttu-id="b8c9f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8c9f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8c9f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8c9f-112">Permission type</span></span>      | <span data-ttu-id="b8c9f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8c9f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8c9f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8c9f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b8c9f-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8c9f-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b8c9f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8c9f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8c9f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-117">Not supported.</span></span>    |
|<span data-ttu-id="b8c9f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8c9f-118">Application</span></span> | <span data-ttu-id="b8c9f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8c9f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8c9f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="b8c9f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8c9f-121">Request headers</span></span>
| <span data-ttu-id="b8c9f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b8c9f-122">Header</span></span>       | <span data-ttu-id="b8c9f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="b8c9f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8c9f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8c9f-124">Authorization</span></span>  | <span data-ttu-id="b8c9f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8c9f-127">Preferir</span><span class="sxs-lookup"><span data-stu-id="b8c9f-127">Prefer</span></span> | <span data-ttu-id="b8c9f-128">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-128">return=minimal.</span></span> <span data-ttu-id="b8c9f-129">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="b8c9f-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="b8c9f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8c9f-131">Request body</span></span>
<span data-ttu-id="b8c9f-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8c9f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8c9f-133">Response</span></span>
<span data-ttu-id="b8c9f-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8c9f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8c9f-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b8c9f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8c9f-137">Request</span></span>
<span data-ttu-id="b8c9f-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="b8c9f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8c9f-139">Response</span></span>
<span data-ttu-id="b8c9f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b8c9f-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
