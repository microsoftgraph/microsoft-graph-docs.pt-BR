---
title: 'group: addFavorite'
description: Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.
localization_priority: Normal
ms.openlocfilehash: 33a6b0b44aa680db4164debdf6994a69f205ad14
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813248"
---
# <a name="group-addfavorite"></a><span data-ttu-id="d4720-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="d4720-104">group: addFavorite</span></span>

> <span data-ttu-id="d4720-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d4720-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4720-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d4720-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4720-p103">Adicionar o grupo à lista de grupos de favoritos do usuário atual. Com suporte apenas para grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="d4720-p103">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4720-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4720-109">Permissions</span></span>
<span data-ttu-id="d4720-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4720-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4720-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4720-112">Permission type</span></span>      | <span data-ttu-id="d4720-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4720-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4720-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4720-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d4720-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4720-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d4720-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4720-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4720-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4720-117">Not supported.</span></span>    |
|<span data-ttu-id="d4720-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4720-118">Application</span></span> | <span data-ttu-id="d4720-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4720-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4720-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4720-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="d4720-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4720-121">Request headers</span></span>
| <span data-ttu-id="d4720-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4720-122">Header</span></span>       | <span data-ttu-id="d4720-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d4720-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d4720-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4720-124">Authorization</span></span>  | <span data-ttu-id="d4720-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4720-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d4720-127">Preferir</span><span class="sxs-lookup"><span data-stu-id="d4720-127">Prefer</span></span> | <span data-ttu-id="d4720-128">retorno=mínimo.</span><span class="sxs-lookup"><span data-stu-id="d4720-128">return=minimal.</span></span> <span data-ttu-id="d4720-129">Se o cabeçalho de resposta mínimo estiver incluído no cabeçalho da solicitação, uma resposta bem-sucedida retornará o código `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d4720-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="d4720-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d4720-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="d4720-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4720-131">Request body</span></span>
<span data-ttu-id="d4720-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4720-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4720-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4720-133">Response</span></span>
<span data-ttu-id="d4720-p107">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4720-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4720-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4720-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d4720-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4720-137">Request</span></span>
<span data-ttu-id="d4720-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4720-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="d4720-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4720-139">Response</span></span>
<span data-ttu-id="d4720-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d4720-140">The following is an example of the response.</span></span>
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
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
