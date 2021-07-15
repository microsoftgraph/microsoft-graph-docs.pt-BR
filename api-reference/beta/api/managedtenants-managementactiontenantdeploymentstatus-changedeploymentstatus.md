---
title: 'managementActionTenantDeploymentStatus: changeDeploymentStatus'
description: Altera o status de implantação de nível de locatário para a ação de gerenciamento. Essas informações são usadas para fornecer informações sobre quais ações de gerenciamento estão em um estado específico. Como exemplo, pode haver um plano para aplicar a autenticação multifator necessária para administradores, portanto, seria ideal alterar o status para planejado para refletir o status apropriado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 572ee7f6c6769ec500c47edee5d35dd18fe75d3f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440901"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a><span data-ttu-id="46e44-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="46e44-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span></span>
<span data-ttu-id="46e44-106">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="46e44-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46e44-107">Altera o status de implantação de nível de locatário para a ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46e44-107">Changes the tenant level deployment status for the management action.</span></span> <span data-ttu-id="46e44-108">Essas informações são usadas para fornecer informações sobre quais ações de gerenciamento estão em um estado específico.</span><span class="sxs-lookup"><span data-stu-id="46e44-108">This information is used to provide insights into what management actions are in a specific state.</span></span> <span data-ttu-id="46e44-109">Como exemplo, pode haver um plano para aplicar a autenticação multifator necessária para administradores, portanto, seria ideal alterar o status para planejado para refletir o status apropriado.</span><span class="sxs-lookup"><span data-stu-id="46e44-109">As example there might be a plan to apply the require multi-factor authentication for admins, so it would be ideal to change the status to planned to reflect the appropriate status.</span></span>

## <a name="permissions"></a><span data-ttu-id="46e44-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="46e44-110">Permissions</span></span>
<span data-ttu-id="46e44-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46e44-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46e44-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46e44-113">Permission type</span></span>|<span data-ttu-id="46e44-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46e44-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46e44-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46e44-115">Delegated (work or school account)</span></span>|<span data-ttu-id="46e44-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e44-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="46e44-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46e44-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46e44-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46e44-118">Not supported.</span></span>|
|<span data-ttu-id="46e44-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46e44-119">Application</span></span>|<span data-ttu-id="46e44-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46e44-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46e44-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46e44-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
```

## <a name="request-headers"></a><span data-ttu-id="46e44-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46e44-122">Request headers</span></span>
|<span data-ttu-id="46e44-123">Nome</span><span class="sxs-lookup"><span data-stu-id="46e44-123">Name</span></span>|<span data-ttu-id="46e44-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e44-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46e44-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="46e44-125">Authorization</span></span>|<span data-ttu-id="46e44-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46e44-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="46e44-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46e44-128">Content-Type</span></span>|<span data-ttu-id="46e44-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46e44-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46e44-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46e44-131">Request body</span></span>
<span data-ttu-id="46e44-132">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="46e44-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="46e44-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="46e44-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="46e44-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="46e44-134">Parameter</span></span>|<span data-ttu-id="46e44-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="46e44-135">Type</span></span>|<span data-ttu-id="46e44-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="46e44-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46e44-137">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="46e44-137">tenantGroupId</span></span>|<span data-ttu-id="46e44-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e44-138">String</span></span>|<span data-ttu-id="46e44-139">O identificador do grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="46e44-139">The identifier for the tenant group.</span></span>|
|<span data-ttu-id="46e44-140">tenantId</span><span class="sxs-lookup"><span data-stu-id="46e44-140">tenantId</span></span>|<span data-ttu-id="46e44-141">String</span><span class="sxs-lookup"><span data-stu-id="46e44-141">String</span></span>|<span data-ttu-id="46e44-142">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="46e44-142">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="46e44-143">managementActionId</span><span class="sxs-lookup"><span data-stu-id="46e44-143">managementActionId</span></span>|<span data-ttu-id="46e44-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e44-144">String</span></span>|<span data-ttu-id="46e44-145">O identificador da ação [de gerenciamento](../resources/managedtenants-managementaction.md).</span><span class="sxs-lookup"><span data-stu-id="46e44-145">The identifier for the [management action](../resources/managedtenants-managementaction.md).</span></span>|
|<span data-ttu-id="46e44-146">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="46e44-146">managementTemplateId</span></span>|<span data-ttu-id="46e44-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e44-147">String</span></span>|<span data-ttu-id="46e44-148">O identificador do modelo [de gerenciamento](../resources/managedtenants-managementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="46e44-148">The identifier for the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|
|<span data-ttu-id="46e44-149">status</span><span class="sxs-lookup"><span data-stu-id="46e44-149">status</span></span>|<span data-ttu-id="46e44-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46e44-150">String</span></span>|<span data-ttu-id="46e44-151">O novo status para a [implantação do](../resources/managedtenants-managementaction.md) locatário de ações de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="46e44-151">The new status for the [management action](../resources/managedtenants-managementaction.md) tenant deployment.</span></span>|

## <a name="response"></a><span data-ttu-id="46e44-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e44-152">Response</span></span>

<span data-ttu-id="46e44-153">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46e44-153">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46e44-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46e44-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46e44-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46e44-155">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="46e44-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="46e44-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "managementactiontenantdeploymentstatus_changedeploymentstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
Content-Type: application/json
Content-length: 153

{
  "tenantGroupId": "String",
  "tenantId": "String",
  "managementActionId": "String",
  "managementTemplateId": "String",
  "status": "String"
}
```
# <a name="c"></a>[<span data-ttu-id="46e44-157">C#</span><span class="sxs-lookup"><span data-stu-id="46e44-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/managementactiontenantdeploymentstatus-changedeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46e44-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46e44-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/managementactiontenantdeploymentstatus-changedeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46e44-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46e44-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/managementactiontenantdeploymentstatus-changedeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46e44-160">Java</span><span class="sxs-lookup"><span data-stu-id="46e44-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/managementactiontenantdeploymentstatus-changedeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46e44-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e44-161">Response</span></span>
><span data-ttu-id="46e44-162">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="46e44-162">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.managedTenants.ManagementActionDeploymentStatus",
  "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
  "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
  "status": "planned",
  "workloadActionDeploymentStatuses": []
}
```
