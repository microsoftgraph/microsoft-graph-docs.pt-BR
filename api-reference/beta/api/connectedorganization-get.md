---
title: Obter connectedOrganization
description: Recupere as propriedades e os relacionamentos de um objeto connectedorganization.
author: markwahl-msft
ms.prod: microsoft-identity-platform
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 27b0765bf16f4fabf5057b35ad4d1b0992ba79de
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872706"
---
# <a name="get-connectedorganization"></a><span data-ttu-id="ed01b-103">Obter connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="ed01b-103">Get connectedOrganization</span></span>

<span data-ttu-id="ed01b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed01b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed01b-105">Recupere as propriedades e os relacionamentos de um [objeto connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="ed01b-105">Retrieve the properties and relationships of a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed01b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed01b-106">Permissions</span></span>

<span data-ttu-id="ed01b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed01b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed01b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed01b-109">Permission type</span></span>|<span data-ttu-id="ed01b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed01b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="ed01b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed01b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed01b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed01b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ed01b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed01b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed01b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed01b-114">Not supported.</span></span> |
| <span data-ttu-id="ed01b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed01b-115">Application</span></span>                            | <span data-ttu-id="ed01b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed01b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed01b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed01b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed01b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ed01b-118">Optional query parameters</span></span>

<span data-ttu-id="ed01b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ed01b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ed01b-120">Por exemplo, para recuperar apenas as fontes de identidade, adicione `$select=identitySources` .</span><span class="sxs-lookup"><span data-stu-id="ed01b-120">For example, to retrieve only the identity sources, add `$select=identitySources`.</span></span> <span data-ttu-id="ed01b-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ed01b-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed01b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed01b-122">Request headers</span></span>

|<span data-ttu-id="ed01b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="ed01b-123">Name</span></span>|<span data-ttu-id="ed01b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed01b-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed01b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed01b-125">Authorization</span></span>|<span data-ttu-id="ed01b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed01b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed01b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed01b-128">Request body</span></span>

<span data-ttu-id="ed01b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed01b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed01b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed01b-130">Response</span></span>

<span data-ttu-id="ed01b-131">Se bem-sucedido, este método retorna um código de resposta e um `200 OK` [objeto connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed01b-131">If successful, this method returns a `200 OK` response code and a [connectedOrganization](../resources/connectedorganization.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed01b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ed01b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed01b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed01b-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ed01b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed01b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganization"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```
# <a name="c"></a>[<span data-ttu-id="ed01b-135">C#</span><span class="sxs-lookup"><span data-stu-id="ed01b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed01b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed01b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed01b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed01b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed01b-138">Java</span><span class="sxs-lookup"><span data-stu-id="ed01b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed01b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed01b-139">Response</span></span>

<span data-ttu-id="ed01b-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ed01b-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


