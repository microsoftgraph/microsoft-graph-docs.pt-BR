---
title: Restaurar item excluído
description: 'Restaura um item recentemente excluído de itens excluídos. '
author: lleonard-msft
ms.openlocfilehash: 3a78d2d481fb26c6c6b56770375d4ce23f007bd5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301313"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="77107-103">Restaurar item excluído</span><span class="sxs-lookup"><span data-stu-id="77107-103">Restore deleted item</span></span>

<span data-ttu-id="77107-104">Restaura um item recentemente excluído de [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="77107-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="77107-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="77107-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="77107-106">Se um item foi excluído acidentalmente, você poderá restaurá-lo totalmente.</span><span class="sxs-lookup"><span data-stu-id="77107-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="77107-107">Um item recentemente excluído permanecerá disponível por até 30 dias.</span><span class="sxs-lookup"><span data-stu-id="77107-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="77107-108">Após 30 dias, esse item será excluído permanentemente.</span><span class="sxs-lookup"><span data-stu-id="77107-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="77107-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="77107-109">Permissions</span></span>
<span data-ttu-id="77107-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77107-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="77107-112">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="77107-112">For users:</span></span>

|<span data-ttu-id="77107-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77107-113">Permission type</span></span>      | <span data-ttu-id="77107-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77107-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77107-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77107-115">Delegated (work or school account)</span></span> | <span data-ttu-id="77107-116">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77107-116">User.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="77107-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77107-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77107-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77107-118">Not supported.</span></span> |
|<span data-ttu-id="77107-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77107-119">Application</span></span> | <span data-ttu-id="77107-120">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77107-120">User.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="77107-121">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="77107-121">For groups:</span></span>

|<span data-ttu-id="77107-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77107-122">Permission type</span></span>      | <span data-ttu-id="77107-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77107-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77107-124">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77107-124">Delegated (work or school account)</span></span> | <span data-ttu-id="77107-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77107-125">Group.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="77107-126">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77107-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77107-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77107-127">Not supported.</span></span>    |
|<span data-ttu-id="77107-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77107-128">Application</span></span> | <span data-ttu-id="77107-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77107-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77107-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77107-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deletedItems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="77107-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77107-131">Request headers</span></span>
| <span data-ttu-id="77107-132">Nome</span><span class="sxs-lookup"><span data-stu-id="77107-132">Name</span></span>       | <span data-ttu-id="77107-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="77107-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="77107-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="77107-134">Authorization</span></span>  | <span data-ttu-id="77107-135">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="77107-135">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="77107-136">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77107-136">Accept</span></span> | <span data-ttu-id="77107-137">application/json</span><span class="sxs-lookup"><span data-stu-id="77107-137">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="77107-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77107-138">Request body</span></span>
<span data-ttu-id="77107-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77107-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77107-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="77107-140">Response</span></span>

<span data-ttu-id="77107-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77107-141">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77107-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77107-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77107-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77107-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}/restore
```
<span data-ttu-id="77107-144">No corpo da solicitação, forneça uma representação JSON do objeto [directoryObject](../resources/directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="77107-144">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="77107-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="77107-145">Response</span></span>
<span data-ttu-id="77107-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77107-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
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