---
title: Listar connectedOrganizations
description: Recupere uma lista de objetos connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0d74b4624833ca8c6a9feecf824f6e4346ca952c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437440"
---
# <a name="list-connectedorganizations"></a><span data-ttu-id="6bd0e-103">Listar connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="6bd0e-103">List connectedOrganizations</span></span>

<span data-ttu-id="6bd0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6bd0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bd0e-105">Recupere uma lista de [objetos connectedOrganization.](../resources/connectedorganization.md)</span><span class="sxs-lookup"><span data-stu-id="6bd0e-105">Retrieve a list of [connectedOrganization](../resources/connectedorganization.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6bd0e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6bd0e-106">Permissions</span></span>

<span data-ttu-id="6bd0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bd0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bd0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6bd0e-109">Permission type</span></span>|<span data-ttu-id="6bd0e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6bd0e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="6bd0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6bd0e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6bd0e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bd0e-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6bd0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6bd0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bd0e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6bd0e-114">Not supported.</span></span> |
| <span data-ttu-id="6bd0e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6bd0e-115">Application</span></span>                            | <span data-ttu-id="6bd0e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bd0e-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6bd0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6bd0e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6bd0e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6bd0e-118">Optional query parameters</span></span>
<span data-ttu-id="6bd0e-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6bd0e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6bd0e-120">Por exemplo, para recuperar apenas as organizações conectadas com um nome de exibição específico, adicione `$filter=displayName eq 'Name'` .</span><span class="sxs-lookup"><span data-stu-id="6bd0e-120">For example, to retrieve only the connected organizations with a specific display name, add `$filter=displayName eq 'Name'`.</span></span> <span data-ttu-id="6bd0e-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6bd0e-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bd0e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd0e-122">Request headers</span></span>
|<span data-ttu-id="6bd0e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6bd0e-123">Name</span></span>|<span data-ttu-id="6bd0e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6bd0e-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6bd0e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6bd0e-125">Authorization</span></span>|<span data-ttu-id="6bd0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6bd0e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bd0e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd0e-128">Request body</span></span>
<span data-ttu-id="6bd0e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6bd0e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6bd0e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bd0e-130">Response</span></span>

<span data-ttu-id="6bd0e-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos connectedOrganization](../resources/connectedorganization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6bd0e-131">If successful, this method returns a `200 OK` response code and a collection of [connectedOrganization](../resources/connectedorganization.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6bd0e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6bd0e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6bd0e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6bd0e-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6bd0e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6bd0e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganizations"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations
```
# <a name="c"></a>[<span data-ttu-id="6bd0e-135">C#</span><span class="sxs-lookup"><span data-stu-id="6bd0e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6bd0e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6bd0e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6bd0e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6bd0e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6bd0e-138">Java</span><span class="sxs-lookup"><span data-stu-id="6bd0e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6bd0e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6bd0e-139">Response</span></span>
<span data-ttu-id="6bd0e-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6bd0e-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.connectedOrganization)"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectedOrganizations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


