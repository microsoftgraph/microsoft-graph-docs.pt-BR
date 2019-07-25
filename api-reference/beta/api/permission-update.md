---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Alterar permissões de compartilhamento
localization_priority: Normal
ms.openlocfilehash: f2bc5954380836af12382ec02f4d04f9fa4c29c3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876985"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="285ac-102">Atualizar a permissão de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="285ac-102">Update sharing permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="285ac-103">Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.</span><span class="sxs-lookup"><span data-stu-id="285ac-103">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="285ac-104">Somente a propriedade **roles** pode ser modificada dessa forma.</span><span class="sxs-lookup"><span data-stu-id="285ac-104">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="285ac-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="285ac-105">Permissions</span></span>

<span data-ttu-id="285ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="285ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="285ac-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="285ac-108">Permission type</span></span>      | <span data-ttu-id="285ac-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="285ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="285ac-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="285ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="285ac-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285ac-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="285ac-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="285ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="285ac-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285ac-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="285ac-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="285ac-114">Application</span></span> | <span data-ttu-id="285ac-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="285ac-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="285ac-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="285ac-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="285ac-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="285ac-117">Optional request headers</span></span>

| <span data-ttu-id="285ac-118">Nome</span><span class="sxs-lookup"><span data-stu-id="285ac-118">Name</span></span>          | <span data-ttu-id="285ac-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="285ac-119">Type</span></span>   | <span data-ttu-id="285ac-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="285ac-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="285ac-121">if-match</span><span class="sxs-lookup"><span data-stu-id="285ac-121">if-match</span></span>      | <span data-ttu-id="285ac-122">string</span><span class="sxs-lookup"><span data-stu-id="285ac-122">string</span></span> | <span data-ttu-id="285ac-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="285ac-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="285ac-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="285ac-124">Request body</span></span>

<span data-ttu-id="285ac-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="285ac-125">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="285ac-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="285ac-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="285ac-127">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="285ac-127">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="285ac-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="285ac-128">Property</span></span>     | <span data-ttu-id="285ac-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="285ac-129">Type</span></span>   | <span data-ttu-id="285ac-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="285ac-130">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="285ac-131">**roles**</span><span class="sxs-lookup"><span data-stu-id="285ac-131">**roles**</span></span>    | <span data-ttu-id="285ac-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="285ac-132">String collection</span></span> | <span data-ttu-id="285ac-133">Uma matriz de tipos de permissão.</span><span class="sxs-lookup"><span data-stu-id="285ac-133">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="285ac-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="285ac-134">Response</span></span>

<span data-ttu-id="285ac-135">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [permission](../resources/permission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="285ac-135">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="285ac-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="285ac-136">Example</span></span>

<span data-ttu-id="285ac-137">Aqui está um exemplo da solicitação que altera a função da permissão de compartilhamento para somente leitura.</span><span class="sxs-lookup"><span data-stu-id="285ac-137">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="285ac-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="285ac-138">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="285ac-139">C#</span><span class="sxs-lookup"><span data-stu-id="285ac-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="285ac-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="285ac-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="285ac-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="285ac-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="285ac-142">Java</span><span class="sxs-lookup"><span data-stu-id="285ac-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="285ac-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="285ac-143">Response</span></span>

<span data-ttu-id="285ac-144">Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) no corpo da resposta que representa o estado atualizado da permissão.</span><span class="sxs-lookup"><span data-stu-id="285ac-144">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
