---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: lleonard-msft
ms.openlocfilehash: 0088daf7f84217ca921a1e3e80243d7002b5f6b6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356536"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="f2a20-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="f2a20-103">Restore deleted item</span></span>

> <span data-ttu-id="f2a20-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2a20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2a20-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2a20-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2a20-106">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="f2a20-106">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="f2a20-107">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="f2a20-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="f2a20-108">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="f2a20-108">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="f2a20-109">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="f2a20-109">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="f2a20-110">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="f2a20-110">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2a20-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="f2a20-111">Permissions</span></span>
<span data-ttu-id="f2a20-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2a20-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f2a20-114">Para usuários: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2a20-114">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="f2a20-115">Para grupos: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2a20-115">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f2a20-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2a20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="f2a20-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a20-117">Request headers</span></span>
| <span data-ttu-id="f2a20-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f2a20-118">Name</span></span>       | <span data-ttu-id="f2a20-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2a20-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f2a20-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2a20-120">Authorization</span></span>  | <span data-ttu-id="f2a20-121">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="f2a20-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f2a20-122">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2a20-122">Accept</span></span> | <span data-ttu-id="f2a20-123">application/json</span><span class="sxs-lookup"><span data-stu-id="f2a20-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2a20-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a20-124">Request body</span></span>
<span data-ttu-id="f2a20-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2a20-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2a20-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a20-126">Response</span></span>

<span data-ttu-id="f2a20-127">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2a20-127">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2a20-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2a20-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2a20-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2a20-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="f2a20-130">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="f2a20-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f2a20-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2a20-131">Response</span></span>
<span data-ttu-id="f2a20-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2a20-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->