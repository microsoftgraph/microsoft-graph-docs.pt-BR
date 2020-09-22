---
title: Remover patrocinador interno da organização conectada
description: Remover um usuário ou grupo dos patrocinadores internos da organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 303adc9bb54599a358cb318bfb98e84e7f4423bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982371"
---
# <a name="remove-connected-organization-internal-sponsor"></a><span data-ttu-id="6f490-103">Remover patrocinador interno da organização conectada</span><span class="sxs-lookup"><span data-stu-id="6f490-103">Remove connected organization internal sponsor</span></span>

<span data-ttu-id="6f490-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f490-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f490-105">Remover um usuário ou grupo dos patrocinadores internos da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="6f490-105">Remove a user or a group from the connected organization's internal sponsors.</span></span> <span data-ttu-id="6f490-106">Os patrocinadores internos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="6f490-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f490-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6f490-107">Permissions</span></span>
<span data-ttu-id="6f490-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f490-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f490-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f490-110">Permission type</span></span>      | <span data-ttu-id="6f490-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6f490-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f490-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f490-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6f490-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f490-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="6f490-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f490-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f490-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f490-115">Not supported.</span></span>    |
|<span data-ttu-id="6f490-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f490-116">Application</span></span> | <span data-ttu-id="6f490-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f490-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f490-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f490-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6f490-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f490-119">Request headers</span></span>
| <span data-ttu-id="6f490-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6f490-120">Name</span></span>       | <span data-ttu-id="6f490-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f490-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f490-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f490-122">Authorization</span></span>  | <span data-ttu-id="6f490-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f490-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f490-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f490-125">Request body</span></span>
<span data-ttu-id="6f490-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f490-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f490-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f490-127">Response</span></span>
<span data-ttu-id="6f490-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f490-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f490-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f490-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f490-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f490-131">Request</span></span>

<span data-ttu-id="6f490-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f490-132">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="6f490-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f490-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_internalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="6f490-134">C#</span><span class="sxs-lookup"><span data-stu-id="6f490-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-internalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f490-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f490-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-internalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f490-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f490-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-internalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6f490-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f490-137">Response</span></span>

<span data-ttu-id="6f490-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6f490-138">The following is an example of the response.</span></span>

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
  "description": "Delete connected organization internal sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


