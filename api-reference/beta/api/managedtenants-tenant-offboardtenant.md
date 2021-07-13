---
title: 'tenant: offboardTenant'
description: Executa os procedimentos apropriados para remover um locatário gerenciado da plataforma de gerenciamento de vários locatários. Nenhum relacionamento, como o comércio e privilégios administrativos de representante, será afetado. A única alteração feita invocando essa ação é que o locatário será desprovisionado da plataforma de gerenciamento de vários locatários.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: fc7a21323b7f1cd0abfe171eb80cead469d7816b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402121"
---
# <a name="tenant-offboardtenant"></a><span data-ttu-id="f9421-105">tenant: offboardTenant</span><span class="sxs-lookup"><span data-stu-id="f9421-105">tenant: offboardTenant</span></span>
<span data-ttu-id="f9421-106">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f9421-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9421-107">Executa os procedimentos apropriados para remover um locatário gerenciado da plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="f9421-107">Carries out the appropriate procedures to remove a managed tenant from the multi-tenant management platform.</span></span> <span data-ttu-id="f9421-108">Nenhum relacionamento, como o comércio e privilégios administrativos de representante, será afetado.</span><span class="sxs-lookup"><span data-stu-id="f9421-108">No relationships, such as commerce and delegate administrative privileges, will be impacted.</span></span> <span data-ttu-id="f9421-109">A única alteração feita invocando essa ação é que o locatário será desprovisionado da plataforma de gerenciamento de vários locatários.</span><span class="sxs-lookup"><span data-stu-id="f9421-109">The only change made by invoking this action is the tenant will be deprovisioned from the multi-tenant management platform.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9421-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9421-110">Permissions</span></span>
<span data-ttu-id="f9421-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9421-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9421-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9421-113">Permission type</span></span>|<span data-ttu-id="f9421-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9421-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9421-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9421-115">Delegated (work or school account)</span></span>|<span data-ttu-id="f9421-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9421-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="f9421-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9421-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9421-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9421-118">Not supported.</span></span>|
|<span data-ttu-id="f9421-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9421-119">Application</span></span>|<span data-ttu-id="f9421-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9421-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9421-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9421-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```

## <a name="request-headers"></a><span data-ttu-id="f9421-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9421-122">Request headers</span></span>
|<span data-ttu-id="f9421-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f9421-123">Name</span></span>|<span data-ttu-id="f9421-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9421-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f9421-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9421-125">Authorization</span></span>|<span data-ttu-id="f9421-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f9421-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9421-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9421-128">Request body</span></span>
<span data-ttu-id="f9421-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9421-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9421-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9421-130">Response</span></span>

<span data-ttu-id="f9421-131">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um [locatário](../resources/managedtenants-tenant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9421-131">If successful, this action returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f9421-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f9421-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f9421-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9421-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenant_offboardtenant"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}/offboardTenant
```

### <a name="response"></a><span data-ttu-id="f9421-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9421-134">Response</span></span>
><span data-ttu-id="f9421-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f9421-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
