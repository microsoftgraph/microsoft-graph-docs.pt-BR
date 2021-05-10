---
title: Listar unifiedRoleManagementPolicies
description: Obter uma lista dos objetos unifiedRoleManagementPolicy e suas propriedades.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 809e947965f180fca2bdc0078ff69a64c00960cc
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299021"
---
# <a name="list-unifiedrolemanagementpolicies"></a><span data-ttu-id="d9af2-103">Listar unifiedRoleManagementPolicies</span><span class="sxs-lookup"><span data-stu-id="d9af2-103">List unifiedRoleManagementPolicies</span></span>
<span data-ttu-id="d9af2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9af2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9af2-105">Obter uma lista dos [objetos unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d9af2-105">Get a list of the [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="d9af2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9af2-106">Permissions</span></span>
<span data-ttu-id="d9af2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9af2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9af2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9af2-109">Permission type</span></span>|<span data-ttu-id="d9af2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9af2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9af2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9af2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9af2-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="d9af2-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="d9af2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9af2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9af2-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="d9af2-114">Not supported</span></span>|
|<span data-ttu-id="d9af2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9af2-115">Application</span></span>|<span data-ttu-id="d9af2-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="d9af2-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9af2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9af2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9af2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9af2-118">Optional query parameters</span></span>
<span data-ttu-id="d9af2-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9af2-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d9af2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d9af2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9af2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9af2-121">Request headers</span></span>
|<span data-ttu-id="d9af2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d9af2-122">Name</span></span>|<span data-ttu-id="d9af2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9af2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d9af2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9af2-124">Authorization</span></span>|<span data-ttu-id="d9af2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9af2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9af2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9af2-127">Request body</span></span>
<span data-ttu-id="d9af2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9af2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9af2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9af2-129">Response</span></span>

<span data-ttu-id="d9af2-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9af2-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicy](../resources/unifiedrolemanagementpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9af2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9af2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d9af2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9af2-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies
```


### <a name="response"></a><span data-ttu-id="d9af2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9af2-133">Response</span></span>
<span data-ttu-id="d9af2-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9af2-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "description": "Policy for all privileged admins",
      "isOrganizationDefault": false,
      "scopeId": "f93a5c37-5c37-f93a-375c-3af9375c3af9",
      "scopeType": "subscription",
      "lastModifiedDateTime": "2020-09-09T21:35:27.91Z",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identity"
      }
    }
  ]
}
```

