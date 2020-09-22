---
title: Remover patrocinador externo da organização conectada
description: Remover um usuário ou grupo dos patrocinadores externos da organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bfe43a22b42995b9e6ffc9423817b9631e1aa2ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982385"
---
# <a name="remove-connected-organization-external-sponsor"></a><span data-ttu-id="6db73-103">Remover patrocinador externo da organização conectada</span><span class="sxs-lookup"><span data-stu-id="6db73-103">Remove connected organization external sponsor</span></span>

<span data-ttu-id="6db73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6db73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6db73-105">Remover um usuário ou grupo dos patrocinadores externos da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="6db73-105">Remove a user or a group from the connected organization's external sponsors.</span></span> <span data-ttu-id="6db73-106">Os patrocinadores externos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="6db73-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="6db73-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6db73-107">Permissions</span></span>
<span data-ttu-id="6db73-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6db73-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6db73-110">Permission type</span></span>      | <span data-ttu-id="6db73-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6db73-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6db73-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6db73-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6db73-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6db73-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="6db73-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6db73-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6db73-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6db73-115">Not supported.</span></span>    |
|<span data-ttu-id="6db73-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6db73-116">Application</span></span> | <span data-ttu-id="6db73-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6db73-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6db73-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6db73-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="6db73-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-119">Request headers</span></span>
| <span data-ttu-id="6db73-120">Nome</span><span class="sxs-lookup"><span data-stu-id="6db73-120">Name</span></span>       | <span data-ttu-id="6db73-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db73-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6db73-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6db73-122">Authorization</span></span>  | <span data-ttu-id="6db73-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6db73-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6db73-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-125">Request body</span></span>
<span data-ttu-id="6db73-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6db73-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6db73-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db73-127">Response</span></span>
<span data-ttu-id="6db73-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6db73-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6db73-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6db73-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6db73-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-131">Request</span></span>

<span data-ttu-id="6db73-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db73-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6db73-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6db73-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="6db73-134">C#</span><span class="sxs-lookup"><span data-stu-id="6db73-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6db73-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6db73-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6db73-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6db73-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6db73-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db73-137">Response</span></span>

<span data-ttu-id="6db73-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6db73-138">The following is an example of the response.</span></span>

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
  "description": "Delete connected organization external sponsor",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


