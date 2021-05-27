---
title: 'rbacApplication: roleSchedules'
description: Recupere tanto roleAssignmentSchedules quanto roleEligibilitySchedules.
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 415d7a5565ff4f35b55f003726d24cfe589b472e
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680121"
---
# <a name="rbacapplication-roleschedules"></a><span data-ttu-id="9e33d-103">rbacApplication: roleSchedules</span><span class="sxs-lookup"><span data-stu-id="9e33d-103">rbacApplication: roleSchedules</span></span>
<span data-ttu-id="9e33d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e33d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e33d-105">Recupere tanto roleAssignmentSchedules quanto roleEligibilitySchedules.</span><span class="sxs-lookup"><span data-stu-id="9e33d-105">Retrieve both roleAssignmentSchedules and roleEligibilitySchedules.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e33d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e33d-106">Permissions</span></span>
<span data-ttu-id="9e33d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e33d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e33d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e33d-109">Permission type</span></span>|<span data-ttu-id="9e33d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e33d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e33d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e33d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e33d-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="9e33d-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="9e33d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e33d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e33d-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9e33d-114">Not supported</span></span>|
|<span data-ttu-id="9e33d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e33d-115">Application</span></span>|<span data-ttu-id="9e33d-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="9e33d-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e33d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e33d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /roleManagement/directory/roleSchedules
```

## <a name="function-parameters"></a><span data-ttu-id="9e33d-118">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="9e33d-118">Function parameters</span></span>
<span data-ttu-id="9e33d-119">A tabela a seguir mostra os parâmetros de consulta que podem ser usados com esse método.</span><span class="sxs-lookup"><span data-stu-id="9e33d-119">The following table shows the query parameters that can be used with this method.</span></span>

|<span data-ttu-id="9e33d-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9e33d-120">Parameter</span></span>|<span data-ttu-id="9e33d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e33d-121">Type</span></span>|<span data-ttu-id="9e33d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e33d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e33d-123">directoryScopeId</span><span class="sxs-lookup"><span data-stu-id="9e33d-123">directoryScopeId</span></span>|<span data-ttu-id="9e33d-124">String</span><span class="sxs-lookup"><span data-stu-id="9e33d-124">String</span></span>|<span data-ttu-id="9e33d-125">ID do objeto directory que representa o escopo da atribuição.</span><span class="sxs-lookup"><span data-stu-id="9e33d-125">Id of the directory object that represents the scope of the assignment.</span></span> <span data-ttu-id="9e33d-126">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="9e33d-126">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="9e33d-127">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9e33d-127">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="9e33d-128">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e33d-128">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="9e33d-129">appScopeId</span><span class="sxs-lookup"><span data-stu-id="9e33d-129">appScopeId</span></span>|<span data-ttu-id="9e33d-130">String</span><span class="sxs-lookup"><span data-stu-id="9e33d-130">String</span></span>|<span data-ttu-id="9e33d-131">ID do escopo específico do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e33d-131">Id of the app specific scope.</span></span> <span data-ttu-id="9e33d-132">O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso.</span><span class="sxs-lookup"><span data-stu-id="9e33d-132">The scope of an assignment determines the set of resources for which the principal has been granted access.</span></span> <span data-ttu-id="9e33d-133">Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos.</span><span class="sxs-lookup"><span data-stu-id="9e33d-133">Directory scopes are shared scopes stored in the directory that are understood by multiple applications.</span></span> <span data-ttu-id="9e33d-134">Use "/" para o escopo de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="9e33d-134">Use "/" for tenant-wide scope.</span></span> <span data-ttu-id="9e33d-135">Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e33d-135">App scopes are scopes that are defined and understood by this application only.</span></span> |
|<span data-ttu-id="9e33d-136">principalId</span><span class="sxs-lookup"><span data-stu-id="9e33d-136">principalId</span></span>|<span data-ttu-id="9e33d-137">String</span><span class="sxs-lookup"><span data-stu-id="9e33d-137">String</span></span>|<span data-ttu-id="9e33d-138">Objectid da entidade à qual os agendamentos pertencem.</span><span class="sxs-lookup"><span data-stu-id="9e33d-138">Objectid of the principal to which the schedules belong.</span></span> |
|<span data-ttu-id="9e33d-139">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="9e33d-139">roleDefinitionId</span></span>|<span data-ttu-id="9e33d-140">String</span><span class="sxs-lookup"><span data-stu-id="9e33d-140">String</span></span>|<span data-ttu-id="9e33d-141">ID do unifiedRoleDefinition para a atribuição.</span><span class="sxs-lookup"><span data-stu-id="9e33d-141">ID of the unifiedRoleDefinition for the assignment.</span></span> <span data-ttu-id="9e33d-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9e33d-142">Read only.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="9e33d-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e33d-143">Request headers</span></span>
|<span data-ttu-id="9e33d-144">Nome</span><span class="sxs-lookup"><span data-stu-id="9e33d-144">Name</span></span>|<span data-ttu-id="9e33d-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e33d-145">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9e33d-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e33d-146">Authorization</span></span>|<span data-ttu-id="9e33d-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e33d-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e33d-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e33d-149">Request body</span></span>
<span data-ttu-id="9e33d-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e33d-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e33d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e33d-151">Response</span></span>

<span data-ttu-id="9e33d-152">Se tiver êxito, este método retornará um código de resposta e uma coleção `200 OK` [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e33d-152">If successful, this method returns a `200 OK` response code and a [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e33d-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9e33d-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e33d-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e33d-154">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9e33d-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e33d-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "rbacapplication_roleschedules"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleSchedules(directoryScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',appScopeId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',principalId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea',roleDefinitionId='a3bb8764-cb92-4276-9d2a-ca1e895e55ea')
```
# <a name="c"></a>[<span data-ttu-id="9e33d-156">C#</span><span class="sxs-lookup"><span data-stu-id="9e33d-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rbacapplication-roleschedules-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e33d-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e33d-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rbacapplication-roleschedules-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e33d-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e33d-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rbacapplication-roleschedules-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9e33d-159">Java</span><span class="sxs-lookup"><span data-stu-id="9e33d-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/rbacapplication-roleschedules-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9e33d-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e33d-160">Response</span></span>
<span data-ttu-id="9e33d-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9e33d-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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
