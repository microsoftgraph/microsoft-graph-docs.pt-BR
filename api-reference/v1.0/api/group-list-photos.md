---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9190ef5fe88ccba98fb50d4da5f31fce918b3115
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016252"
---
# <a name="list-photos"></a><span data-ttu-id="0ae5c-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="0ae5c-103">List photos</span></span>
<span data-ttu-id="0ae5c-104">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="0ae5c-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ae5c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ae5c-105">Permissions</span></span>
<span data-ttu-id="0ae5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ae5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ae5c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ae5c-108">Permission type</span></span>      | <span data-ttu-id="0ae5c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ae5c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ae5c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ae5c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ae5c-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ae5c-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="0ae5c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ae5c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ae5c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-113">Not supported.</span></span>    |
|<span data-ttu-id="0ae5c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ae5c-114">Application</span></span> | <span data-ttu-id="0ae5c-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ae5c-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ae5c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ae5c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ae5c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ae5c-117">Optional query parameters</span></span>
<span data-ttu-id="0ae5c-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ae5c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae5c-119">Request headers</span></span>
| <span data-ttu-id="0ae5c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0ae5c-120">Name</span></span>       | <span data-ttu-id="0ae5c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ae5c-121">Type</span></span> | <span data-ttu-id="0ae5c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ae5c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0ae5c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ae5c-123">Authorization</span></span>  | <span data-ttu-id="0ae5c-124">string</span><span class="sxs-lookup"><span data-stu-id="0ae5c-124">string</span></span>  | <span data-ttu-id="0ae5c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ae5c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae5c-127">Request body</span></span>
<span data-ttu-id="0ae5c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ae5c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ae5c-129">Response</span></span>
<span data-ttu-id="0ae5c-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ae5c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ae5c-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0ae5c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ae5c-132">Request</span></span>
<span data-ttu-id="0ae5c-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ae5c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ae5c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ae5c-135">C#</span><span class="sxs-lookup"><span data-stu-id="0ae5c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ae5c-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ae5c-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ae5c-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ae5c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0ae5c-138">Java</span><span class="sxs-lookup"><span data-stu-id="0ae5c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photos-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ae5c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ae5c-139">Response</span></span>
<span data-ttu-id="0ae5c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-140">The following is an example of the response.</span></span>
><span data-ttu-id="0ae5c-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0ae5c-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ae5c-142">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
