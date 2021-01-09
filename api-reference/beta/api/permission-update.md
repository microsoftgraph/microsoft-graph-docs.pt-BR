---
author: JeremyKelley
description: Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.
ms.date: 09/10/2017
title: Alterar permissões de compartilhamento
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 56f9d600a36fb7b94757e6c783e2d397306e2de0
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790682"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="77768-103">Atualizar a permissão de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="77768-103">Update sharing permission</span></span>

<span data-ttu-id="77768-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77768-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77768-105">Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.</span><span class="sxs-lookup"><span data-stu-id="77768-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="77768-106">Somente a propriedade **roles** pode ser modificada dessa forma.</span><span class="sxs-lookup"><span data-stu-id="77768-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="77768-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="77768-107">Permissions</span></span>

<span data-ttu-id="77768-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77768-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77768-110">Permission type</span></span>      | <span data-ttu-id="77768-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77768-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77768-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77768-112">Delegated (work or school account)</span></span> | <span data-ttu-id="77768-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77768-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="77768-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77768-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77768-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77768-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="77768-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77768-116">Application</span></span> | <span data-ttu-id="77768-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77768-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77768-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77768-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="77768-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="77768-119">Optional request headers</span></span>

| <span data-ttu-id="77768-120">Nome</span><span class="sxs-lookup"><span data-stu-id="77768-120">Name</span></span>          | <span data-ttu-id="77768-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="77768-121">Type</span></span>   | <span data-ttu-id="77768-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="77768-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="77768-123">if-match</span><span class="sxs-lookup"><span data-stu-id="77768-123">if-match</span></span>      | <span data-ttu-id="77768-124">string</span><span class="sxs-lookup"><span data-stu-id="77768-124">string</span></span> | <span data-ttu-id="77768-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="77768-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77768-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77768-126">Request body</span></span>

<span data-ttu-id="77768-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="77768-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="77768-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="77768-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="77768-129">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="77768-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="77768-130">As propriedades a seguir nesses tipos de permissão podem ser modificadas.</span><span class="sxs-lookup"><span data-stu-id="77768-130">The following properties on these permission types can be modified.</span></span>

| <span data-ttu-id="77768-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77768-131">Permission Type</span></span>        | <span data-ttu-id="77768-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77768-132">Property</span></span> | <span data-ttu-id="77768-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="77768-133">Type</span></span>              | <span data-ttu-id="77768-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="77768-134">Description</span></span>                   |
|:-----------------------|:---------|:------------------|:------------------------------|
| <span data-ttu-id="77768-135">Usuário</span><span class="sxs-lookup"><span data-stu-id="77768-135">User</span></span>                   | <span data-ttu-id="77768-136">funções</span><span class="sxs-lookup"><span data-stu-id="77768-136">roles</span></span>    | <span data-ttu-id="77768-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="77768-137">String collection</span></span> | <span data-ttu-id="77768-138">Uma matriz de tipos de permissão.</span><span class="sxs-lookup"><span data-stu-id="77768-138">An array of permission types.</span></span> |
| <span data-ttu-id="77768-139">Link de compartilhamento anônimo</span><span class="sxs-lookup"><span data-stu-id="77768-139">Anonymous Sharing Link</span></span> | <span data-ttu-id="77768-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="77768-140">expirationDateTime</span></span> | <span data-ttu-id="77768-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77768-141">DateTimeOffset</span></span> | <span data-ttu-id="77768-142">Um formato de yyyy-MM-ddTHH:mm:ssZ de DateTimeOffset para o tempo de expiração da permissão.</span><span class="sxs-lookup"><span data-stu-id="77768-142">A format of yyyy-MM-ddTHH:mm:ssZ of DateTimeOffset for the expiration time of the permission.</span></span> |

### <a name="remarks"></a><span data-ttu-id="77768-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="77768-143">Remarks</span></span>
<span data-ttu-id="77768-144">As modificações de permissão sem suporte incluem o seguinte:</span><span class="sxs-lookup"><span data-stu-id="77768-144">Unsupported permission modifications include the following:</span></span>
- <span data-ttu-id="77768-145">Links de compartilhamento organizacional</span><span class="sxs-lookup"><span data-stu-id="77768-145">Organizational sharing links</span></span>
- <span data-ttu-id="77768-146">Links de compartilhamento de pessoas</span><span class="sxs-lookup"><span data-stu-id="77768-146">People sharing links</span></span>

## <a name="response"></a><span data-ttu-id="77768-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="77768-147">Response</span></span>

<span data-ttu-id="77768-148">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [permission](../resources/permission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77768-148">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77768-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77768-149">Example</span></span>

<span data-ttu-id="77768-150">Aqui está um exemplo da solicitação que altera a função da permissão de compartilhamento para somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77768-150">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="http"></a>[<span data-ttu-id="77768-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="77768-151">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="c"></a>[<span data-ttu-id="77768-152">C#</span><span class="sxs-lookup"><span data-stu-id="77768-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="77768-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77768-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77768-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77768-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="77768-155">Java</span><span class="sxs-lookup"><span data-stu-id="77768-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77768-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="77768-156">Response</span></span>

<span data-ttu-id="77768-157">Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) no corpo da resposta que representa o estado atualizado da permissão.</span><span class="sxs-lookup"><span data-stu-id="77768-157">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true } -->

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
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission",
  "suppressions": [
  ]
}
-->


