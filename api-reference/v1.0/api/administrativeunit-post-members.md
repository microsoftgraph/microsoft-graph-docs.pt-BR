---
title: Adicionar um membro
description: Use essa API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 634013e968b5fc69c2565848bf85e343f03b2f4f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991488"
---
# <a name="add-a-member"></a><span data-ttu-id="218b9-103">Adicionar um membro</span><span class="sxs-lookup"><span data-stu-id="218b9-103">Add a member</span></span>

<span data-ttu-id="218b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="218b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="218b9-105">Use essa API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="218b9-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="218b9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="218b9-106">Permissions</span></span>
<span data-ttu-id="218b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="218b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="218b9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="218b9-109">Permission type</span></span>      | <span data-ttu-id="218b9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="218b9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="218b9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="218b9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="218b9-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="218b9-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="218b9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="218b9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="218b9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="218b9-114">Not supported.</span></span>    |
|<span data-ttu-id="218b9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="218b9-115">Application</span></span> | <span data-ttu-id="218b9-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="218b9-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="218b9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="218b9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="218b9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="218b9-118">Request headers</span></span>
| <span data-ttu-id="218b9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="218b9-119">Name</span></span>      |<span data-ttu-id="218b9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="218b9-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="218b9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="218b9-121">Authorization</span></span>  | <span data-ttu-id="218b9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="218b9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="218b9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="218b9-124">Request body</span></span>
<span data-ttu-id="218b9-125">No corpo da solicitação, forneça o de um usuário , grupo ou `id` [directoryObject](../resources/directoryobject.md) a ser adicionado. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="218b9-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="218b9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="218b9-126">Response</span></span>

<span data-ttu-id="218b9-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="218b9-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="218b9-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="218b9-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="218b9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="218b9-130">Request</span></span>
<span data-ttu-id="218b9-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="218b9-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="218b9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="218b9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeUnits_members"
} -->
```http
POST https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/v1.0/groups/{id}"
}

```
# <a name="c"></a>[<span data-ttu-id="218b9-133">C#</span><span class="sxs-lookup"><span data-stu-id="218b9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="218b9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="218b9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="218b9-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="218b9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="218b9-136">Java</span><span class="sxs-lookup"><span data-stu-id="218b9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="218b9-137">No corpo da solicitação, forneça o `id` objeto [do usuário](../resources/user.md) ou grupo que você deseja adicionar. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="218b9-137">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="218b9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="218b9-138">Response</span></span>
<span data-ttu-id="218b9-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="218b9-139">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
