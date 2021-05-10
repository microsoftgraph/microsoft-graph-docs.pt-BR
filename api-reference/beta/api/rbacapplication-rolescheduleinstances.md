---
title: 'rbacApplication: roleScheduleInstances'
description: Recupere tanto roleAssignmentScheduleInstances quanto roleEligibilityScheduleInstances.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a80fa4beec6996cf390b2a4d96e4a919409ca036
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299038"
---
# <a name="rbacapplication-rolescheduleinstances"></a><span data-ttu-id="bb5ac-103">rbacApplication: roleScheduleInstances</span><span class="sxs-lookup"><span data-stu-id="bb5ac-103">rbacApplication: roleScheduleInstances</span></span>
<span data-ttu-id="bb5ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb5ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb5ac-105">Recupere tanto roleAssignmentScheduleInstances quanto roleEligibilityScheduleInstances.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-105">Retrieve both roleAssignmentScheduleInstances and roleEligibilityScheduleInstances.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb5ac-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb5ac-106">Permissions</span></span>
<span data-ttu-id="bb5ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb5ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb5ac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb5ac-109">Permission type</span></span>|<span data-ttu-id="bb5ac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb5ac-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb5ac-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb5ac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb5ac-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="bb5ac-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="bb5ac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb5ac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb5ac-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bb5ac-114">Not supported</span></span>|
|<span data-ttu-id="bb5ac-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb5ac-115">Application</span></span>|<span data-ttu-id="bb5ac-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="bb5ac-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb5ac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb5ac-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleScheduleInstances
```

## <a name="query-parameters"></a><span data-ttu-id="bb5ac-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="bb5ac-118">Query parameters</span></span>
<span data-ttu-id="bb5ac-119">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-119">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="bb5ac-120">A tabela a seguir mostra os parâmetros de consulta que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-120">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="bb5ac-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bb5ac-121">Parameter</span></span>|<span data-ttu-id="bb5ac-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb5ac-122">Type</span></span>|<span data-ttu-id="bb5ac-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb5ac-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb5ac-124">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="bb5ac-124">directoryScopeId</span></span>|<span data-ttu-id="bb5ac-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb5ac-125">String</span></span>|<span data-ttu-id="bb5ac-126">ID do objeto directory que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-126">Id of the directory object that represents the scope of the assignment.</span></span> <span data-ttu-id="bb5ac-127">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-127">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="bb5ac-128">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-128">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="bb5ac-129">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-129">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="bb5ac-130">appScopeId</span><span class="sxs-lookup"><span data-stu-id="bb5ac-130">appScopeId</span></span>|<span data-ttu-id="bb5ac-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb5ac-131">String</span></span>|<span data-ttu-id="bb5ac-132">ID do escopo específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-132">Id of the app specific scope.</span></span> <span data-ttu-id="bb5ac-133">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-133">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="bb5ac-134">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-134">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="bb5ac-135">Use "/" para o escopo de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-135">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="bb5ac-136">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-136">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="bb5ac-137">principalId</span><span class="sxs-lookup"><span data-stu-id="bb5ac-137">principalId</span></span>|<span data-ttu-id="bb5ac-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb5ac-138">String</span></span>|<span data-ttu-id="bb5ac-139">Objectid da entidade à qual os agendamentos pertencem.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-139">Objectid of the principal to which the schedules belong.</span></span> |
|<span data-ttu-id="bb5ac-140">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="bb5ac-140">roleDefinitionId</span></span>|<span data-ttu-id="bb5ac-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bb5ac-141">String</span></span>|<span data-ttu-id="bb5ac-142">ID do unifiedRoleDefinition para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-142">ID of the unifiedRoleDefinition for the assignment.</span></span> <span data-ttu-id="bb5ac-143">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-143">Read only.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="bb5ac-144">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5ac-144">Request headers</span></span>
|<span data-ttu-id="bb5ac-145">Nome</span><span class="sxs-lookup"><span data-stu-id="bb5ac-145">Name</span></span>|<span data-ttu-id="bb5ac-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb5ac-146">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bb5ac-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb5ac-147">Authorization</span></span>|<span data-ttu-id="bb5ac-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb5ac-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5ac-150">Request body</span></span>
<span data-ttu-id="bb5ac-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb5ac-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5ac-152">Response</span></span>

<span data-ttu-id="bb5ac-153">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-153">If successful, this method returns a `200 OK` response code and a [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb5ac-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bb5ac-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb5ac-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb5ac-155">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "rbacapplication_rolescheduleinstances"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleScheduleInstances(directoryScopeId='parameterValue',appScopeId='parameterValue',principalId='parameterValue',roleDefinitionId='parameterValue')
```


### <a name="response"></a><span data-ttu-id="bb5ac-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb5ac-156">Response</span></span>
<span data-ttu-id="bb5ac-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bb5ac-157">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleScheduleInstanceBase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleScheduleInstanceBase",
      "id": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "principalId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "roleDefinitionId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "directoryScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "appScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea"
    }
  ]
}
```
