---
author: JeremyKelley
description: Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.
ms.date: 09/10/2017
title: Alterar permissões de compartilhamento
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 726f0fc85593d70b37162df94bce3a504b80b6e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349555"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="6b461-103">Atualizar a permissão de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="6b461-103">Update sharing permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b461-104">Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.</span><span class="sxs-lookup"><span data-stu-id="6b461-104">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="6b461-105">Somente a propriedade **roles** pode ser modificada dessa forma.</span><span class="sxs-lookup"><span data-stu-id="6b461-105">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b461-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b461-106">Permissions</span></span>

<span data-ttu-id="6b461-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b461-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b461-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b461-109">Permission type</span></span>      | <span data-ttu-id="6b461-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b461-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b461-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b461-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b461-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b461-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b461-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b461-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b461-114">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b461-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b461-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b461-115">Application</span></span> | <span data-ttu-id="6b461-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b461-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b461-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b461-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="6b461-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="6b461-118">Optional request headers</span></span>

| <span data-ttu-id="6b461-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b461-119">Name</span></span>          | <span data-ttu-id="6b461-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b461-120">Type</span></span>   | <span data-ttu-id="6b461-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b461-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6b461-122">if-match</span><span class="sxs-lookup"><span data-stu-id="6b461-122">if-match</span></span>      | <span data-ttu-id="6b461-123">string</span><span class="sxs-lookup"><span data-stu-id="6b461-123">string</span></span> | <span data-ttu-id="6b461-124">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="6b461-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b461-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b461-125">Request body</span></span>

<span data-ttu-id="6b461-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6b461-126">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="6b461-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="6b461-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="6b461-128">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="6b461-128">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6b461-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b461-129">Property</span></span>     | <span data-ttu-id="6b461-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b461-130">Type</span></span>   | <span data-ttu-id="6b461-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b461-131">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="6b461-132">**roles**</span><span class="sxs-lookup"><span data-stu-id="6b461-132">**roles**</span></span>    | <span data-ttu-id="6b461-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b461-133">String collection</span></span> | <span data-ttu-id="6b461-134">Uma matriz de tipos de permissão.</span><span class="sxs-lookup"><span data-stu-id="6b461-134">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="6b461-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b461-135">Response</span></span>

<span data-ttu-id="6b461-136">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [permission](../resources/permission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b461-136">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b461-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b461-137">Example</span></span>

<span data-ttu-id="6b461-138">Aqui está um exemplo da solicitação que altera a função da permissão de compartilhamento para somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b461-138">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6b461-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b461-139">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b461-140">C#</span><span class="sxs-lookup"><span data-stu-id="6b461-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b461-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b461-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b461-142">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6b461-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6b461-143">Java</span><span class="sxs-lookup"><span data-stu-id="6b461-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b461-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b461-144">Response</span></span>

<span data-ttu-id="6b461-145">Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) no corpo da resposta que representa o estado atualizado da permissão.</span><span class="sxs-lookup"><span data-stu-id="6b461-145">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
