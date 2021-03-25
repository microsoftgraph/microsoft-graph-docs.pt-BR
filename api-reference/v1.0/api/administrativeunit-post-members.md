---
title: Adicionar um membro
description: Use essa API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8fac296f9bf281a1ef3140f469dfd80f7c0a935b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202135"
---
# <a name="add-a-member"></a><span data-ttu-id="8c6e2-103">Adicionar um membro</span><span class="sxs-lookup"><span data-stu-id="8c6e2-103">Add a member</span></span>

<span data-ttu-id="8c6e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c6e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c6e2-105">Use essa API para adicionar um membro (usuário ou grupo) a uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="8c6e2-105">Use this API to add a member (user or group) to an administrative unit.</span></span>

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a><span data-ttu-id="8c6e2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c6e2-106">Permissions</span></span>
<span data-ttu-id="8c6e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c6e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c6e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c6e2-109">Permission type</span></span>      | <span data-ttu-id="8c6e2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c6e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c6e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c6e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8c6e2-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8c6e2-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c6e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c6e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c6e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c6e2-114">Not supported.</span></span>    |
|<span data-ttu-id="8c6e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c6e2-115">Application</span></span> | <span data-ttu-id="8c6e2-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c6e2-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c6e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c6e2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8c6e2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c6e2-118">Request headers</span></span>
| <span data-ttu-id="8c6e2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8c6e2-119">Name</span></span>      |<span data-ttu-id="8c6e2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c6e2-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c6e2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c6e2-121">Authorization</span></span>  | <span data-ttu-id="8c6e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c6e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c6e2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c6e2-124">Request body</span></span>
<span data-ttu-id="8c6e2-125">No corpo da solicitação, forneça o de um usuário , grupo ou `id` [directoryObject](../resources/directoryobject.md) a ser adicionado. [](../resources/user.md) [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="8c6e2-125">In the request body, provide the `id` of a [user](../resources/user.md),  [group](../resources/group.md) or [directoryObject](../resources/directoryobject.md) to be added.</span></span>

## <a name="response"></a><span data-ttu-id="8c6e2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c6e2-126">Response</span></span>

<span data-ttu-id="8c6e2-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c6e2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c6e2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c6e2-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c6e2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c6e2-130">Request</span></span>
<span data-ttu-id="8c6e2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c6e2-131">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8c6e2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c6e2-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8c6e2-133">C#</span><span class="sxs-lookup"><span data-stu-id="8c6e2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c6e2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c6e2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c6e2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c6e2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8c6e2-136">Java</span><span class="sxs-lookup"><span data-stu-id="8c6e2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8c6e2-137">No corpo da solicitação, forneça o `id` objeto [do usuário](../resources/user.md) ou grupo que você deseja adicionar. [](../resources/group.md)</span><span class="sxs-lookup"><span data-stu-id="8c6e2-137">In the request body, provide the `id` of the [user](../resources/user.md) or [group](../resources/group.md) object you want to add.</span></span>

### <a name="response"></a><span data-ttu-id="8c6e2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c6e2-138">Response</span></span>
<span data-ttu-id="8c6e2-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c6e2-139">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
