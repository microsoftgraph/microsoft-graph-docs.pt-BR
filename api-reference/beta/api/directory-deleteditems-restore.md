---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0c0a7a4e1e3087cf05eef023620eb273a62b9556
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435315"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="dca8c-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="dca8c-103">Restore deleted item</span></span>

<span data-ttu-id="dca8c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dca8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dca8c-105">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="dca8c-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="dca8c-106">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="dca8c-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="dca8c-107">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="dca8c-107">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="dca8c-108">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="dca8c-108">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="dca8c-109">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="dca8c-109">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="dca8c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="dca8c-110">Permissions</span></span>
<span data-ttu-id="dca8c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca8c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="dca8c-113">Para aplicativos: Application. ReadWrite. OwnedBy, Application. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="dca8c-113">For applications: Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="dca8c-114">Para usuários: user. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="dca8c-114">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="dca8c-115">Para grupos: Group. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="dca8c-115">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="dca8c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dca8c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="dca8c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dca8c-117">Request headers</span></span>
| <span data-ttu-id="dca8c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="dca8c-118">Name</span></span>       | <span data-ttu-id="dca8c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="dca8c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dca8c-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dca8c-120">Authorization</span></span>  | <span data-ttu-id="dca8c-121">&lt;Token&gt; de portador *necessário*</span><span class="sxs-lookup"><span data-stu-id="dca8c-121">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="dca8c-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="dca8c-122">Content-type</span></span> | <span data-ttu-id="dca8c-123">application/json</span><span class="sxs-lookup"><span data-stu-id="dca8c-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dca8c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dca8c-124">Request body</span></span>
<span data-ttu-id="dca8c-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dca8c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dca8c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="dca8c-126">Response</span></span>

<span data-ttu-id="dca8c-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dca8c-127">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dca8c-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dca8c-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="dca8c-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dca8c-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dca8c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dca8c-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="c"></a>[<span data-ttu-id="dca8c-131">C#</span><span class="sxs-lookup"><span data-stu-id="dca8c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dca8c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dca8c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dca8c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dca8c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="dca8c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dca8c-134">Response</span></span>
<span data-ttu-id="dca8c-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dca8c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
