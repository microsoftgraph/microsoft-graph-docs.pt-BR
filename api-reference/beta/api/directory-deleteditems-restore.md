---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8462004fb515598c2469df95b19c71c39fc457e5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417531"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="6d857-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="6d857-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d857-104">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="6d857-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="6d857-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="6d857-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="6d857-106">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="6d857-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="6d857-107">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="6d857-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="6d857-108">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="6d857-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d857-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d857-109">Permissions</span></span>
<span data-ttu-id="6d857-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d857-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="6d857-112">Para usuários: user. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6d857-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="6d857-113">Para grupos: Group. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="6d857-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="6d857-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d857-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="6d857-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d857-115">Request headers</span></span>
| <span data-ttu-id="6d857-116">Nome</span><span class="sxs-lookup"><span data-stu-id="6d857-116">Name</span></span>       | <span data-ttu-id="6d857-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d857-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6d857-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d857-118">Authorization</span></span>  | <span data-ttu-id="6d857-119">&lt;Token&gt; de portador *necessário*</span><span class="sxs-lookup"><span data-stu-id="6d857-119">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="6d857-120">Content-type</span><span class="sxs-lookup"><span data-stu-id="6d857-120">Content-type</span></span> | <span data-ttu-id="6d857-121">application/json</span><span class="sxs-lookup"><span data-stu-id="6d857-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d857-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d857-122">Request body</span></span>
<span data-ttu-id="6d857-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d857-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d857-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d857-124">Response</span></span>

<span data-ttu-id="6d857-125">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d857-125">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d857-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d857-126">Example</span></span>
### <a name="request"></a><span data-ttu-id="6d857-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d857-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6d857-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d857-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d857-129">C#</span><span class="sxs-lookup"><span data-stu-id="6d857-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d857-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d857-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d857-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6d857-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6d857-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d857-132">Response</span></span>
<span data-ttu-id="6d857-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d857-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
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
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
