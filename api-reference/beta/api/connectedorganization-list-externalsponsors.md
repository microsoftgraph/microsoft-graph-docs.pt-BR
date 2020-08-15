---
title: Listar externalSponsors
description: Recupere uma lista de externalSponsors do connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a523c0a75b6cffb20738f42f33554accbe945c18
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757391"
---
# <a name="list-externalsponsors"></a><span data-ttu-id="72d6a-103">Listar externalSponsors</span><span class="sxs-lookup"><span data-stu-id="72d6a-103">List externalSponsors</span></span>

<span data-ttu-id="72d6a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72d6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72d6a-105">Recupere uma lista de patrocinadores externos de um [connectedOrganization](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="72d6a-105">Retrieve a list of a [connectedOrganization](../resources/connectedorganization.md)'s external sponsors.</span></span>  <span data-ttu-id="72d6a-106">Os patrocinadores externos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="72d6a-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="72d6a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="72d6a-107">Permissions</span></span>

<span data-ttu-id="72d6a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72d6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72d6a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72d6a-110">Permission type</span></span>|<span data-ttu-id="72d6a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="72d6a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="72d6a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72d6a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="72d6a-113">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="72d6a-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="72d6a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72d6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72d6a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72d6a-115">Not supported.</span></span> |
| <span data-ttu-id="72d6a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72d6a-116">Application</span></span>                            | <span data-ttu-id="72d6a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72d6a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72d6a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72d6a-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```

## <a name="request-headers"></a><span data-ttu-id="72d6a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72d6a-119">Request headers</span></span>
|<span data-ttu-id="72d6a-120">Nome</span><span class="sxs-lookup"><span data-stu-id="72d6a-120">Name</span></span>|<span data-ttu-id="72d6a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="72d6a-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="72d6a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="72d6a-122">Authorization</span></span>|<span data-ttu-id="72d6a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72d6a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72d6a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72d6a-125">Request body</span></span>
<span data-ttu-id="72d6a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72d6a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72d6a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="72d6a-127">Response</span></span>

<span data-ttu-id="72d6a-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72d6a-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72d6a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72d6a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72d6a-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72d6a-130">Request</span></span>

<span data-ttu-id="72d6a-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72d6a-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "connectedorganization_get_externalSponsors"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```

### <a name="response"></a><span data-ttu-id="72d6a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="72d6a-132">Response</span></span>

<span data-ttu-id="72d6a-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72d6a-133">The following is an example of the response.</span></span>

<span data-ttu-id="72d6a-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="72d6a-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List externalSponsors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
