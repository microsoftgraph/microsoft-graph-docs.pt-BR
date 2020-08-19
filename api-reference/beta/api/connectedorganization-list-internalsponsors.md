---
title: Listar internalSponsors
description: Recupere uma lista de internalSponsors do connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7a99dc0daf5c4f46bd0c4667d0833d2cadb7c24e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810150"
---
# <a name="list-internalsponsors"></a><span data-ttu-id="d21d6-103">Listar internalSponsors</span><span class="sxs-lookup"><span data-stu-id="d21d6-103">List internalSponsors</span></span>

<span data-ttu-id="d21d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d21d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d21d6-105">Recupere uma lista de patrocinadores internos de um [connectedOrganization](../resources/connectedorganization.md).</span><span class="sxs-lookup"><span data-stu-id="d21d6-105">Retrieve a list of a [connectedOrganization](../resources/connectedorganization.md)'s internal sponsors.</span></span>  <span data-ttu-id="d21d6-106">Os patrocinadores internos são um conjunto de usuários que podem aprovar solicitações em nome de outros usuários da organização conectada.</span><span class="sxs-lookup"><span data-stu-id="d21d6-106">The internal sponsors are a set of users who can approve requests on behalf of other users from that connected organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="d21d6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="d21d6-107">Permissions</span></span>

<span data-ttu-id="d21d6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d21d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d21d6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d21d6-110">Permission type</span></span>|<span data-ttu-id="d21d6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d21d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="d21d6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d21d6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d21d6-113">EntitlementManagement. Read. All, EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d21d6-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="d21d6-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d21d6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d21d6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d21d6-115">Not supported.</span></span> |
| <span data-ttu-id="d21d6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d21d6-116">Application</span></span>                            | <span data-ttu-id="d21d6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d21d6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d21d6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d21d6-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors
```

## <a name="request-headers"></a><span data-ttu-id="d21d6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d21d6-119">Request headers</span></span>
|<span data-ttu-id="d21d6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d21d6-120">Name</span></span>|<span data-ttu-id="d21d6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d21d6-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d21d6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d21d6-122">Authorization</span></span>|<span data-ttu-id="d21d6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d21d6-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d21d6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d21d6-125">Request body</span></span>
<span data-ttu-id="d21d6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d21d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d21d6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d21d6-127">Response</span></span>

<span data-ttu-id="d21d6-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d21d6-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d21d6-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d21d6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d21d6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d21d6-130">Request</span></span>

<span data-ttu-id="d21d6-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d21d6-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d21d6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d21d6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connectedorganization_get_internalSponsors"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}/internalSponsors
```
# <a name="c"></a>[<span data-ttu-id="d21d6-133">C#</span><span class="sxs-lookup"><span data-stu-id="d21d6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectedorganization-get-internalsponsors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d21d6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d21d6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectedorganization-get-internalsponsors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d21d6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d21d6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectedorganization-get-internalsponsors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d21d6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d21d6-136">Response</span></span>

<span data-ttu-id="d21d6-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d21d6-137">The following is an example of the response.</span></span>

<span data-ttu-id="d21d6-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d21d6-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "List internalSponsors",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
