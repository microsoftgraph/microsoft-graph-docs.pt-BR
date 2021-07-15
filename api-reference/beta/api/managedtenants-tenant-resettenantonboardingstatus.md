---
title: 'locatário: resetTenantOnboardingStatus'
description: Executa os procedimentos apropriados para redefinir o status de integração do locatário gerenciado que foi removido da plataforma de gerenciamento de vários locatários usando a ação offboardTenant. Ao invocar essa ação, a plataforma tentará integrar o locatário gerenciado para gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e7d584343475f5f1698b4bccde13a0f1115abf43
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440397"
---
# <a name="tenant-resettenantonboardingstatus"></a><span data-ttu-id="24012-104">locatário: resetTenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="24012-104">tenant: resetTenantOnboardingStatus</span></span>
<span data-ttu-id="24012-105">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="24012-105">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24012-106">Executa os procedimentos apropriados para redefinir o status de integração do locatário gerenciado que foi removido da plataforma de gerenciamento de vários locatários usando a [ação offboardTenant.](../api/managedtenants-tenant-offboardtenant.md)</span><span class="sxs-lookup"><span data-stu-id="24012-106">Carries out the appropriate procedures to reset the onboarding status for the managed tenant that was removed from the multi-tenant management platform using the [offboardTenant](../api/managedtenants-tenant-offboardtenant.md) action.</span></span> <span data-ttu-id="24012-107">Ao invocar essa ação, a plataforma tentará integrar o locatário gerenciado para gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="24012-107">By invoking this action the platform will attempt to onboard the managed tenant for management.</span></span>

## <a name="permissions"></a><span data-ttu-id="24012-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="24012-108">Permissions</span></span>
<span data-ttu-id="24012-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24012-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24012-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24012-111">Permission type</span></span>|<span data-ttu-id="24012-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24012-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24012-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24012-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24012-114">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24012-114">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="24012-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24012-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24012-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24012-116">Not supported.</span></span>|
|<span data-ttu-id="24012-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24012-117">Application</span></span>|<span data-ttu-id="24012-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24012-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24012-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24012-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus
```

## <a name="request-headers"></a><span data-ttu-id="24012-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24012-120">Request headers</span></span>
|<span data-ttu-id="24012-121">Nome</span><span class="sxs-lookup"><span data-stu-id="24012-121">Name</span></span>|<span data-ttu-id="24012-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="24012-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24012-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24012-123">Authorization</span></span>|<span data-ttu-id="24012-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24012-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24012-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24012-126">Request body</span></span>
<span data-ttu-id="24012-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24012-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24012-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="24012-128">Response</span></span>

<span data-ttu-id="24012-129">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um [locatário](../resources/managedtenants-tenant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24012-129">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24012-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24012-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24012-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24012-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="24012-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="24012-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenant_resettenantonboardingstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus
```
# <a name="c"></a>[<span data-ttu-id="24012-133">C#</span><span class="sxs-lookup"><span data-stu-id="24012-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenant-resettenantonboardingstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24012-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24012-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenant-resettenantonboardingstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24012-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24012-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenant-resettenantonboardingstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24012-136">Java</span><span class="sxs-lookup"><span data-stu-id="24012-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenant-resettenantonboardingstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24012-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="24012-137">Response</span></span>
><span data-ttu-id="24012-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24012-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "contract": {
    "displayName": "Fourth Coffee",
    "defaultDomainName": "fourthcoffe001.onmicrosoft.com",
    "contractType": 2
  },
  "tenantStatusInformation": {
    "onboardingStatus": "inactive",
    "onboardingDateTime": "2012-02-20T00:00:00Z",
    "onboardedByUserId": "",
    "offboardedDateTime": "2012-02-20T00:00:00Z",
    "offboardedBy": "",
    "delegatedPrivilegeStatus": "delegatedAdminPrivileges",
    "workloadStatuses": []
  },
  "createdDateTime": "2012-02-20T00:00:00Z",
  "lastUpdatedDatetime": "2021-02-20T00:00:00Z"
}
```
