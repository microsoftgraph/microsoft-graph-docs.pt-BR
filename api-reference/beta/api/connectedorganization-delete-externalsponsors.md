---
title: Remover patrocinador externo da organização conectada
description: Remover um usuário ou grupo dos patrocinadores externos da organização conectada.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bfdb23fe1da1c1724b47b9a17a9846d3d708ebbf
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757406"
---
# <a name="remove-connected-organization-external-sponsor"></a><span data-ttu-id="97d40-103">Remover patrocinador externo da organização conectada</span><span class="sxs-lookup"><span data-stu-id="97d40-103">Remove connected organization external sponsor</span></span>

<span data-ttu-id="97d40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97d40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97d40-105">Remover um usuário ou grupo dos patrocinadores externos da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="97d40-105">Remove a user or a group from the connected organization's external sponsors.</span></span> <span data-ttu-id="97d40-106">Os patrocinadores externos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="97d40-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="97d40-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="97d40-107">Permissions</span></span>
<span data-ttu-id="97d40-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97d40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97d40-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97d40-110">Permission type</span></span>      | <span data-ttu-id="97d40-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97d40-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97d40-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97d40-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="97d40-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97d40-113">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="97d40-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97d40-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97d40-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97d40-115">Not supported.</span></span>    |
|<span data-ttu-id="97d40-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97d40-116">Application</span></span> | <span data-ttu-id="97d40-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97d40-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97d40-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97d40-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="97d40-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97d40-119">Request headers</span></span>
| <span data-ttu-id="97d40-120">Nome</span><span class="sxs-lookup"><span data-stu-id="97d40-120">Name</span></span>       | <span data-ttu-id="97d40-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="97d40-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="97d40-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="97d40-122">Authorization</span></span>  | <span data-ttu-id="97d40-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97d40-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97d40-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97d40-125">Request body</span></span>
<span data-ttu-id="97d40-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97d40-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97d40-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d40-127">Response</span></span>
<span data-ttu-id="97d40-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97d40-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97d40-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97d40-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97d40-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97d40-131">Request</span></span>

<span data-ttu-id="97d40-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97d40-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_externalsponsor_from_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{connectedOrganizationId}/externalSponsors/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="97d40-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="97d40-133">Response</span></span>

<span data-ttu-id="97d40-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97d40-134">The following is an example of the response.</span></span>

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
