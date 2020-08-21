---
title: Adicionar patrocinador externo da organização conectada
description: Adicionar um usuário ou grupo aos patrocinadores externos da organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 98a71e2e3e0ca5c15cb7321b2d4ae59ad5576506
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810180"
---
# <a name="add-connected-organization-external-sponsor"></a><span data-ttu-id="c0f10-103">Adicionar patrocinador externo da organização conectada</span><span class="sxs-lookup"><span data-stu-id="c0f10-103">Add connected organization external sponsor</span></span>

<span data-ttu-id="c0f10-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0f10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f10-105">Adicione um usuário ou um grupo aos patrocinadores externos da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="c0f10-105">Add a user or a group to the connected organization's external sponsors.</span></span> <span data-ttu-id="c0f10-106">Os patrocinadores externos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="c0f10-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0f10-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c0f10-107">Permissions</span></span>
<span data-ttu-id="c0f10-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0f10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0f10-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0f10-110">Permission type</span></span>      | <span data-ttu-id="c0f10-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c0f10-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0f10-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0f10-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0f10-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0f10-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="c0f10-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0f10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0f10-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0f10-115">Not supported.</span></span>    |
|<span data-ttu-id="c0f10-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0f10-116">Application</span></span> | <span data-ttu-id="c0f10-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0f10-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0f10-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0f10-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c0f10-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f10-119">Request headers</span></span>
| <span data-ttu-id="c0f10-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c0f10-120">Name</span></span>       | <span data-ttu-id="c0f10-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f10-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c0f10-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0f10-122">Authorization</span></span>  | <span data-ttu-id="c0f10-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0f10-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0f10-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="c0f10-125">Content-type</span></span> | <span data-ttu-id="c0f10-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0f10-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0f10-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f10-128">Request body</span></span>
<span data-ttu-id="c0f10-129">No corpo da solicitação, forneça uma representação JSON da referência ao objeto [User](../resources/user.md) ou [Group](../resources/group.md) a ser adicionado, como uma `@odata.id` propriedade com o URI completo do usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="c0f10-129">In the request body, supply a JSON representation of the reference to the [user](../resources/user.md) or [group](../resources/group.md) object to be added, as an `@odata.id` property with the full URI of the user or group.</span></span>

## <a name="response"></a><span data-ttu-id="c0f10-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0f10-130">Response</span></span>
<span data-ttu-id="c0f10-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0f10-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0f10-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0f10-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c0f10-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0f10-134">Request</span></span>

<span data-ttu-id="c0f10-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0f10-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0f10-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0f10-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalsponsor_from_connectedorganization"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/users/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="c0f10-137">C#</span><span class="sxs-lookup"><span data-stu-id="c0f10-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0f10-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0f10-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0f10-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0f10-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0f10-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0f10-140">Response</span></span>

<span data-ttu-id="c0f10-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c0f10-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connected organization external sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->