---
title: 'group: addFavorite'
description: Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.
localization_priority: Normal
ms.openlocfilehash: 2de37dccfa1912240b6ac131c700d3031b2ea2b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826730"
---
# <a name="group-addfavorite"></a><span data-ttu-id="6c7de-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="6c7de-104">group: addFavorite</span></span>
<span data-ttu-id="6c7de-p102">Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="6c7de-p102">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c7de-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c7de-107">Permissions</span></span>
<span data-ttu-id="6c7de-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c7de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c7de-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c7de-110">Permission type</span></span>      | <span data-ttu-id="6c7de-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c7de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c7de-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c7de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c7de-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c7de-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6c7de-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c7de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c7de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c7de-115">Not supported.</span></span>    |
|<span data-ttu-id="6c7de-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c7de-116">Application</span></span> | <span data-ttu-id="6c7de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c7de-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c7de-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c7de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="6c7de-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7de-119">Request headers</span></span>
| <span data-ttu-id="6c7de-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c7de-120">Header</span></span>       | <span data-ttu-id="6c7de-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c7de-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6c7de-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c7de-122">Authorization</span></span>  | <span data-ttu-id="6c7de-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c7de-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6c7de-125">Preferir</span><span class="sxs-lookup"><span data-stu-id="6c7de-125">Prefer</span></span> | <span data-ttu-id="6c7de-126">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="6c7de-126">return=minimal.</span></span> <span data-ttu-id="6c7de-127">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6c7de-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="6c7de-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6c7de-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6c7de-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7de-129">Request body</span></span>
<span data-ttu-id="6c7de-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c7de-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c7de-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7de-131">Response</span></span>
<span data-ttu-id="6c7de-p106">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c7de-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c7de-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c7de-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6c7de-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c7de-135">Request</span></span>
<span data-ttu-id="6c7de-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c7de-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="6c7de-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c7de-137">Response</span></span>
<span data-ttu-id="6c7de-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6c7de-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
