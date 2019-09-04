---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7ce86133178a00a936893af2e585515964bf8cf9
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721569"
---
# <a name="list-photos"></a><span data-ttu-id="7b421-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="7b421-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b421-104">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="7b421-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b421-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b421-105">Permissions</span></span>
<span data-ttu-id="7b421-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b421-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b421-108">Permission type</span></span>      | <span data-ttu-id="7b421-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b421-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b421-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b421-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7b421-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b421-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b421-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b421-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b421-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b421-113">Not supported.</span></span>    |
|<span data-ttu-id="7b421-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b421-114">Application</span></span> | <span data-ttu-id="7b421-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b421-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b421-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b421-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b421-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7b421-117">Optional query parameters</span></span>
<span data-ttu-id="7b421-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7b421-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b421-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b421-119">Request headers</span></span>
| <span data-ttu-id="7b421-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7b421-120">Name</span></span>       | <span data-ttu-id="7b421-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b421-121">Type</span></span> | <span data-ttu-id="7b421-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b421-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7b421-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b421-123">Authorization</span></span>  | <span data-ttu-id="7b421-124">string</span><span class="sxs-lookup"><span data-stu-id="7b421-124">string</span></span>  | <span data-ttu-id="7b421-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b421-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b421-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b421-127">Request body</span></span>
<span data-ttu-id="7b421-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b421-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b421-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b421-129">Response</span></span>
<span data-ttu-id="7b421-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b421-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b421-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b421-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7b421-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b421-132">Request</span></span>
<span data-ttu-id="7b421-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b421-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7b421-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b421-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7b421-135">C#</span><span class="sxs-lookup"><span data-stu-id="7b421-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b421-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b421-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7b421-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7b421-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7b421-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b421-138">Response</span></span>
<span data-ttu-id="7b421-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b421-139">The following is an example of the response.</span></span>
><span data-ttu-id="7b421-140">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7b421-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7b421-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b421-141">All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
