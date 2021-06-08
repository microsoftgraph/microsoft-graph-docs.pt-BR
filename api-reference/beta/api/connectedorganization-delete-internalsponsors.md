---
title: Remover o patrocinador interno da organização conectado
description: Remova um usuário ou grupo dos patrocinadores internos da organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1b2eeb4df11235ca021b348bc1ad5f0068565dfe
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786163"
---
# <a name="remove-connected-organization-internal-sponsor"></a><span data-ttu-id="25545-103">Remover o patrocinador interno da organização conectado</span><span class="sxs-lookup"><span data-stu-id="25545-103">Remove connected organization internal sponsor</span></span>

<span data-ttu-id="25545-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25545-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25545-105">Remova um usuário ou um grupo dos patrocinadores internos da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="25545-105">Remove a user or a group from the connected organization's internal sponsors.</span></span> <span data-ttu-id="25545-106">Os patrocinadores internos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários dessa organização conectada.</span><span class="sxs-lookup"><span data-stu-id="25545-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="25545-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="25545-107">Permissions</span></span>
<span data-ttu-id="25545-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25545-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25545-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25545-110">Permission type</span></span>      | <span data-ttu-id="25545-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25545-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25545-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25545-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="25545-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25545-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="25545-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25545-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25545-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25545-115">Not supported.</span></span>    |
|<span data-ttu-id="25545-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25545-116">Application</span></span> | <span data-ttu-id="25545-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25545-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25545-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25545-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="25545-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25545-119">Request headers</span></span>
| <span data-ttu-id="25545-120">Nome</span><span class="sxs-lookup"><span data-stu-id="25545-120">Name</span></span>       | <span data-ttu-id="25545-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="25545-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="25545-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="25545-122">Authorization</span></span>  | <span data-ttu-id="25545-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25545-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25545-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25545-125">Request body</span></span>
<span data-ttu-id="25545-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25545-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25545-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="25545-127">Response</span></span>
<span data-ttu-id="25545-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25545-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25545-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25545-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="25545-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25545-131">Request</span></span>

<span data-ttu-id="25545-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25545-132">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="25545-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="25545-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_internalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="25545-134">C#</span><span class="sxs-lookup"><span data-stu-id="25545-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-internalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25545-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25545-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-internalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25545-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25545-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-internalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25545-137">Java</span><span class="sxs-lookup"><span data-stu-id="25545-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-internalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25545-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="25545-138">Response</span></span>

<span data-ttu-id="25545-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25545-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connected organization internal sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


