---
title: Listar roleManagementPolicies
description: Obter os recursos unifiedRoleManagementPolicy da propriedade de navegação roleManagementPolicies.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d51e045c25229ceffe84a3553be8878b001bdc24
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680721"
---
# <a name="list-rolemanagementpolicies"></a><span data-ttu-id="64b62-103">Listar roleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="64b62-103">List roleManagementPolicies</span></span>
<span data-ttu-id="64b62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="64b62-105">Obter os recursos unifiedRoleManagementPolicy da propriedade de navegação roleManagementPolicies.</span><span class="sxs-lookup"><span data-stu-id="64b62-105">Get the unifiedRoleManagementPolicy resources from the roleManagementPolicies navigation property.</span></span>


## <a name="permissions"></a><span data-ttu-id="64b62-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="64b62-106">Permissions</span></span>
<span data-ttu-id="64b62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64b62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b62-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64b62-109">Permission type</span></span>|<span data-ttu-id="64b62-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64b62-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64b62-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64b62-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64b62-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="64b62-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="64b62-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64b62-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64b62-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="64b62-114">Not supported</span></span>|
|<span data-ttu-id="64b62-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64b62-115">Application</span></span>|<span data-ttu-id="64b62-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="64b62-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="64b62-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64b62-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64b62-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64b62-118">Optional query parameters</span></span>
<span data-ttu-id="64b62-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64b62-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="64b62-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="64b62-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="64b62-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64b62-121">Request headers</span></span>
|<span data-ttu-id="64b62-122">Nome</span><span class="sxs-lookup"><span data-stu-id="64b62-122">Name</span></span>|<span data-ttu-id="64b62-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="64b62-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="64b62-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="64b62-124">Authorization</span></span>|<span data-ttu-id="64b62-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64b62-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b62-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64b62-127">Request body</span></span>
<span data-ttu-id="64b62-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64b62-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64b62-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b62-129">Response</span></span>

<span data-ttu-id="64b62-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64b62-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64b62-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="64b62-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="64b62-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64b62-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="64b62-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="64b62-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies
```
# <a name="c"></a>[<span data-ttu-id="64b62-134">C#</span><span class="sxs-lookup"><span data-stu-id="64b62-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64b62-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64b62-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64b62-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64b62-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64b62-137">Java</span><span class="sxs-lookup"><span data-stu-id="64b62-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="64b62-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="64b62-138">Response</span></span>
<span data-ttu-id="64b62-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="64b62-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "displayName": "Policy1",
      "description": "A policy for all privileged administrators",
      "isOrganizationDefault": true,
      "scopeId": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "scopeType": "subscriptions",
      "lastModifiedDateTime": "2021-03-17T02:54:27.167+00:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identity"
      }
    }
  ]
}
```

