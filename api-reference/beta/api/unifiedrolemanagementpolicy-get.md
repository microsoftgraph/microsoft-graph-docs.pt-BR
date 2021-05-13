---
title: Obter unifiedRoleManagementPolicy
description: Leia as propriedades e as relações de um objeto unifiedRoleManagementPolicy.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2136258212faeaaba241e25e7743eaff9e9a6aec
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475055"
---
# <a name="get-unifiedrolemanagementpolicy"></a><span data-ttu-id="10fca-103">Obter unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="10fca-103">Get unifiedRoleManagementPolicy</span></span>
<span data-ttu-id="10fca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10fca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10fca-105">Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicy.](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="10fca-105">Read the properties and relationships of an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="10fca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10fca-106">Permissions</span></span>
<span data-ttu-id="10fca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10fca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10fca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10fca-109">Permission type</span></span>|<span data-ttu-id="10fca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10fca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10fca-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10fca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="10fca-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="10fca-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="10fca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10fca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10fca-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="10fca-114">Not supported</span></span>|
|<span data-ttu-id="10fca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10fca-115">Application</span></span>|<span data-ttu-id="10fca-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="10fca-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="10fca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10fca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10fca-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10fca-118">Optional query parameters</span></span>
<span data-ttu-id="10fca-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="10fca-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="10fca-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="10fca-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="10fca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10fca-121">Request headers</span></span>
|<span data-ttu-id="10fca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="10fca-122">Name</span></span>|<span data-ttu-id="10fca-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="10fca-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="10fca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="10fca-124">Authorization</span></span>|<span data-ttu-id="10fca-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10fca-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="10fca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10fca-127">Request body</span></span>
<span data-ttu-id="10fca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10fca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10fca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="10fca-129">Response</span></span>

<span data-ttu-id="10fca-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10fca-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="10fca-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="10fca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="10fca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10fca-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="10fca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="10fca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/f93a5c37-5c37-f93a-375c-3af9375c3af9
```
# <a name="c"></a>[<span data-ttu-id="10fca-134">C#</span><span class="sxs-lookup"><span data-stu-id="10fca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10fca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10fca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10fca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10fca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="10fca-137">Java</span><span class="sxs-lookup"><span data-stu-id="10fca-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="10fca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="10fca-138">Response</span></span>
<span data-ttu-id="10fca-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10fca-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
    "displayName": "Policy1",
    "description": "Policy for privileged admins",
    "isOrganizationDefault": true,
    "scopeId": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
    "scopeType": "subscription",
    "lastModifiedDateTime": "2020-09-09T21:35:27.91Z",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```

