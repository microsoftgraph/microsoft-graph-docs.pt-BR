---
title: Obter unifiedRoleManagementPolicy
description: Leia as propriedades e as relações de um objeto unifiedRoleManagementPolicy.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c88442960327de7d89d17e32549bc6eefb874db1
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299042"
---
# <a name="get-unifiedrolemanagementpolicy"></a><span data-ttu-id="a0d55-103">Obter unifiedRoleManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="a0d55-103">Get unifiedRoleManagementPolicy</span></span>
<span data-ttu-id="a0d55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0d55-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0d55-105">Leia as propriedades e as relações de [um objeto unifiedRoleManagementPolicy.](../resources/unifiedrolemanagementpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="a0d55-105">Read the properties and relationships of an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0d55-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0d55-106">Permissions</span></span>
<span data-ttu-id="a0d55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0d55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0d55-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0d55-109">Permission type</span></span>|<span data-ttu-id="a0d55-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0d55-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0d55-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0d55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0d55-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a0d55-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="a0d55-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0d55-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0d55-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0d55-114">Not supported</span></span>|
|<span data-ttu-id="a0d55-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0d55-115">Application</span></span>|<span data-ttu-id="a0d55-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a0d55-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0d55-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0d55-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0d55-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0d55-118">Optional query parameters</span></span>
<span data-ttu-id="a0d55-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0d55-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a0d55-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a0d55-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0d55-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d55-121">Request headers</span></span>
|<span data-ttu-id="a0d55-122">Nome</span><span class="sxs-lookup"><span data-stu-id="a0d55-122">Name</span></span>|<span data-ttu-id="a0d55-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0d55-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a0d55-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0d55-124">Authorization</span></span>|<span data-ttu-id="a0d55-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0d55-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0d55-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d55-127">Request body</span></span>
<span data-ttu-id="a0d55-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0d55-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0d55-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d55-129">Response</span></span>

<span data-ttu-id="a0d55-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0d55-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0d55-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a0d55-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a0d55-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0d55-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/f93a5c37-5c37-f93a-375c-3af9375c3af9
```


### <a name="response"></a><span data-ttu-id="a0d55-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0d55-133">Response</span></span>
<span data-ttu-id="a0d55-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a0d55-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

