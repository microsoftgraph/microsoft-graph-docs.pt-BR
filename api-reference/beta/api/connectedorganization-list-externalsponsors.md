---
title: Listar externalSponsors
description: Recupere uma lista de externalSponsors do connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3b4a72fc419b64863a51c6a422bea17e35911b35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996525"
---
# <a name="list-externalsponsors"></a><span data-ttu-id="8d94f-103">Listar externalSponsors</span><span class="sxs-lookup"><span data-stu-id="8d94f-103">List externalSponsors</span></span>

<span data-ttu-id="8d94f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d94f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d94f-105">Recupere uma lista de patrocinadores externos de um [connectedOrganization](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="8d94f-105">Retrieve a list of a [connectedOrganization](../resources/connectedorganization.md)'s external sponsors.</span></span>  <span data-ttu-id="8d94f-106">Os patrocinadores externos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="8d94f-106">The external sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d94f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d94f-107">Permissions</span></span>

<span data-ttu-id="8d94f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d94f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d94f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d94f-110">Permission type</span></span>|<span data-ttu-id="8d94f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d94f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="8d94f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d94f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d94f-113">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8d94f-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="8d94f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d94f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d94f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d94f-115">Not supported.</span></span> |
| <span data-ttu-id="8d94f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d94f-116">Application</span></span>                            | <span data-ttu-id="8d94f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d94f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d94f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d94f-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```

## <a name="request-headers"></a><span data-ttu-id="8d94f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d94f-119">Request headers</span></span>
|<span data-ttu-id="8d94f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8d94f-120">Name</span></span>|<span data-ttu-id="8d94f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d94f-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8d94f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d94f-122">Authorization</span></span>|<span data-ttu-id="8d94f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d94f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d94f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d94f-125">Request body</span></span>
<span data-ttu-id="8d94f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d94f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d94f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d94f-127">Response</span></span>

<span data-ttu-id="8d94f-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d94f-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d94f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8d94f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d94f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d94f-130">Request</span></span>

<span data-ttu-id="8d94f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d94f-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8d94f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d94f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connectedorganization_get_externalSponsors"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/externalSponsors
```
# <a name="c"></a>[<span data-ttu-id="8d94f-133">C#</span><span class="sxs-lookup"><span data-stu-id="8d94f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectedorganization-get-externalsponsors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d94f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d94f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectedorganization-get-externalsponsors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d94f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d94f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectedorganization-get-externalsponsors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d94f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d94f-136">Response</span></span>

<span data-ttu-id="8d94f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8d94f-137">The following is an example of the response.</span></span>

<span data-ttu-id="8d94f-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8d94f-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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


