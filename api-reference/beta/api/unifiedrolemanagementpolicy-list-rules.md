---
title: Listar regras
description: Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação de regras.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4a9f37cc806f3afec446e826e43f90a43d626b8
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299023"
---
# <a name="list-rules"></a><span data-ttu-id="7179e-103">Listar regras</span><span class="sxs-lookup"><span data-stu-id="7179e-103">List rules</span></span>
<span data-ttu-id="7179e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7179e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7179e-105">Obter os recursos unifiedRoleManagementPolicyRule da propriedade de navegação de regras.</span><span class="sxs-lookup"><span data-stu-id="7179e-105">Get the unifiedRoleManagementPolicyRule resources from the rules navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="7179e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7179e-106">Permissions</span></span>
<span data-ttu-id="7179e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7179e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7179e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7179e-109">Permission type</span></span>|<span data-ttu-id="7179e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7179e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7179e-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7179e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7179e-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7179e-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="7179e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7179e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7179e-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7179e-114">Not supported</span></span>|
|<span data-ttu-id="7179e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7179e-115">Application</span></span>|<span data-ttu-id="7179e-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7179e-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="7179e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7179e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7179e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7179e-118">Optional query parameters</span></span>
<span data-ttu-id="7179e-119">Este método dá suporte a todos os parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7179e-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7179e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7179e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7179e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7179e-121">Request headers</span></span>
|<span data-ttu-id="7179e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7179e-122">Name</span></span>|<span data-ttu-id="7179e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7179e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7179e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7179e-124">Authorization</span></span>|<span data-ttu-id="7179e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7179e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7179e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7179e-127">Request body</span></span>
<span data-ttu-id="7179e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7179e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7179e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7179e-129">Response</span></span>

<span data-ttu-id="7179e-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7179e-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7179e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7179e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7179e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7179e-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/rules
```


### <a name="response"></a><span data-ttu-id="7179e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7179e-133">Response</span></span>
<span data-ttu-id="7179e-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7179e-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyRule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
      "target": {
        "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
      }
    }
  ]
}
```

