---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Alterar permissões de compartilhamento
localization_priority: Normal
ms.openlocfilehash: 44f98d559ab6dc4c81a4efede2f3f60020c2f944
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859679"
---
# <a name="update-sharing-permission"></a><span data-ttu-id="12bd1-102">Atualizar a permissão de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="12bd1-102">Update sharing permission</span></span>

> <span data-ttu-id="12bd1-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="12bd1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12bd1-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="12bd1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12bd1-105">Atualiza as propriedades de permissão de compartilhamento pela correção do recurso de permissão.</span><span class="sxs-lookup"><span data-stu-id="12bd1-105">Update the properties of a sharing permission by patching the permission resource.</span></span>

<span data-ttu-id="12bd1-106">Somente a propriedade **roles** pode ser modificada dessa forma.</span><span class="sxs-lookup"><span data-stu-id="12bd1-106">Only the **roles** property can be modified this way.</span></span>

## <a name="permissions"></a><span data-ttu-id="12bd1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="12bd1-107">Permissions</span></span>

<span data-ttu-id="12bd1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12bd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12bd1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12bd1-110">Permission type</span></span>      | <span data-ttu-id="12bd1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12bd1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12bd1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12bd1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12bd1-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12bd1-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="12bd1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12bd1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12bd1-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12bd1-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="12bd1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12bd1-116">Application</span></span> | <span data-ttu-id="12bd1-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12bd1-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12bd1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12bd1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
PATCH /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="12bd1-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="12bd1-119">Optional request headers</span></span>

| <span data-ttu-id="12bd1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="12bd1-120">Name</span></span>          | <span data-ttu-id="12bd1-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="12bd1-121">Type</span></span>   | <span data-ttu-id="12bd1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="12bd1-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="12bd1-123">if-match</span><span class="sxs-lookup"><span data-stu-id="12bd1-123">if-match</span></span>      | <span data-ttu-id="12bd1-124">string</span><span class="sxs-lookup"><span data-stu-id="12bd1-124">string</span></span> | <span data-ttu-id="12bd1-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="12bd1-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12bd1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12bd1-126">Request body</span></span>

<span data-ttu-id="12bd1-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="12bd1-127">In the request body, supply the values for relevant fields that should be updated.</span></span>

<span data-ttu-id="12bd1-128">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="12bd1-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="12bd1-129">Para obter o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="12bd1-129">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="12bd1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12bd1-130">Property</span></span>     | <span data-ttu-id="12bd1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="12bd1-131">Type</span></span>   | <span data-ttu-id="12bd1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="12bd1-132">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="12bd1-133">**roles**</span><span class="sxs-lookup"><span data-stu-id="12bd1-133">**roles**</span></span>    | <span data-ttu-id="12bd1-134">String</span><span class="sxs-lookup"><span data-stu-id="12bd1-134">String</span></span> | <span data-ttu-id="12bd1-135">Uma matriz de tipos de permissão.</span><span class="sxs-lookup"><span data-stu-id="12bd1-135">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="12bd1-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="12bd1-136">Response</span></span>

<span data-ttu-id="12bd1-137">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [permission](../resources/permission.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12bd1-137">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12bd1-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12bd1-138">Example</span></span>

<span data-ttu-id="12bd1-139">Aqui está um exemplo da solicitação que altera a função da permissão de compartilhamento para somente leitura.</span><span class="sxs-lookup"><span data-stu-id="12bd1-139">Here is an example of the request that changes the role on the sharing permission to read-only.</span></span>

<!-- {"blockType": "request", "name": "update-permission", "@odata.type": "microsoft.graph.permission", "scopes": "files.readwrite"} -->

```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```

### <a name="response"></a><span data-ttu-id="12bd1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="12bd1-140">Response</span></span>

<span data-ttu-id="12bd1-141">Se for bem-sucedido, esse método retornará um recurso [Permission](../resources/permission.md) no corpo da resposta que representa o estado atualizado da permissão.</span><span class="sxs-lookup"><span data-stu-id="12bd1-141">If successful, this method returns a [Permission](../resources/permission.md) resource in the response body that represents the updated state of the permission.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update an item's sharing permissions",
  "keywords": "permission, permissions, sharing, change permissions, update permission",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
