---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 170de24c41e6e2edee43d43e822ab67270b61f22
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260855"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="2ed99-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="2ed99-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ed99-104">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="2ed99-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="2ed99-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2ed99-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="2ed99-106">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="2ed99-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="2ed99-107">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="2ed99-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="2ed99-108">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="2ed99-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ed99-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ed99-109">Permissions</span></span>
<span data-ttu-id="2ed99-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ed99-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="2ed99-112">Para usuários: user. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="2ed99-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="2ed99-113">Para grupos: Group. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="2ed99-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="2ed99-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ed99-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="2ed99-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed99-115">Request headers</span></span>
| <span data-ttu-id="2ed99-116">Nome</span><span class="sxs-lookup"><span data-stu-id="2ed99-116">Name</span></span>       | <span data-ttu-id="2ed99-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ed99-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ed99-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ed99-118">Authorization</span></span>  | <span data-ttu-id="2ed99-119">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="2ed99-119">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="2ed99-120">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2ed99-120">Accept</span></span> | <span data-ttu-id="2ed99-121">application/json</span><span class="sxs-lookup"><span data-stu-id="2ed99-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ed99-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed99-122">Request body</span></span>
<span data-ttu-id="2ed99-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ed99-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ed99-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ed99-124">Response</span></span>

<span data-ttu-id="2ed99-125">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ed99-125">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ed99-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ed99-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ed99-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ed99-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="2ed99-128">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="2ed99-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2ed99-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ed99-129">Response</span></span>
<span data-ttu-id="2ed99-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ed99-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2ed99-132">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="2ed99-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2ed99-133">C#</span><span class="sxs-lookup"><span data-stu-id="2ed99-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ed99-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ed99-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="2ed99-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2ed99-135">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
