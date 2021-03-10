---
title: 'permission: revokeGrants'
description: Atualizar permissões de compartilhamento de um item
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 8a60aa04b999009ad279b0715ed97cbc045e268a
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625499"
---
# <a name="permission-revokegrants"></a><span data-ttu-id="88db6-103">permission: revokeGrants</span><span class="sxs-lookup"><span data-stu-id="88db6-103">permission: revokeGrants</span></span>
<span data-ttu-id="88db6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88db6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88db6-105">Revogar o acesso a [um listItem][] ou [driveItem][] concedido por meio de um link de compartilhamento removendo o [destinatário][] especificado do link.</span><span class="sxs-lookup"><span data-stu-id="88db6-105">Revoke access to a [listItem][] or [driveItem][] granted via a sharing link by removing the specified [recipient][] from the link.</span></span>

><span data-ttu-id="88db6-106">**Observação:** Essa funcionalidade só está disponível para compartilhamento de links com escopo para usuários.</span><span class="sxs-lookup"><span data-stu-id="88db6-106">**Note:** This functionality is only available for sharing links scoped to users.</span></span>

[listItem]: ../resources/listitem.md
[driveItem]: ../resources/driveitem.md
[recipient]: ../resources/driverecipient.md

## <a name="permissions"></a><span data-ttu-id="88db6-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="88db6-110">Permissions</span></span>
<span data-ttu-id="88db6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88db6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88db6-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="88db6-113">Permission type</span></span>|<span data-ttu-id="88db6-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="88db6-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88db6-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="88db6-115">Delegated (work or school account)</span></span>|<span data-ttu-id="88db6-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88db6-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>|
|<span data-ttu-id="88db6-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="88db6-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88db6-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="88db6-118">Not supported</span></span>|
|<span data-ttu-id="88db6-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="88db6-119">Application</span></span>|<span data-ttu-id="88db6-120">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88db6-120">Files.ReadWrite.All, Sites.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88db6-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="88db6-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /drives/{drive-id}/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /me/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
POST /sites/{site-id}/lists/{list-id}/items/{listItem-id}/driveItem/permissions/{perm-id}/revokeGrants
POST /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}/revokeGrants
```

## <a name="request-headers"></a><span data-ttu-id="88db6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="88db6-122">Request headers</span></span>
|<span data-ttu-id="88db6-123">Nome</span><span class="sxs-lookup"><span data-stu-id="88db6-123">Name</span></span>|<span data-ttu-id="88db6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="88db6-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88db6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="88db6-125">Authorization</span></span>|<span data-ttu-id="88db6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88db6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="88db6-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88db6-128">Content-Type</span></span>|<span data-ttu-id="88db6-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="88db6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88db6-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="88db6-131">Request body</span></span>
<span data-ttu-id="88db6-132">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="88db6-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="88db6-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="88db6-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="88db6-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="88db6-134">Parameter</span></span>|<span data-ttu-id="88db6-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="88db6-135">Type</span></span>|<span data-ttu-id="88db6-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="88db6-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88db6-137">grantees</span><span class="sxs-lookup"><span data-stu-id="88db6-137">grantees</span></span>|<span data-ttu-id="88db6-138">[Coleção driveRecipient](../resources/driverecipient.md)</span><span class="sxs-lookup"><span data-stu-id="88db6-138">[driveRecipient](../resources/driverecipient.md) collection</span></span>|<span data-ttu-id="88db6-139">Uma coleção de destinatários que serão revogados acesso ao link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="88db6-139">A collection of recipients who will be revoked access to the sharing link.</span></span>|

## <a name="response"></a><span data-ttu-id="88db6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="88db6-140">Response</span></span>

<span data-ttu-id="88db6-141">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e uma [permissão](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="88db6-141">If successful, this action returns a `200 OK` response code and a [permission](../resources/permission.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88db6-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="88db6-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88db6-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="88db6-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="88db6-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="88db6-144">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="88db6-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88db6-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-revokegrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="88db6-146">C#</span><span class="sxs-lookup"><span data-stu-id="88db6-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-revokegrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88db6-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88db6-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-revokegrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88db6-148">Java</span><span class="sxs-lookup"><span data-stu-id="88db6-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-revokegrants-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="88db6-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="88db6-149">Response</span></span>

<span data-ttu-id="88db6-150">Se tiver êxito, este método retornará [um recurso Permission](../resources/permission.md) no corpo da resposta que representa o estado atualizado do link de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="88db6-150">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the sharing link.</span></span>

><span data-ttu-id="88db6-151">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="88db6-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
