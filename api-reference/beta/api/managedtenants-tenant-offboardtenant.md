---
title: 'tenant: offboardTenant'
description: Executa os procedimentos apropriados para remover um locatário gerenciado da plataforma de gerenciamento de vários locatários. Nenhum relacionamento, como o comércio e privilégios administrativos de representante, será afetado. A única alteração feita invocando essa ação é que o locatário será desprovisionado da plataforma de gerenciamento de vários locatários.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: d6d4d07c7af19299e679275354206bc55da3ffdb
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442467"
---
# <a name="tenant-offboardtenant"></a><span data-ttu-id="8b5fe-105">tenant: offboardTenant</span><span class="sxs-lookup"><span data-stu-id="8b5fe-105">tenant: offboardTenant</span></span>
<span data-ttu-id="8b5fe-106">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8b5fe-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b5fe-107">Executa os procedimentos apropriados para remover um locatário gerenciado da plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-107">Carries out the appropriate procedures to remove a managed tenant from the multi-tenant management platform.</span></span> <span data-ttu-id="8b5fe-108">Nenhum relacionamento, como o comércio e privilégios administrativos de representante, será afetado.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-108">No relationships, such as commerce and delegate administrative privileges, will be impacted.</span></span> <span data-ttu-id="8b5fe-109">A única alteração feita invocando essa ação é que o locatário será desprovisionado da plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-109">The only change made by invoking this action is the tenant will be deprovisioned from the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b5fe-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b5fe-110">Permissions</span></span>
<span data-ttu-id="8b5fe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b5fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b5fe-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b5fe-113">Permission type</span></span>|<span data-ttu-id="8b5fe-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b5fe-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b5fe-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b5fe-115">Delegated (work or school account)</span></span>|<span data-ttu-id="8b5fe-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b5fe-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="8b5fe-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b5fe-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b5fe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-118">Not supported.</span></span>|
|<span data-ttu-id="8b5fe-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b5fe-119">Application</span></span>|<span data-ttu-id="8b5fe-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b5fe-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b5fe-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```

## <a name="request-headers"></a><span data-ttu-id="8b5fe-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b5fe-122">Request headers</span></span>
|<span data-ttu-id="8b5fe-123">Nome</span><span class="sxs-lookup"><span data-stu-id="8b5fe-123">Name</span></span>|<span data-ttu-id="8b5fe-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b5fe-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8b5fe-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b5fe-125">Authorization</span></span>|<span data-ttu-id="8b5fe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b5fe-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b5fe-128">Request body</span></span>
<span data-ttu-id="8b5fe-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b5fe-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b5fe-130">Response</span></span>

<span data-ttu-id="8b5fe-131">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um [locatário](../resources/managedtenants-tenant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-131">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b5fe-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8b5fe-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b5fe-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b5fe-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8b5fe-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b5fe-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenant_offboardtenant"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```
# <a name="c"></a>[<span data-ttu-id="8b5fe-135">C#</span><span class="sxs-lookup"><span data-stu-id="8b5fe-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenant-offboardtenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b5fe-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b5fe-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenant-offboardtenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b5fe-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b5fe-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenant-offboardtenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b5fe-138">Java</span><span class="sxs-lookup"><span data-stu-id="8b5fe-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenant-offboardtenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b5fe-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b5fe-139">Response</span></span>
><span data-ttu-id="8b5fe-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b5fe-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenant"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.managedTenants.tenant",
    "id": "String (identifier)",
    "tenantId": "String",
    "displayName": "String",
    "contract": {
      "@odata.type": "microsoft.graph.managedTenants.tenantContract"
    },
    "tenantStatusInformation": {
      "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
    },
    "lastUpdatedDateTime": "String (timestamp)",
    "createdDateTime": "String (timestamp)"
  }
}
```
