---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Alterar permissões de compartilhamento
localization_priority: Normal
ms.openlocfilehash: fa32f4bbc8867088ceb776cfb7f2556ca49d2f1e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611370"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="d8706-102">Atualizar a permissão de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="d8706-102">Update sharing permission</span></span>

<span data-ttu-id="d8706-103">Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.</span><span class="sxs-lookup"><span data-stu-id="d8706-103">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="d8706-104">Somente a propriedade **roles** pode ser modificada dessa forma.</span><span class="sxs-lookup"><span data-stu-id="d8706-104">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8706-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8706-105">Permissions</span></span>

<span data-ttu-id="d8706-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8706-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8706-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8706-108">Permission type</span></span>      | <span data-ttu-id="d8706-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8706-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8706-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8706-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d8706-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8706-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8706-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8706-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8706-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8706-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8706-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8706-114">Application</span></span> | <span data-ttu-id="d8706-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8706-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8706-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8706-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="d8706-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d8706-117">Optional request headers</span></span>

| <span data-ttu-id="d8706-118">Nome</span><span class="sxs-lookup"><span data-stu-id="d8706-118">Name</span></span>          | <span data-ttu-id="d8706-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8706-119">Type</span></span>   | <span data-ttu-id="d8706-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8706-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d8706-121">if-match</span><span class="sxs-lookup"><span data-stu-id="d8706-121">if-match</span></span>      | <span data-ttu-id="d8706-122">string</span><span class="sxs-lookup"><span data-stu-id="d8706-122">string</span></span> | <span data-ttu-id="d8706-123">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="d8706-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8706-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8706-124">Request body</span></span>

<span data-ttu-id="d8706-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="d8706-125">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="d8706-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="d8706-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="d8706-127">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d8706-127">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d8706-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8706-128">Property</span></span> | <span data-ttu-id="d8706-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8706-129">Type</span></span>              | <span data-ttu-id="d8706-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8706-130">Description</span></span>                   |
|:---------|:------------------|:------------------------------|
| <span data-ttu-id="d8706-131">funções</span><span class="sxs-lookup"><span data-stu-id="d8706-131">roles</span></span>    | <span data-ttu-id="d8706-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d8706-132">String collection</span></span> | <span data-ttu-id="d8706-133">Uma matriz de tipos de permissão.</span><span class="sxs-lookup"><span data-stu-id="d8706-133">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="d8706-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8706-134">Response</span></span>

<span data-ttu-id="d8706-135">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [permission](../resources/permission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8706-135">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8706-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8706-136">Example</span></span>

<span data-ttu-id="d8706-137">Aqui está um exemplo da solicitação que altera a função da permissão de compartilhamento para somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d8706-137">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- { "blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="d8706-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8706-138">Response</span></span>

<span data-ttu-id="d8706-139">Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) no corpo da resposta que representa o estado atualizado da permissão.</span><span class="sxs-lookup"><span data-stu-id="d8706-139">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d8706-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="d8706-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d8706-141">Basic</span><span class="sxs-lookup"><span data-stu-id="d8706-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update-permission-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8706-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8706-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update-permission-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="d8706-143">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="d8706-143">Error responses</span></span>

<span data-ttu-id="d8706-144">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="d8706-144">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "Sharing/Update permission",
  "suppressions": [
    "Error: /api-reference/v1.0/api/permission-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/permission-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
