---
title: Obter connectedOrganization
description: Recupere as propriedades e as relações de um objeto connectedorganization.
author: markwahl-msft
ms.prod: governance
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: ec4bfa06754f9381c19154e886691f7657e0ab18
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437482"
---
# <a name="get-connectedorganization"></a><span data-ttu-id="1f461-103">Obter connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="1f461-103">Get connectedOrganization</span></span>

<span data-ttu-id="1f461-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f461-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f461-105">Recupere as propriedades e as relações de um [objeto connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="1f461-105">Retrieve the properties and relationships of a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f461-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1f461-106">Permissions</span></span>

<span data-ttu-id="1f461-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f461-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f461-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f461-109">Permission type</span></span>|<span data-ttu-id="1f461-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1f461-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="1f461-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f461-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f461-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f461-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1f461-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f461-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f461-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f461-114">Not supported.</span></span> |
| <span data-ttu-id="1f461-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f461-115">Application</span></span>                            | <span data-ttu-id="1f461-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f461-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f461-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f461-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f461-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1f461-118">Optional query parameters</span></span>

<span data-ttu-id="1f461-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1f461-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1f461-120">Por exemplo, para recuperar apenas as fontes de identidade, adicione `$select=identitySources` .</span><span class="sxs-lookup"><span data-stu-id="1f461-120">For example, to retrieve only the identity sources, add `$select=identitySources`.</span></span> <span data-ttu-id="1f461-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1f461-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f461-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f461-122">Request headers</span></span>

|<span data-ttu-id="1f461-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1f461-123">Name</span></span>|<span data-ttu-id="1f461-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f461-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1f461-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f461-125">Authorization</span></span>|<span data-ttu-id="1f461-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f461-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f461-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f461-128">Request body</span></span>

<span data-ttu-id="1f461-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f461-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f461-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f461-130">Response</span></span>

<span data-ttu-id="1f461-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f461-131">If successful, this method returns a `200 OK` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f461-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1f461-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f461-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f461-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1f461-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1f461-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganization"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="1f461-135">C#</span><span class="sxs-lookup"><span data-stu-id="1f461-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1f461-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1f461-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1f461-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1f461-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1f461-138">Java</span><span class="sxs-lookup"><span data-stu-id="1f461-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1f461-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f461-139">Response</span></span>

<span data-ttu-id="1f461-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1f461-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectedOrganization"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f",
  "displayName": "Wingtip Toys",
  "description": "Wingtip Toys",
  "createdBy": "admin@contoso.com",
  "createdDateTime": "2020-05-13T15:18:04.81Z",
  "modifiedBy": "admin@contoso.com",
  "modifiedDateTime": "2020-05-13T15:18:04.81Z",
  "identitySources": [
    {
      "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "bf85dc9d-cb43-44a4-80c4-469e8c58249e",
      "displayName": "Wingtip Toys Co"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


