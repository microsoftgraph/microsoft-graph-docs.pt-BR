---
author: JeremyKelley
description: Retornar a permissão de compartilhamento eficaz de um recurso de permissão específico.
ms.date: 09/10/2017
title: Obter permissão
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 2613eb4e260d3ead63d2619f15ca43521744aec5
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151647"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="46807-103">Obter permissão de compartilhamento para um arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="46807-103">Get sharing permission for a file or folder</span></span>

<span data-ttu-id="46807-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46807-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46807-105">Retornar a permissão de compartilhamento eficaz de um recurso de permissão específico.</span><span class="sxs-lookup"><span data-stu-id="46807-105">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="46807-106">Permissões efetivas de um item podem vir de duas fontes: permissões definidas diretamente no próprio item, ou permissões herdadas de ancestrais do item.</span><span class="sxs-lookup"><span data-stu-id="46807-106">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="46807-p101">Os chamadores podem diferenciar se a permissão é herdada ou não verificando a propriedade `inheritedFrom` Esta propriedade é um recurso [itemReference](../resources/itemreference.md) que faz referência ao ancestral do qual a permissão é herdada.</span><span class="sxs-lookup"><span data-stu-id="46807-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

## <a name="permissions"></a><span data-ttu-id="46807-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="46807-109">Permissions</span></span>

<span data-ttu-id="46807-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46807-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46807-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46807-112">Permission type</span></span>      | <span data-ttu-id="46807-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46807-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46807-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46807-114">Delegated (work or school account)</span></span> | <span data-ttu-id="46807-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46807-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="46807-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46807-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46807-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46807-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="46807-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46807-118">Application</span></span> | <span data-ttu-id="46807-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46807-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46807-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46807-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46807-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46807-121">Optional query parameters</span></span>

<span data-ttu-id="46807-122">Esse método é compatível com o [parâmetro de consulta $select](/graph/query-parameters) para formar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46807-122">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="46807-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="46807-123">Response</span></span>

<span data-ttu-id="46807-124">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [Permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46807-124">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46807-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46807-125">Example</span></span>

### <a name="request"></a><span data-ttu-id="46807-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46807-126">Request</span></span>

<span data-ttu-id="46807-127">Aqui está um exemplo da solicitação para acessar uma permissão em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="46807-127">Here is an example of the request to access a permission on a folder.</span></span>


# <a name="http"></a>[<span data-ttu-id="46807-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="46807-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="46807-129">C#</span><span class="sxs-lookup"><span data-stu-id="46807-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46807-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46807-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46807-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46807-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46807-132">Java</span><span class="sxs-lookup"><span data-stu-id="46807-132">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="46807-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46807-133">Response</span></span>

<span data-ttu-id="46807-134">Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) para a ID especificada.</span><span class="sxs-lookup"><span data-stu-id="46807-134">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="46807-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="46807-135">Remarks</span></span>

<span data-ttu-id="46807-136">O recurso [Permission](../resources/permission.md) usa _facets_ para fornecer informações sobre o tipo de permissão representado pelo recurso.</span><span class="sxs-lookup"><span data-stu-id="46807-136">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="46807-p103">Permissões com uma faceta [**link**](../resources/sharinglink.md) representam links de compartilhamento criados no item. Os links de compartilhamento contêm um token exclusivo que fornece acesso ao item para qualquer pessoa com o link.</span><span class="sxs-lookup"><span data-stu-id="46807-p103">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="46807-139">Permissões com uma faceta [**invitation**](../resources/sharinginvitation.md) representam permissões adicionadas convidando usuários ou grupos específicos para ter acesso ao arquivo.</span><span class="sxs-lookup"><span data-stu-id="46807-139">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get permission",
  "suppressions": [
  ]
}
-->
