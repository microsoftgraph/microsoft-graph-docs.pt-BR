---
title: 'rbacApplication: roleSchedules'
description: Recupere tanto roleAssignmentSchedules quanto roleEligibilitySchedules.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb226f2b8e116b57e8514b642ecd46d0b4c9bde4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299037"
---
# <a name="rbacapplication-roleschedules"></a><span data-ttu-id="183ad-103">rbacApplication: roleSchedules</span><span class="sxs-lookup"><span data-stu-id="183ad-103">rbacApplication: roleSchedules</span></span>
<span data-ttu-id="183ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="183ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="183ad-105">Recupere tanto roleAssignmentSchedules quanto roleEligibilitySchedules.</span><span class="sxs-lookup"><span data-stu-id="183ad-105">Retrieve both roleAssignmentSchedules and roleEligibilitySchedules.</span></span>

## <a name="permissions"></a><span data-ttu-id="183ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="183ad-106">Permissions</span></span>
<span data-ttu-id="183ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="183ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="183ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="183ad-109">Permission type</span></span>|<span data-ttu-id="183ad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="183ad-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="183ad-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="183ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="183ad-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="183ad-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="183ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="183ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="183ad-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="183ad-114">Not supported</span></span>|
|<span data-ttu-id="183ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="183ad-115">Application</span></span>|<span data-ttu-id="183ad-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="183ad-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="183ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="183ad-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleSchedules
```

## <a name="function-parameters"></a><span data-ttu-id="183ad-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="183ad-118">Function parameters</span></span>
<span data-ttu-id="183ad-119">A tabela a seguir mostra os parâmetros de consulta que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="183ad-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="183ad-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="183ad-120">Parameter</span></span>|<span data-ttu-id="183ad-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="183ad-121">Type</span></span>|<span data-ttu-id="183ad-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="183ad-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="183ad-123">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="183ad-123">directoryScopeId</span></span>|<span data-ttu-id="183ad-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="183ad-124">String</span></span>|<span data-ttu-id="183ad-125">ID do objeto directory que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="183ad-125">Id of the directory object that represents the scope of the assignment.</span></span> <span data-ttu-id="183ad-126">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="183ad-126">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="183ad-127">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="183ad-127">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="183ad-128">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="183ad-128">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="183ad-129">appScopeId</span><span class="sxs-lookup"><span data-stu-id="183ad-129">appScopeId</span></span>|<span data-ttu-id="183ad-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="183ad-130">String</span></span>|<span data-ttu-id="183ad-131">ID do escopo específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="183ad-131">Id of the app specific scope.</span></span> <span data-ttu-id="183ad-132">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="183ad-132">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="183ad-133">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="183ad-133">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="183ad-134">Use "/" para o escopo de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="183ad-134">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="183ad-135">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="183ad-135">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="183ad-136">principalId</span><span class="sxs-lookup"><span data-stu-id="183ad-136">principalId</span></span>|<span data-ttu-id="183ad-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="183ad-137">String</span></span>|<span data-ttu-id="183ad-138">Objectid da entidade à qual os agendamentos pertencem.</span><span class="sxs-lookup"><span data-stu-id="183ad-138">Objectid of the principal to which the schedules belong.</span></span> |
|<span data-ttu-id="183ad-139">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="183ad-139">roleDefinitionId</span></span>|<span data-ttu-id="183ad-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="183ad-140">String</span></span>|<span data-ttu-id="183ad-141">ID do unifiedRoleDefinition para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="183ad-141">ID of the unifiedRoleDefinition for the assignment.</span></span> <span data-ttu-id="183ad-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="183ad-142">Read only.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="183ad-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="183ad-143">Request headers</span></span>
|<span data-ttu-id="183ad-144">Nome</span><span class="sxs-lookup"><span data-stu-id="183ad-144">Name</span></span>|<span data-ttu-id="183ad-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="183ad-145">Description</span></span>|
|:---|:---|
|<span data-ttu-id="183ad-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="183ad-146">Authorization</span></span>|<span data-ttu-id="183ad-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="183ad-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="183ad-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="183ad-149">Request body</span></span>
<span data-ttu-id="183ad-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="183ad-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="183ad-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="183ad-151">Response</span></span>

<span data-ttu-id="183ad-152">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="183ad-152">If successful, this method returns a `200 OK` response code and a [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="183ad-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="183ad-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="183ad-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="183ad-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "rbacapplication_roleschedules"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleSchedules(directoryScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',appScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',principalId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',roleDefinitionId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea')
```


### <a name="response"></a><span data-ttu-id="183ad-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="183ad-155">Response</span></span>
<span data-ttu-id="183ad-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="183ad-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleScheduleBase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Identity.Governance.Common.Data.ExternalModels.V1.unifiedRoleScheduleBase",
      "id": "String (identifier)",
      "principalId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "roleDefinitionId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "directoryScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "appScopeId": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "createdUsing": "a3bb8764-cb92-4276-9d2a-ca1e895e55ea",
      "createdDateTime": "2020-09-09T21:32:27.91Z",
      "modifiedDateTime": "2020-09-09T21:32:27.91Z",
      "status": "Provisioned"
    }
  ]
}
```
