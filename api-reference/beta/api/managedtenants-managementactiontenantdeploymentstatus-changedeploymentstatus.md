---
title: 'managementActionTenantDeploymentStatus: changeDeploymentStatus'
description: Altera o status de implantação de nível de locatário para a ação de gerenciamento. Essas informações são usadas para fornecer informações sobre quais ações de gerenciamento estão em um estado específico. Como exemplo, pode haver um plano para aplicar a autenticação multifator necessária para administradores, portanto, seria ideal alterar o status para planejado para refletir o status apropriado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 4d8c5acacee4eb31e8d014820466eae69534232f
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402014"
---
# <a name="managementactiontenantdeploymentstatus-changedeploymentstatus"></a><span data-ttu-id="da767-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="da767-105">managementActionTenantDeploymentStatus: changeDeploymentStatus</span></span>
<span data-ttu-id="da767-106">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="da767-106">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da767-107">Altera o status de implantação de nível de locatário para a ação de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="da767-107">Changes the tenant level deployment status for the management action.</span></span> <span data-ttu-id="da767-108">Essas informações são usadas para fornecer informações sobre quais ações de gerenciamento estão em um estado específico.</span><span class="sxs-lookup"><span data-stu-id="da767-108">This information is used to provide insights into what management actions are in a specific state.</span></span> <span data-ttu-id="da767-109">Como exemplo, pode haver um plano para aplicar a autenticação multifator necessária para administradores, portanto, seria ideal alterar o status para planejado para refletir o status apropriado.</span><span class="sxs-lookup"><span data-stu-id="da767-109">As example there might be a plan to apply the require multi-factor authentication for admins, so it would be ideal to change the status to planned to reflect the appropriate status.</span></span>

## <a name="permissions"></a><span data-ttu-id="da767-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="da767-110">Permissions</span></span>
<span data-ttu-id="da767-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da767-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da767-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da767-113">Permission type</span></span>|<span data-ttu-id="da767-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da767-114">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da767-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da767-115">Delegated (work or school account)</span></span>|<span data-ttu-id="da767-116">ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da767-116">ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="da767-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da767-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da767-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da767-118">Not supported.</span></span>|
|<span data-ttu-id="da767-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da767-119">Application</span></span>|<span data-ttu-id="da767-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da767-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da767-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da767-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/changeDeploymentStatus
```

## <a name="request-headers"></a><span data-ttu-id="da767-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da767-122">Request headers</span></span>
|<span data-ttu-id="da767-123">Nome</span><span class="sxs-lookup"><span data-stu-id="da767-123">Name</span></span>|<span data-ttu-id="da767-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="da767-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da767-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="da767-125">Authorization</span></span>|<span data-ttu-id="da767-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da767-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="da767-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da767-128">Content-Type</span></span>|<span data-ttu-id="da767-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da767-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da767-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da767-131">Request body</span></span>
<span data-ttu-id="da767-132">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="da767-132">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="da767-133">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="da767-133">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="da767-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="da767-134">Parameter</span></span>|<span data-ttu-id="da767-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="da767-135">Type</span></span>|<span data-ttu-id="da767-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="da767-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da767-137">tenantGroupId</span><span class="sxs-lookup"><span data-stu-id="da767-137">tenantGroupId</span></span>|<span data-ttu-id="da767-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da767-138">String</span></span>|<span data-ttu-id="da767-139">O identificador do grupo de locatários.</span><span class="sxs-lookup"><span data-stu-id="da767-139">The identifier for the tenant group.</span></span>|
|<span data-ttu-id="da767-140">tenantId</span><span class="sxs-lookup"><span data-stu-id="da767-140">tenantId</span></span>|<span data-ttu-id="da767-141">String</span><span class="sxs-lookup"><span data-stu-id="da767-141">String</span></span>|<span data-ttu-id="da767-142">O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="da767-142">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|
|<span data-ttu-id="da767-143">managementActionId</span><span class="sxs-lookup"><span data-stu-id="da767-143">managementActionId</span></span>|<span data-ttu-id="da767-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da767-144">String</span></span>|<span data-ttu-id="da767-145">O identificador da ação [de gerenciamento](../resources/managedtenants-managementaction.md).</span><span class="sxs-lookup"><span data-stu-id="da767-145">The identifier for the [management action](../resources/managedtenants-managementaction.md).</span></span>|
|<span data-ttu-id="da767-146">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="da767-146">managementTemplateId</span></span>|<span data-ttu-id="da767-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da767-147">String</span></span>|<span data-ttu-id="da767-148">O identificador do modelo [de gerenciamento](../resources/managedtenants-managementtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="da767-148">The identifier for the [management template](../resources/managedtenants-managementtemplate.md).</span></span>|
|<span data-ttu-id="da767-149">status</span><span class="sxs-lookup"><span data-stu-id="da767-149">status</span></span>|<span data-ttu-id="da767-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da767-150">String</span></span>|<span data-ttu-id="da767-151">O novo status para a [implantação do](../resources/managedtenants-managementaction.md) locatário de ações de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="da767-151">The new status for the [management action](../resources/managedtenants-managementaction.md) tenant deployment.</span></span>|

## <a name="response"></a><span data-ttu-id="da767-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="da767-152">Response</span></span>

<span data-ttu-id="da767-153">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da767-153">If successful, this action returns a `200 OK` response code and a [managementActionDeploymentStatus](../resources/managedtenants-managementactiondeploymentstatus.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da767-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="da767-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da767-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da767-155">Request</span></span>
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

### <a name="response"></a><span data-ttu-id="da767-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="da767-156">Response</span></span>
><span data-ttu-id="da767-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="da767-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
