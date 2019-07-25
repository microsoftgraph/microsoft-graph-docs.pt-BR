---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 4eee35fa0a991681f07d35d5540bcc76c4ecbba0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858286"
---
# <a name="list-photos"></a><span data-ttu-id="34df0-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="34df0-103">List photos</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34df0-104">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="34df0-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="34df0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="34df0-105">Permissions</span></span>
<span data-ttu-id="34df0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34df0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34df0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34df0-108">Permission type</span></span>      | <span data-ttu-id="34df0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34df0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34df0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34df0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="34df0-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34df0-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="34df0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34df0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34df0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34df0-113">Not supported.</span></span>    |
|<span data-ttu-id="34df0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34df0-114">Application</span></span> | <span data-ttu-id="34df0-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34df0-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34df0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34df0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34df0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34df0-117">Optional query parameters</span></span>
<span data-ttu-id="34df0-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="34df0-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="34df0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34df0-119">Request headers</span></span>
| <span data-ttu-id="34df0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="34df0-120">Name</span></span>       | <span data-ttu-id="34df0-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="34df0-121">Type</span></span> | <span data-ttu-id="34df0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="34df0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="34df0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="34df0-123">Authorization</span></span>  | <span data-ttu-id="34df0-124">string</span><span class="sxs-lookup"><span data-stu-id="34df0-124">string</span></span>  | <span data-ttu-id="34df0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34df0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="34df0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34df0-127">Request body</span></span>
<span data-ttu-id="34df0-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34df0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34df0-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34df0-129">Response</span></span>
<span data-ttu-id="34df0-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34df0-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34df0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34df0-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="34df0-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34df0-132">Request</span></span>
<span data-ttu-id="34df0-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34df0-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="34df0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="34df0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="34df0-135">C#</span><span class="sxs-lookup"><span data-stu-id="34df0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="34df0-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="34df0-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="34df0-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="34df0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="34df0-138">Java</span><span class="sxs-lookup"><span data-stu-id="34df0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photos-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="34df0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="34df0-139">Response</span></span>
<span data-ttu-id="34df0-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="34df0-140">The following is an example of the response.</span></span>
><span data-ttu-id="34df0-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="34df0-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="34df0-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34df0-142">All the properties will be returned from an actual call.</span></span>
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
