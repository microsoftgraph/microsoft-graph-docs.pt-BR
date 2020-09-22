---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Alterar permissões de compartilhamento
localization_priority: Normal
description: Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 59fe051abe8389808b6a66f01108b647ab620aae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020717"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="f09ef-103">Atualizar a permissão de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="f09ef-103">Update sharing permission</span></span>

<span data-ttu-id="f09ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f09ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f09ef-105">Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.</span><span class="sxs-lookup"><span data-stu-id="f09ef-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="f09ef-106">Somente a propriedade **roles** pode ser modificada dessa forma.</span><span class="sxs-lookup"><span data-stu-id="f09ef-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="f09ef-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f09ef-107">Permissions</span></span>

<span data-ttu-id="f09ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f09ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f09ef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f09ef-110">Permission type</span></span>      | <span data-ttu-id="f09ef-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f09ef-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f09ef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f09ef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f09ef-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f09ef-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f09ef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f09ef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f09ef-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f09ef-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f09ef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f09ef-116">Application</span></span> | <span data-ttu-id="f09ef-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f09ef-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f09ef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f09ef-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="f09ef-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="f09ef-119">Optional request headers</span></span>

| <span data-ttu-id="f09ef-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f09ef-120">Name</span></span>          | <span data-ttu-id="f09ef-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f09ef-121">Type</span></span>   | <span data-ttu-id="f09ef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f09ef-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f09ef-123">if-match</span><span class="sxs-lookup"><span data-stu-id="f09ef-123">if-match</span></span>      | <span data-ttu-id="f09ef-124">string</span><span class="sxs-lookup"><span data-stu-id="f09ef-124">string</span></span> | <span data-ttu-id="f09ef-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="f09ef-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f09ef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f09ef-126">Request body</span></span>

<span data-ttu-id="f09ef-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f09ef-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="f09ef-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f09ef-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="f09ef-129">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f09ef-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f09ef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f09ef-130">Property</span></span> | <span data-ttu-id="f09ef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f09ef-131">Type</span></span>              | <span data-ttu-id="f09ef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f09ef-132">Description</span></span>                   |
|:---------|:------------------|:------------------------------|
| <span data-ttu-id="f09ef-133">funções</span><span class="sxs-lookup"><span data-stu-id="f09ef-133">roles</span></span>    | <span data-ttu-id="f09ef-134">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f09ef-134">String collection</span></span> | <span data-ttu-id="f09ef-135">Uma matriz de tipos de permissão.</span><span class="sxs-lookup"><span data-stu-id="f09ef-135">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="f09ef-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f09ef-136">Response</span></span>

<span data-ttu-id="f09ef-137">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [permission](../resources/permission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f09ef-137">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f09ef-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f09ef-138">Example</span></span>

<span data-ttu-id="f09ef-139">Aqui está um exemplo da solicitação que altera a função da permissão de compartilhamento para somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f09ef-139">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="http"></a>[<span data-ttu-id="f09ef-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f09ef-140">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="c"></a>[<span data-ttu-id="f09ef-141">C#</span><span class="sxs-lookup"><span data-stu-id="f09ef-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f09ef-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f09ef-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f09ef-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f09ef-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f09ef-144">Java</span><span class="sxs-lookup"><span data-stu-id="f09ef-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f09ef-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f09ef-145">Response</span></span>

<span data-ttu-id="f09ef-146">Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) no corpo da resposta que representa o estado atualizado da permissão.</span><span class="sxs-lookup"><span data-stu-id="f09ef-146">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="f09ef-147">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="f09ef-147">Error responses</span></span>

<span data-ttu-id="f09ef-148">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="f09ef-148">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission",
  "suppressions": [
  ]
} -->

