---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 57676cff7fd85cb12c46f7da1294da3653766ca0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263025"
---
# <a name="list-photos"></a><span data-ttu-id="3d9ce-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="3d9ce-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d9ce-104">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="3d9ce-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d9ce-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d9ce-105">Permissions</span></span>
<span data-ttu-id="3d9ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d9ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d9ce-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d9ce-108">Permission type</span></span>      | <span data-ttu-id="3d9ce-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d9ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d9ce-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d9ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d9ce-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d9ce-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d9ce-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d9ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d9ce-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-113">Not supported.</span></span>    |
|<span data-ttu-id="3d9ce-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3d9ce-114">Application</span></span> | <span data-ttu-id="3d9ce-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d9ce-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d9ce-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d9ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d9ce-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3d9ce-117">Optional query parameters</span></span>
<span data-ttu-id="3d9ce-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d9ce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d9ce-119">Request headers</span></span>
| <span data-ttu-id="3d9ce-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3d9ce-120">Name</span></span>       | <span data-ttu-id="3d9ce-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d9ce-121">Type</span></span> | <span data-ttu-id="3d9ce-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d9ce-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3d9ce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d9ce-123">Authorization</span></span>  | <span data-ttu-id="3d9ce-124">string</span><span class="sxs-lookup"><span data-stu-id="3d9ce-124">string</span></span>  | <span data-ttu-id="3d9ce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d9ce-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d9ce-127">Request body</span></span>
<span data-ttu-id="3d9ce-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d9ce-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d9ce-129">Response</span></span>
<span data-ttu-id="3d9ce-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d9ce-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d9ce-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3d9ce-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d9ce-132">Request</span></span>
<span data-ttu-id="3d9ce-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="3d9ce-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d9ce-134">Response</span></span>
<span data-ttu-id="3d9ce-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-135">The following is an example of the response.</span></span>
><span data-ttu-id="3d9ce-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3d9ce-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3d9ce-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profilePhoto",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 94

{
  "value": [
    {
      "height": 99,
      "width": 99,
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d9ce-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3d9ce-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d9ce-139">C#</span><span class="sxs-lookup"><span data-stu-id="3d9ce-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photos-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d9ce-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d9ce-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photos-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d9ce-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3d9ce-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_photos-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
