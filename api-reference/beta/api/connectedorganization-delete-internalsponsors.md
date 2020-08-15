---
title: Remover patrocinador interno da organização conectada
description: Remover um usuário ou grupo dos patrocinadores internos da organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0085f4641ab03b0b4f93e13e116ff34be514397f
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757405"
---
# <a name="remove-connected-organization-internal-sponsor"></a><span data-ttu-id="94a9e-103">Remover patrocinador interno da organização conectada</span><span class="sxs-lookup"><span data-stu-id="94a9e-103">Remove connected organization internal sponsor</span></span>

<span data-ttu-id="94a9e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a9e-105">Remover um usuário ou grupo dos patrocinadores internos da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="94a9e-105">Remove a user or a group from the connected organization's internal sponsors.</span></span> <span data-ttu-id="94a9e-106">Os patrocinadores internos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="94a9e-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="94a9e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="94a9e-107">Permissions</span></span>
<span data-ttu-id="94a9e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a9e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a9e-110">Permission type</span></span>      | <span data-ttu-id="94a9e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a9e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a9e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a9e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="94a9e-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a9e-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="94a9e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a9e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a9e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a9e-115">Not supported.</span></span>    |
|<span data-ttu-id="94a9e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a9e-116">Application</span></span> | <span data-ttu-id="94a9e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a9e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a9e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a9e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="94a9e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a9e-119">Request headers</span></span>
| <span data-ttu-id="94a9e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="94a9e-120">Name</span></span>       | <span data-ttu-id="94a9e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a9e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="94a9e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a9e-122">Authorization</span></span>  | <span data-ttu-id="94a9e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94a9e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94a9e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a9e-125">Request body</span></span>
<span data-ttu-id="94a9e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94a9e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94a9e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a9e-127">Response</span></span>
<span data-ttu-id="94a9e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a9e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a9e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a9e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="94a9e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a9e-131">Request</span></span>

<span data-ttu-id="94a9e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94a9e-132">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "delete_internalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/internalSponsors/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="94a9e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a9e-133">Response</span></span>

<span data-ttu-id="94a9e-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94a9e-134">The following is an example of the response.</span></span>

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
