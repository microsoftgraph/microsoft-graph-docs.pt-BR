---
title: Listar fotos
description: Recuperar uma lista dos objetos profilePhoto.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c7790daade10154732675835d80e212afb610e3d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33614056"
---
# <a name="list-photos"></a><span data-ttu-id="4b689-103">Listar fotos</span><span class="sxs-lookup"><span data-stu-id="4b689-103">List photos</span></span>
<span data-ttu-id="4b689-104">Recuperar uma lista dos objetos [profilePhoto](../resources/profilephoto.md).</span><span class="sxs-lookup"><span data-stu-id="4b689-104">Retrieve a list of [profilePhoto](../resources/profilephoto.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b689-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b689-105">Permissions</span></span>
<span data-ttu-id="4b689-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b689-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b689-108">Permission type</span></span>      | <span data-ttu-id="4b689-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b689-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b689-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b689-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b689-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b689-111">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="4b689-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b689-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b689-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b689-113">Not supported.</span></span>    |
|<span data-ttu-id="4b689-114">Application</span><span class="sxs-lookup"><span data-stu-id="4b689-114">Application</span></span> | <span data-ttu-id="4b689-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b689-115">Group.ReadBasic.All, Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b689-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b689-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/photos
GET /users/{id | userPrincipalName}/joinedGroups/{id}/photos
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4b689-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4b689-117">Optional query parameters</span></span>
<span data-ttu-id="4b689-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4b689-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b689-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b689-119">Request headers</span></span>
| <span data-ttu-id="4b689-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4b689-120">Name</span></span>       | <span data-ttu-id="4b689-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b689-121">Type</span></span> | <span data-ttu-id="4b689-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b689-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4b689-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b689-123">Authorization</span></span>  | <span data-ttu-id="4b689-124">string</span><span class="sxs-lookup"><span data-stu-id="4b689-124">string</span></span>  | <span data-ttu-id="4b689-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b689-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b689-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b689-127">Request body</span></span>
<span data-ttu-id="4b689-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b689-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b689-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b689-129">Response</span></span>
<span data-ttu-id="4b689-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [profilePhoto](../resources/profilephoto.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b689-130">If successful, this method returns a `200 OK` response code and collection of [profilePhoto](../resources/profilephoto.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b689-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b689-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4b689-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b689-132">Request</span></span>
<span data-ttu-id="4b689-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b689-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photos"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/photos
```

#### <a name="response"></a><span data-ttu-id="4b689-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b689-134">Response</span></span>
<span data-ttu-id="4b689-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4b689-135">The following is an example of the response.</span></span>
><span data-ttu-id="4b689-136">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4b689-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4b689-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b689-137">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4b689-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4b689-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4b689-139">Basic</span><span class="sxs-lookup"><span data-stu-id="4b689-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photos-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b689-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b689-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photos-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List photos",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-photos.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
