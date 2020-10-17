---
title: 'permissão: revokeGrants'
description: Atualizar as permissões de compartilhamento de um item
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a6ac5f1aacc068ef092f3881d67f6c121d84b400
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582363"
---
# <a name="permission-revokegrants"></a><span data-ttu-id="e61b8-103">permissão: revokeGrants</span><span class="sxs-lookup"><span data-stu-id="e61b8-103">permission: revokeGrants</span></span>
<span data-ttu-id="e61b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e61b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e61b8-105">Revogar o acesso a um [ListItem][] ou [driveItem][] concedido por meio de um link de compartilhamento removendo o [destinatário][] especificado do link.</span><span class="sxs-lookup"><span data-stu-id="e61b8-105">Revoke access to a [listItem][] or [driveItem][] granted via a sharing link by removing the specified [recipient][] from the link.</span></span>

><span data-ttu-id="e61b8-106">**Observação:** Essa funcionalidade só está disponível para compartilhar links com escopo para os usuários.</span><span class="sxs-lookup"><span data-stu-id="e61b8-106">**Note:** This functionality is only available for sharing links scoped to users.</span></span>

[listItem]: ../resources/listitem.md
[driveItem]: ../resources/driveitem.md
[recipient]: ../resources/driverecipient.md

## <a name="permissions"></a><span data-ttu-id="e61b8-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="e61b8-110">Permissions</span></span>
<span data-ttu-id="e61b8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e61b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e61b8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e61b8-113">Permission type</span></span>|<span data-ttu-id="e61b8-114">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e61b8-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e61b8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e61b8-115">Delegated (work or school account)</span></span>|<span data-ttu-id="e61b8-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e61b8-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>|
|<span data-ttu-id="e61b8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e61b8-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e61b8-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e61b8-118">Not supported</span></span>|
|<span data-ttu-id="e61b8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e61b8-119">Application</span></span>|<span data-ttu-id="e61b8-120">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e61b8-120">Files.ReadWrite.All, Sites.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e61b8-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e61b8-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drive-id}/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/lists/{list-id}/items/{listItem-id}/permissions/{perm-id}/revokeGrants
POST /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
```

## <a name="request-headers"></a><span data-ttu-id="e61b8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e61b8-122">Request headers</span></span>
|<span data-ttu-id="e61b8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e61b8-123">Name</span></span>|<span data-ttu-id="e61b8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e61b8-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e61b8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e61b8-125">Authorization</span></span>|<span data-ttu-id="e61b8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e61b8-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e61b8-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e61b8-128">Content-Type</span></span>|<span data-ttu-id="e61b8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e61b8-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e61b8-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e61b8-131">Request body</span></span>
<span data-ttu-id="e61b8-132">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e61b8-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="e61b8-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="e61b8-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="e61b8-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e61b8-134">Parameter</span></span>|<span data-ttu-id="e61b8-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="e61b8-135">Type</span></span>|<span data-ttu-id="e61b8-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="e61b8-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e61b8-137">granters</span><span class="sxs-lookup"><span data-stu-id="e61b8-137">grantees</span></span>|<span data-ttu-id="e61b8-138">coleção [driveRecipient](../resources/driverecipient.md)</span><span class="sxs-lookup"><span data-stu-id="e61b8-138">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="e61b8-139">Uma coleção de destinatários que serão revogados de acesso ao link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="e61b8-139">A collection of recipients who will be revoked access to the sharing link.</span></span>|

## <a name="response"></a><span data-ttu-id="e61b8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e61b8-140">Response</span></span>

<span data-ttu-id="e61b8-141">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e uma [permissão](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e61b8-141">If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e61b8-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e61b8-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e61b8-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e61b8-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "permission-revokegrants"
}
-->
``` http
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants

Content-Type: application/json
Content-length: 95

{
  "grantees": [
    {
      "email": "ryan@contoso.com"
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="e61b8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e61b8-144">Response</span></span>

<span data-ttu-id="e61b8-145">Se tiver êxito, este método retornará um recurso [Permission](../resources/permission.md) no corpo da resposta que representa o estado atualizado do link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="e61b8-145">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the sharing link.</span></span>

><span data-ttu-id="e61b8-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e61b8-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "users",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission"
} -->
