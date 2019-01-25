---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 42af211afb9f508e9033f3e77f2b1dd14aa484d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520729"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="4150e-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="4150e-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4150e-104">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="4150e-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="4150e-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="4150e-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="4150e-106">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="4150e-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="4150e-107">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="4150e-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="4150e-108">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="4150e-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="4150e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4150e-109">Permissions</span></span>
<span data-ttu-id="4150e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4150e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="4150e-112">Para usuários: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4150e-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="4150e-113">Para grupos: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4150e-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4150e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4150e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="4150e-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4150e-115">Request headers</span></span>
| <span data-ttu-id="4150e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="4150e-116">Name</span></span>       | <span data-ttu-id="4150e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="4150e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4150e-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="4150e-118">Authorization</span></span>  | <span data-ttu-id="4150e-119">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="4150e-119">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="4150e-120">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4150e-120">Accept</span></span> | <span data-ttu-id="4150e-121">application/json</span><span class="sxs-lookup"><span data-stu-id="4150e-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4150e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4150e-122">Request body</span></span>
<span data-ttu-id="4150e-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4150e-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4150e-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="4150e-124">Response</span></span>

<span data-ttu-id="4150e-125">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4150e-125">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4150e-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4150e-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4150e-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4150e-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="4150e-128">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="4150e-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4150e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4150e-129">Response</span></span>
<span data-ttu-id="4150e-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4150e-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
