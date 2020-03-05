---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: dacef0feb1e97ad52502b0ad456bbf7cd2c92209
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419363"
---
# <a name="list-photos"></a><span data-ttu-id="53766-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="53766-103">List photos</span></span>

<span data-ttu-id="53766-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="53766-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53766-105">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="53766-105">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="53766-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="53766-106">Permissions</span></span>
<span data-ttu-id="53766-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53766-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53766-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53766-109">Permission type</span></span>      | <span data-ttu-id="53766-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53766-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53766-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53766-111">Delegated (work or school account)</span></span> | <span data-ttu-id="53766-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53766-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="53766-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53766-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53766-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53766-114">Not supported.</span></span>    |
|<span data-ttu-id="53766-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53766-115">Application</span></span> | <span data-ttu-id="53766-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53766-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53766-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53766-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="53766-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="53766-118">Optional query parameters</span></span>
<span data-ttu-id="53766-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="53766-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="53766-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53766-120">Request headers</span></span>
| <span data-ttu-id="53766-121">Nome</span><span class="sxs-lookup"><span data-stu-id="53766-121">Name</span></span>       | <span data-ttu-id="53766-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="53766-122">Type</span></span> | <span data-ttu-id="53766-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="53766-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53766-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="53766-124">Authorization</span></span>  | <span data-ttu-id="53766-125">string</span><span class="sxs-lookup"><span data-stu-id="53766-125">string</span></span>  | <span data-ttu-id="53766-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53766-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53766-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53766-128">Request body</span></span>
<span data-ttu-id="53766-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="53766-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53766-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="53766-130">Response</span></span>
<span data-ttu-id="53766-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53766-131">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53766-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53766-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="53766-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53766-133">Request</span></span>
<span data-ttu-id="53766-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="53766-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="53766-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="53766-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="c"></a>[<span data-ttu-id="53766-136">C#</span><span class="sxs-lookup"><span data-stu-id="53766-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53766-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53766-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53766-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53766-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="53766-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="53766-139">Response</span></span>
<span data-ttu-id="53766-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="53766-140">The following is an example of the response.</span></span>
><span data-ttu-id="53766-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="53766-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="53766-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53766-142">All the properties will be returned from an actual call.</span></span>
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
