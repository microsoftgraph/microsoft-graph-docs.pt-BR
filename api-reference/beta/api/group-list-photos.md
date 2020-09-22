---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2c462ae486d528f6d3084e714af890777380d8e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990918"
---
# <a name="list-photos"></a><span data-ttu-id="97ea3-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="97ea3-103">List photos</span></span>

<span data-ttu-id="97ea3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97ea3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97ea3-105">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="97ea3-105">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="97ea3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="97ea3-106">Permissions</span></span>
<span data-ttu-id="97ea3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97ea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97ea3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97ea3-109">Permission type</span></span>      | <span data-ttu-id="97ea3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97ea3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97ea3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97ea3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="97ea3-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97ea3-112">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="97ea3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97ea3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97ea3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97ea3-114">Not supported.</span></span>    |
|<span data-ttu-id="97ea3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97ea3-115">Application</span></span> | <span data-ttu-id="97ea3-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97ea3-116">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="97ea3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97ea3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97ea3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97ea3-118">Optional query parameters</span></span>
<span data-ttu-id="97ea3-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="97ea3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97ea3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97ea3-120">Request headers</span></span>
| <span data-ttu-id="97ea3-121">Nome</span><span class="sxs-lookup"><span data-stu-id="97ea3-121">Name</span></span>       | <span data-ttu-id="97ea3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="97ea3-122">Type</span></span> | <span data-ttu-id="97ea3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="97ea3-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97ea3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="97ea3-124">Authorization</span></span>  | <span data-ttu-id="97ea3-125">string</span><span class="sxs-lookup"><span data-stu-id="97ea3-125">string</span></span>  | <span data-ttu-id="97ea3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97ea3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97ea3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97ea3-128">Request body</span></span>
<span data-ttu-id="97ea3-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97ea3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97ea3-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="97ea3-130">Response</span></span>
<span data-ttu-id="97ea3-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97ea3-131">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97ea3-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97ea3-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="97ea3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97ea3-133">Request</span></span>
<span data-ttu-id="97ea3-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97ea3-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97ea3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="97ea3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/photos
```
# <a name="c"></a>[<span data-ttu-id="97ea3-136">C#</span><span class="sxs-lookup"><span data-stu-id="97ea3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photos-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97ea3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97ea3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photos-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97ea3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97ea3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photos-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="97ea3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="97ea3-139">Response</span></span>
<span data-ttu-id="97ea3-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97ea3-140">The following is an example of the response.</span></span>
><span data-ttu-id="97ea3-141">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="97ea3-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="97ea3-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97ea3-142">All the properties will be returned from an actual call.</span></span>
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


