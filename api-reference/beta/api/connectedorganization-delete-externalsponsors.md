---
title: Remover patrocinador externo da organização conectada
description: Remova um usuário ou grupo dos patrocinadores externos da organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 189abc149f7dd076ee8c03b523868d2d49356921
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437531"
---
# <a name="remove-connected-organization-external-sponsor"></a><span data-ttu-id="ca8c2-103">Remover patrocinador externo da organização conectada</span><span class="sxs-lookup"><span data-stu-id="ca8c2-103">Remove connected organization external sponsor</span></span>

<span data-ttu-id="ca8c2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca8c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca8c2-105">Remova um usuário ou um grupo dos patrocinadores externos da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="ca8c2-105">Remove a user or a group from the connected organization's external sponsors.</span></span> <span data-ttu-id="ca8c2-106">Os patrocinadores externos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários dessa organização conectada.</span><span class="sxs-lookup"><span data-stu-id="ca8c2-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca8c2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca8c2-107">Permissions</span></span>
<span data-ttu-id="ca8c2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca8c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca8c2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca8c2-110">Permission type</span></span>      | <span data-ttu-id="ca8c2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca8c2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca8c2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca8c2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca8c2-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8c2-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="ca8c2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca8c2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca8c2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca8c2-115">Not supported.</span></span>    |
|<span data-ttu-id="ca8c2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca8c2-116">Application</span></span> | <span data-ttu-id="ca8c2-117">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca8c2-117">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca8c2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8c2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ca8c2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8c2-119">Request headers</span></span>
| <span data-ttu-id="ca8c2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ca8c2-120">Name</span></span>       | <span data-ttu-id="ca8c2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca8c2-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ca8c2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca8c2-122">Authorization</span></span>  | <span data-ttu-id="ca8c2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca8c2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca8c2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8c2-125">Request body</span></span>
<span data-ttu-id="ca8c2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ca8c2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca8c2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8c2-127">Response</span></span>
<span data-ttu-id="ca8c2-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca8c2-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca8c2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca8c2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca8c2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca8c2-131">Request</span></span>

<span data-ttu-id="ca8c2-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca8c2-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ca8c2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca8c2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="ca8c2-134">C#</span><span class="sxs-lookup"><span data-stu-id="ca8c2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalsponsor-from-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca8c2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca8c2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalsponsor-from-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca8c2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca8c2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalsponsor-from-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca8c2-137">Java</span><span class="sxs-lookup"><span data-stu-id="ca8c2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalsponsor-from-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ca8c2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca8c2-138">Response</span></span>

<span data-ttu-id="ca8c2-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ca8c2-139">The following is an example of the response.</span></span>

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


