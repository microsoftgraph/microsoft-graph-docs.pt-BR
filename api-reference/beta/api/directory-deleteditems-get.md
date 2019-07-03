---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00afcc8312e0272611cda3f8526214593fe8bb6d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437134"
---
# <a name="get-deleted-item"></a><span data-ttu-id="12ca6-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="12ca6-103">Get deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12ca6-104">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="12ca6-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="12ca6-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="12ca6-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="12ca6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12ca6-106">Permissions</span></span>
<span data-ttu-id="12ca6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12ca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="12ca6-109">Para usuários: user. Read. All, User. ReadWrite. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="12ca6-109">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="12ca6-110">Para grupos: Group. Read. All, Group. ReadWrite. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="12ca6-110">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="12ca6-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12ca6-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12ca6-112">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12ca6-112">Optional query parameters</span></span>
<span data-ttu-id="12ca6-113">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="12ca6-113">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12ca6-114">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12ca6-114">Request headers</span></span>
| <span data-ttu-id="12ca6-115">Nome</span><span class="sxs-lookup"><span data-stu-id="12ca6-115">Name</span></span>      |<span data-ttu-id="12ca6-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="12ca6-116">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="12ca6-117">Autorização</span><span class="sxs-lookup"><span data-stu-id="12ca6-117">Authorization</span></span>  | <span data-ttu-id="12ca6-118">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="12ca6-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="12ca6-119">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12ca6-119">Accept</span></span>  | <span data-ttu-id="12ca6-120">application/json</span><span class="sxs-lookup"><span data-stu-id="12ca6-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="12ca6-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12ca6-121">Request body</span></span>
<span data-ttu-id="12ca6-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12ca6-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12ca6-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ca6-123">Response</span></span>

<span data-ttu-id="12ca6-124">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12ca6-124">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12ca6-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12ca6-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12ca6-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12ca6-126">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="12ca6-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="12ca6-127">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="12ca6-128">C#</span><span class="sxs-lookup"><span data-stu-id="12ca6-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12ca6-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="12ca6-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="12ca6-130">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="12ca6-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="12ca6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ca6-131">Response</span></span>
<span data-ttu-id="12ca6-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12ca6-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
