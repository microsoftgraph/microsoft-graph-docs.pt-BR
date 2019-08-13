---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 783b9d798803258fa804567ddb93fda0230499a2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319591"
---
# <a name="list-deleted-items"></a><span data-ttu-id="c107d-103">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="c107d-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c107d-104">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="c107d-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="c107d-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="c107d-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="c107d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c107d-106">Permissions</span></span>
<span data-ttu-id="c107d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c107d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="c107d-109">Para usuários: user. Read. All, Directory. Read. All, User. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c107d-109">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="c107d-110">Para grupos: Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="c107d-110">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="c107d-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c107d-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="c107d-112">Essa API dá suporte atualmente à recuperação de tipos de objeto de grupos (microsoft.graph.group) ou usuários (microsoft.graph.user) de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="c107d-112">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="c107d-113">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="c107d-113">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="c107d-114">Não há suporte para a chamada de GET /directory/deleteditems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="c107d-114">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c107d-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c107d-115">Optional query parameters</span></span>
<span data-ttu-id="c107d-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c107d-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c107d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c107d-117">Request headers</span></span>
| <span data-ttu-id="c107d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c107d-118">Name</span></span>      |<span data-ttu-id="c107d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c107d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c107d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c107d-120">Authorization</span></span>  | <span data-ttu-id="c107d-121">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="c107d-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="c107d-122">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c107d-122">Accept</span></span>  | <span data-ttu-id="c107d-123">application/json</span><span class="sxs-lookup"><span data-stu-id="c107d-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c107d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c107d-124">Request body</span></span>
<span data-ttu-id="c107d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c107d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c107d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c107d-126">Response</span></span>

<span data-ttu-id="c107d-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c107d-127">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c107d-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c107d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c107d-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c107d-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c107d-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c107d-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c107d-131">C#</span><span class="sxs-lookup"><span data-stu-id="c107d-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c107d-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c107d-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c107d-133">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c107d-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c107d-134">Java</span><span class="sxs-lookup"><span data-stu-id="c107d-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c107d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c107d-135">Response</span></span>
<span data-ttu-id="c107d-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c107d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
