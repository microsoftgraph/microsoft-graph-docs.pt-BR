---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação que você deseja em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 4883fedc71cfdcc6c50ab87b46299fdb173552a5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950742"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="8b26e-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="8b26e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b26e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b26e-106">Crie uma solicitação de atribuição de função para representar a operação que você deseja em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="8b26e-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="8b26e-107">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="8b26e-107">The following table lists the operations.</span></span>

| <span data-ttu-id="8b26e-108">Operation</span><span class="sxs-lookup"><span data-stu-id="8b26e-108">Operation</span></span>                                   | <span data-ttu-id="8b26e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="8b26e-110">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="8b26e-110">Assign a role assignment</span></span>                    | <span data-ttu-id="8b26e-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="8b26e-111">AdminAdd</span></span>    |
| <span data-ttu-id="8b26e-112">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="8b26e-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="8b26e-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="8b26e-113">UserAdd</span></span>     |
| <span data-ttu-id="8b26e-114">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="8b26e-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="8b26e-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="8b26e-115">UserRemove</span></span>  |
| <span data-ttu-id="8b26e-116">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="8b26e-116">Remove a role assignment</span></span>                    | <span data-ttu-id="8b26e-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="8b26e-117">AdminRemove</span></span> |
| <span data-ttu-id="8b26e-118">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="8b26e-118">Update a role assignment</span></span>                    | <span data-ttu-id="8b26e-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="8b26e-119">AdminUpdate</span></span> |
| <span data-ttu-id="8b26e-120">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="8b26e-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="8b26e-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="8b26e-121">UserExtend</span></span>  |
| <span data-ttu-id="8b26e-122">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="8b26e-122">Extend a role assignment</span></span>                    | <span data-ttu-id="8b26e-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="8b26e-123">AdminExtend</span></span> |
| <span data-ttu-id="8b26e-124">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="8b26e-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="8b26e-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="8b26e-125">UserRenew</span></span>   |
| <span data-ttu-id="8b26e-126">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="8b26e-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="8b26e-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="8b26e-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="8b26e-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b26e-128">Permissions</span></span>

<span data-ttu-id="8b26e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="8b26e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="8b26e-131">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="8b26e-131">Azure resources</span></span>

| <span data-ttu-id="8b26e-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b26e-132">Permission type</span></span> | <span data-ttu-id="8b26e-133">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b26e-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8b26e-134">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b26e-134">Delegated (work or school account)</span></span> | <span data-ttu-id="8b26e-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="8b26e-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="8b26e-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b26e-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b26e-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b26e-137">Not supported.</span></span> |
| <span data-ttu-id="8b26e-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b26e-138">Application</span></span> | <span data-ttu-id="8b26e-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b26e-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="8b26e-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="8b26e-140">Azure AD</span></span>

| <span data-ttu-id="8b26e-141">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b26e-141">Permission type</span></span> | <span data-ttu-id="8b26e-142">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b26e-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="8b26e-143">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b26e-143">Delegated (work or school account)</span></span> | <span data-ttu-id="8b26e-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="8b26e-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="8b26e-145">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b26e-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b26e-146">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b26e-146">Not supported.</span></span> |
| <span data-ttu-id="8b26e-147">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b26e-147">Application</span></span> | <span data-ttu-id="8b26e-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b26e-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="8b26e-149">Grupos</span><span class="sxs-lookup"><span data-stu-id="8b26e-149">Groups</span></span>

|<span data-ttu-id="8b26e-150">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b26e-150">Permission type</span></span> | <span data-ttu-id="8b26e-151">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b26e-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="8b26e-152">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b26e-152">Delegated (work or school account)</span></span> | <span data-ttu-id="8b26e-153">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="8b26e-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="8b26e-154">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b26e-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b26e-155">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b26e-155">Not supported.</span></span> |
| <span data-ttu-id="8b26e-156">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b26e-156">Application</span></span> | <span data-ttu-id="8b26e-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b26e-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b26e-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b26e-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="8b26e-159">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b26e-159">Request headers</span></span>

| <span data-ttu-id="8b26e-160">Nome</span><span class="sxs-lookup"><span data-stu-id="8b26e-160">Name</span></span>          | <span data-ttu-id="8b26e-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b26e-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="8b26e-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b26e-162">Authorization</span></span> | <span data-ttu-id="8b26e-163">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8b26e-163">Bearer {code}</span></span>    |
| <span data-ttu-id="8b26e-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="8b26e-164">Content-type</span></span>  | <span data-ttu-id="8b26e-165">application/json</span><span class="sxs-lookup"><span data-stu-id="8b26e-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b26e-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b26e-166">Request body</span></span>

<span data-ttu-id="8b26e-167">No corpo da solicitação, fornece uma representação JSON de um [objeto governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8b26e-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="8b26e-168">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b26e-168">Property</span></span>         | <span data-ttu-id="8b26e-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-169">Type</span></span>                                                     | <span data-ttu-id="8b26e-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b26e-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="8b26e-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="8b26e-171">resourceId</span></span>       | <span data-ttu-id="8b26e-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-172">String</span></span>                                                   | <span data-ttu-id="8b26e-173">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b26e-173">The ID of the resource.</span></span> <span data-ttu-id="8b26e-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b26e-174">Required.</span></span> |
| <span data-ttu-id="8b26e-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8b26e-175">roleDefinitionId</span></span> | <span data-ttu-id="8b26e-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-176">String</span></span>                                                   | <span data-ttu-id="8b26e-177">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="8b26e-177">The ID of the role definition.</span></span> <span data-ttu-id="8b26e-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b26e-178">Required.</span></span> |
| <span data-ttu-id="8b26e-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="8b26e-179">subjectId</span></span>        | <span data-ttu-id="8b26e-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-180">String</span></span>                                                   | <span data-ttu-id="8b26e-181">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="8b26e-181">The ID of the subject.</span></span> <span data-ttu-id="8b26e-182">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b26e-182">Required.</span></span> |
| <span data-ttu-id="8b26e-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8b26e-183">assignmentState</span></span>  | <span data-ttu-id="8b26e-184">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-184">String</span></span>                                                   | <span data-ttu-id="8b26e-185">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="8b26e-185">The state of assignment.</span></span> <span data-ttu-id="8b26e-186">O valor pode ser `Eligible` e `Active` .</span><span class="sxs-lookup"><span data-stu-id="8b26e-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="8b26e-187">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b26e-187">Required.</span></span> |
| <span data-ttu-id="8b26e-188">tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-188">type</span></span>             | <span data-ttu-id="8b26e-189">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-189">String</span></span>                                                   | <span data-ttu-id="8b26e-190">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b26e-190">The request type.</span></span> <span data-ttu-id="8b26e-191">O valor pode `AdminAdd` ser , , , , , , `UserAdd` e `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="8b26e-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="8b26e-192">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b26e-192">Required.</span></span> |
| <span data-ttu-id="8b26e-193">motivo</span><span class="sxs-lookup"><span data-stu-id="8b26e-193">reason</span></span>           | <span data-ttu-id="8b26e-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-194">String</span></span>                                                   | <span data-ttu-id="8b26e-195">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e revisão.</span><span class="sxs-lookup"><span data-stu-id="8b26e-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="8b26e-196">Cronograma</span><span class="sxs-lookup"><span data-stu-id="8b26e-196">schedule</span></span>         | [<span data-ttu-id="8b26e-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8b26e-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8b26e-198">O cronograma da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="8b26e-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="8b26e-199">Para o tipo de `UserAdd` `AdminAdd` solicitação de , `AdminUpdate` , e , é `AdminExtend` necessário.</span><span class="sxs-lookup"><span data-stu-id="8b26e-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="8b26e-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b26e-200">Response</span></span>

<span data-ttu-id="8b26e-201">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b26e-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="8b26e-202">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="8b26e-202">Error codes</span></span>

<span data-ttu-id="8b26e-203">Esta API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="8b26e-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="8b26e-204">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="8b26e-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="8b26e-205">Código de erro</span><span class="sxs-lookup"><span data-stu-id="8b26e-205">Error code</span></span>     | <span data-ttu-id="8b26e-206">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="8b26e-206">Error message</span></span>                               | <span data-ttu-id="8b26e-207">Detalhes</span><span class="sxs-lookup"><span data-stu-id="8b26e-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="8b26e-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-208">400 BadRequest</span></span> | <span data-ttu-id="8b26e-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="8b26e-209">RoleNotFound</span></span>                                | <span data-ttu-id="8b26e-210">O `roleDefinitionId` fornecido no corpo da solicitação não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="8b26e-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="8b26e-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-211">400 BadRequest</span></span> | <span data-ttu-id="8b26e-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="8b26e-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="8b26e-213">O recurso fornecido no corpo da solicitação está em estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="8b26e-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="8b26e-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-214">400 BadRequest</span></span> | <span data-ttu-id="8b26e-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="8b26e-215">SubjectNotFound</span></span>                             | <span data-ttu-id="8b26e-216">O `subjectId` fornecido no corpo da solicitação não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="8b26e-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="8b26e-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-217">400 BadRequest</span></span> | <span data-ttu-id="8b26e-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="8b26e-219">Já existe uma [governança pendenteRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema.</span><span class="sxs-lookup"><span data-stu-id="8b26e-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="8b26e-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-220">400 BadRequest</span></span> | <span data-ttu-id="8b26e-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="8b26e-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="8b26e-222">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="8b26e-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="8b26e-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-223">400 BadRequest</span></span> | <span data-ttu-id="8b26e-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="8b26e-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="8b26e-225">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="8b26e-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="8b26e-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="8b26e-226">400 BadRequest</span></span> | <span data-ttu-id="8b26e-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="8b26e-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="8b26e-228">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atendem a políticas internas e não podem ser criados.</span><span class="sxs-lookup"><span data-stu-id="8b26e-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="8b26e-229">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8b26e-229">Examples</span></span>

<span data-ttu-id="8b26e-230">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="8b26e-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="8b26e-231">Exemplo 1: Administrador atribui usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="8b26e-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="8b26e-232">Neste exemplo, um administrador atribui nawu@contoso.com usuário à função Leitor de Cobrança.</span><span class="sxs-lookup"><span data-stu-id="8b26e-232">In this example, an administrator assigns user nawu@contoso.com to the Billing Reader role.</span></span>

 ><span data-ttu-id="8b26e-233">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="8b26e-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="8b26e-234">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b26e-234">Property</span></span>         | <span data-ttu-id="8b26e-235">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-235">Type</span></span>                                                     | <span data-ttu-id="8b26e-236">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8b26e-236">Required</span></span>                 | <span data-ttu-id="8b26e-237">Valor</span><span class="sxs-lookup"><span data-stu-id="8b26e-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="8b26e-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="8b26e-238">resourceId</span></span>       | <span data-ttu-id="8b26e-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-239">String</span></span>                                                   | <span data-ttu-id="8b26e-240">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="8b26e-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8b26e-241">roleDefinitionId</span></span> | <span data-ttu-id="8b26e-242">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-242">String</span></span>                                                   | <span data-ttu-id="8b26e-243">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="8b26e-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="8b26e-244">subjectId</span></span>        | <span data-ttu-id="8b26e-245">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-245">String</span></span>                                                   | <span data-ttu-id="8b26e-246">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="8b26e-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8b26e-247">assignmentState</span></span>  | <span data-ttu-id="8b26e-248">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-248">String</span></span>                                                   | <span data-ttu-id="8b26e-249">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-249">Yes</span></span>                      | <span data-ttu-id="8b26e-250">Qualificado / Ativo</span><span class="sxs-lookup"><span data-stu-id="8b26e-250">Eligible / Active</span></span> |
| <span data-ttu-id="8b26e-251">tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-251">type</span></span>             | <span data-ttu-id="8b26e-252">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-252">String</span></span>                                                   | <span data-ttu-id="8b26e-253">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-253">Yes</span></span>                      | <span data-ttu-id="8b26e-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="8b26e-254">AdminAdd</span></span> |
| <span data-ttu-id="8b26e-255">motivo</span><span class="sxs-lookup"><span data-stu-id="8b26e-255">reason</span></span>           | <span data-ttu-id="8b26e-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-256">String</span></span>                                                   | <span data-ttu-id="8b26e-257">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="8b26e-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="8b26e-258">Cronograma</span><span class="sxs-lookup"><span data-stu-id="8b26e-258">schedule</span></span>         | [<span data-ttu-id="8b26e-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8b26e-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8b26e-260">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="8b26e-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b26e-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b26e-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b26e-262">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_1"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8b26e-263">C#</span><span class="sxs-lookup"><span data-stu-id="8b26e-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b26e-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b26e-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b26e-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b26e-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b26e-266">Java</span><span class="sxs-lookup"><span data-stu-id="8b26e-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="8b26e-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b26e-267">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminAdd",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Evaluate Only",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="8b26e-268">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="8b26e-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="8b26e-269">Neste exemplo, o usuário nawu@contoso.com ativa a função leitor de cobrança qualificada.</span><span class="sxs-lookup"><span data-stu-id="8b26e-269">In this example, the user nawu@contoso.com activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="8b26e-270">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b26e-270">Property</span></span>         | <span data-ttu-id="8b26e-271">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-271">Type</span></span>                                                     | <span data-ttu-id="8b26e-272">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8b26e-272">Required</span></span>                 | <span data-ttu-id="8b26e-273">Valor</span><span class="sxs-lookup"><span data-stu-id="8b26e-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="8b26e-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="8b26e-274">resourceId</span></span>       | <span data-ttu-id="8b26e-275">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-275">String</span></span>                                                   | <span data-ttu-id="8b26e-276">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="8b26e-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8b26e-277">roleDefinitionId</span></span> | <span data-ttu-id="8b26e-278">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-278">String</span></span>                                                   | <span data-ttu-id="8b26e-279">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="8b26e-280">subjectId</span><span class="sxs-lookup"><span data-stu-id="8b26e-280">subjectId</span></span>        | <span data-ttu-id="8b26e-281">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-281">String</span></span>                                                   | <span data-ttu-id="8b26e-282">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="8b26e-283">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8b26e-283">assignmentState</span></span>  | <span data-ttu-id="8b26e-284">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-284">String</span></span>                                                   | <span data-ttu-id="8b26e-285">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-285">Yes</span></span>                      | <span data-ttu-id="8b26e-286">Ativa</span><span class="sxs-lookup"><span data-stu-id="8b26e-286">Active</span></span> |
| <span data-ttu-id="8b26e-287">tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-287">type</span></span>             | <span data-ttu-id="8b26e-288">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-288">String</span></span>                                                   | <span data-ttu-id="8b26e-289">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-289">Yes</span></span>                      | <span data-ttu-id="8b26e-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="8b26e-290">UserAdd</span></span> |
| <span data-ttu-id="8b26e-291">motivo</span><span class="sxs-lookup"><span data-stu-id="8b26e-291">reason</span></span>           | <span data-ttu-id="8b26e-292">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-292">String</span></span>                                                   | <span data-ttu-id="8b26e-293">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="8b26e-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="8b26e-294">Cronograma</span><span class="sxs-lookup"><span data-stu-id="8b26e-294">schedule</span></span>         | [<span data-ttu-id="8b26e-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8b26e-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8b26e-296">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="8b26e-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b26e-297">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b26e-298">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b26e-298">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_2"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
# <a name="c"></a>[<span data-ttu-id="8b26e-299">C#</span><span class="sxs-lookup"><span data-stu-id="8b26e-299">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b26e-300">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b26e-300">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b26e-301">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b26e-301">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b26e-302">Java</span><span class="sxs-lookup"><span data-stu-id="8b26e-302">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8b26e-303">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b26e-303">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
  "type": "UserAdd",
  "assignmentState": "Active",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Activate the owner role",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "EligibilityRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      },
      {
        "key": "JustificationRule",
        "value": "Grant"
      },
      {
        "key": "ActivationDayRule",
        "value": "Grant"
      },
      {
        "key": "ApprovalRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "endDateTime": "0001-01-01T00:00:00Z",
    "duration": "PT9H"
  }
}
```

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="8b26e-304">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="8b26e-304">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="8b26e-305">Neste exemplo, o usuário nawu@contoso.com desativa a função leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="8b26e-305">In this example, the user nawu@contoso.com deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="8b26e-306">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b26e-306">Property</span></span>         | <span data-ttu-id="8b26e-307">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-307">Type</span></span>                                                     | <span data-ttu-id="8b26e-308">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8b26e-308">Required</span></span> | <span data-ttu-id="8b26e-309">Valor</span><span class="sxs-lookup"><span data-stu-id="8b26e-309">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="8b26e-310">resourceId</span><span class="sxs-lookup"><span data-stu-id="8b26e-310">resourceId</span></span>       | <span data-ttu-id="8b26e-311">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-311">String</span></span>                                                   | <span data-ttu-id="8b26e-312">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-312">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="8b26e-313">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8b26e-313">roleDefinitionId</span></span> | <span data-ttu-id="8b26e-314">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-314">String</span></span>                                                   | <span data-ttu-id="8b26e-315">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-315">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="8b26e-316">subjectId</span><span class="sxs-lookup"><span data-stu-id="8b26e-316">subjectId</span></span>        | <span data-ttu-id="8b26e-317">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-317">String</span></span>                                                   | <span data-ttu-id="8b26e-318">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-318">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="8b26e-319">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8b26e-319">assignmentState</span></span>  | <span data-ttu-id="8b26e-320">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-320">String</span></span>                                                   | <span data-ttu-id="8b26e-321">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-321">Yes</span></span>      | <span data-ttu-id="8b26e-322">Ativa</span><span class="sxs-lookup"><span data-stu-id="8b26e-322">Active</span></span> |
| <span data-ttu-id="8b26e-323">tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-323">type</span></span>             | <span data-ttu-id="8b26e-324">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-324">String</span></span>                                                   | <span data-ttu-id="8b26e-325">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-325">Yes</span></span>      | <span data-ttu-id="8b26e-326">UserRemove</span><span class="sxs-lookup"><span data-stu-id="8b26e-326">UserRemove</span></span> |
| <span data-ttu-id="8b26e-327">motivo</span><span class="sxs-lookup"><span data-stu-id="8b26e-327">reason</span></span>           | <span data-ttu-id="8b26e-328">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-328">String</span></span>                                                   | <span data-ttu-id="8b26e-329">Não</span><span class="sxs-lookup"><span data-stu-id="8b26e-329">No</span></span>       |   |
| <span data-ttu-id="8b26e-330">Cronograma</span><span class="sxs-lookup"><span data-stu-id="8b26e-330">schedule</span></span>         | [<span data-ttu-id="8b26e-331">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8b26e-331">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8b26e-332">Não</span><span class="sxs-lookup"><span data-stu-id="8b26e-332">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="8b26e-333">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b26e-333">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b26e-334">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b26e-334">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_3"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
# <a name="c"></a>[<span data-ttu-id="8b26e-335">C#</span><span class="sxs-lookup"><span data-stu-id="8b26e-335">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b26e-336">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b26e-336">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b26e-337">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b26e-337">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b26e-338">Java</span><span class="sxs-lookup"><span data-stu-id="8b26e-338">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8b26e-339">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b26e-339">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
  "type": "UserRemove",
  "assignmentState": "Active",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Evaluate only",
  "schedule": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  }
}
```

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="8b26e-340">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="8b26e-340">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="8b26e-341">Neste exemplo, um administrador remove o usuário nawu@contoso.com da função Leitor de Cobrança.</span><span class="sxs-lookup"><span data-stu-id="8b26e-341">In this example, an administrator removes the user nawu@contoso.com from the Billing Reader role.</span></span>

 ><span data-ttu-id="8b26e-342">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="8b26e-342">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="8b26e-343">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b26e-343">Property</span></span>         | <span data-ttu-id="8b26e-344">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-344">Type</span></span>                                                     | <span data-ttu-id="8b26e-345">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8b26e-345">Required</span></span> | <span data-ttu-id="8b26e-346">Valor</span><span class="sxs-lookup"><span data-stu-id="8b26e-346">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="8b26e-347">resourceId</span><span class="sxs-lookup"><span data-stu-id="8b26e-347">resourceId</span></span>       | <span data-ttu-id="8b26e-348">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-348">String</span></span>                                                   | <span data-ttu-id="8b26e-349">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-349">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="8b26e-350">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8b26e-350">roleDefinitionId</span></span> | <span data-ttu-id="8b26e-351">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-351">String</span></span>                                                   | <span data-ttu-id="8b26e-352">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-352">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="8b26e-353">subjectId</span><span class="sxs-lookup"><span data-stu-id="8b26e-353">subjectId</span></span>        | <span data-ttu-id="8b26e-354">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-354">String</span></span>                                                   | <span data-ttu-id="8b26e-355">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-355">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="8b26e-356">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8b26e-356">assignmentState</span></span>  | <span data-ttu-id="8b26e-357">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-357">String</span></span>                                                   | <span data-ttu-id="8b26e-358">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-358">Yes</span></span>      | <span data-ttu-id="8b26e-359">Qualificado / Ativo</span><span class="sxs-lookup"><span data-stu-id="8b26e-359">Eligible / Active</span></span> |
| <span data-ttu-id="8b26e-360">tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-360">type</span></span>             | <span data-ttu-id="8b26e-361">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-361">String</span></span>                                                   | <span data-ttu-id="8b26e-362">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-362">Yes</span></span>      | <span data-ttu-id="8b26e-363">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="8b26e-363">AdminRemove</span></span> |
| <span data-ttu-id="8b26e-364">motivo</span><span class="sxs-lookup"><span data-stu-id="8b26e-364">reason</span></span>           | <span data-ttu-id="8b26e-365">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-365">String</span></span>                                                   | <span data-ttu-id="8b26e-366">Não</span><span class="sxs-lookup"><span data-stu-id="8b26e-366">No</span></span>       |   |
| <span data-ttu-id="8b26e-367">Cronograma</span><span class="sxs-lookup"><span data-stu-id="8b26e-367">schedule</span></span>         | [<span data-ttu-id="8b26e-368">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8b26e-368">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8b26e-369">Não</span><span class="sxs-lookup"><span data-stu-id="8b26e-369">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="8b26e-370">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b26e-370">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b26e-371">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b26e-371">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_4"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```
# <a name="c"></a>[<span data-ttu-id="8b26e-372">C#</span><span class="sxs-lookup"><span data-stu-id="8b26e-372">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b26e-373">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b26e-373">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b26e-374">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b26e-374">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b26e-375">Java</span><span class="sxs-lookup"><span data-stu-id="8b26e-375">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8b26e-376">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b26e-376">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="8b26e-377">Exemplo 5: atribuição de função de atualização de administrador</span><span class="sxs-lookup"><span data-stu-id="8b26e-377">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="8b26e-378">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@contoso.com para Proprietário.</span><span class="sxs-lookup"><span data-stu-id="8b26e-378">In this example, administrators update the role assignment for the user nawu@contoso.com to Owner.</span></span>

 ><span data-ttu-id="8b26e-379">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="8b26e-379">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="8b26e-380">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b26e-380">Property</span></span>         | <span data-ttu-id="8b26e-381">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-381">Type</span></span>                                                     | <span data-ttu-id="8b26e-382">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8b26e-382">Required</span></span>                | <span data-ttu-id="8b26e-383">Valor</span><span class="sxs-lookup"><span data-stu-id="8b26e-383">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="8b26e-384">resourceId</span><span class="sxs-lookup"><span data-stu-id="8b26e-384">resourceId</span></span>       | <span data-ttu-id="8b26e-385">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-385">String</span></span>                                                   | <span data-ttu-id="8b26e-386">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-386">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="8b26e-387">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8b26e-387">roleDefinitionId</span></span> | <span data-ttu-id="8b26e-388">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-388">String</span></span>                                                   | <span data-ttu-id="8b26e-389">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-389">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="8b26e-390">subjectId</span><span class="sxs-lookup"><span data-stu-id="8b26e-390">subjectId</span></span>        | <span data-ttu-id="8b26e-391">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-391">String</span></span>                                                   | <span data-ttu-id="8b26e-392">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-392">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="8b26e-393">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8b26e-393">assignmentState</span></span>  | <span data-ttu-id="8b26e-394">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-394">String</span></span>                                                   | <span data-ttu-id="8b26e-395">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-395">Yes</span></span>                     | <span data-ttu-id="8b26e-396">Qualificado / Ativo</span><span class="sxs-lookup"><span data-stu-id="8b26e-396">Eligible / Active</span></span> |
| <span data-ttu-id="8b26e-397">tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-397">type</span></span>             | <span data-ttu-id="8b26e-398">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-398">String</span></span>                                                   | <span data-ttu-id="8b26e-399">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-399">Yes</span></span>                     | <span data-ttu-id="8b26e-400">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="8b26e-400">AdminUpdate</span></span> |
| <span data-ttu-id="8b26e-401">motivo</span><span class="sxs-lookup"><span data-stu-id="8b26e-401">reason</span></span>           | <span data-ttu-id="8b26e-402">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-402">String</span></span>                                                   | <span data-ttu-id="8b26e-403">depende de roleSettings</span><span class="sxs-lookup"><span data-stu-id="8b26e-403">depends on roleSettings</span></span> |   |
| <span data-ttu-id="8b26e-404">Cronograma</span><span class="sxs-lookup"><span data-stu-id="8b26e-404">schedule</span></span>         | [<span data-ttu-id="8b26e-405">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8b26e-405">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8b26e-406">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-406">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="8b26e-407">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b26e-407">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b26e-408">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b26e-408">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_5"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8b26e-409">C#</span><span class="sxs-lookup"><span data-stu-id="8b26e-409">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b26e-410">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b26e-410">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b26e-411">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b26e-411">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b26e-412">Java</span><span class="sxs-lookup"><span data-stu-id="8b26e-412">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8b26e-413">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b26e-413">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="8b26e-414">Exemplo 6: o administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="8b26e-414">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="8b26e-415">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o Colaborador do Serviço de Gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="8b26e-415">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="8b26e-416">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="8b26e-416">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="8b26e-417">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b26e-417">Property</span></span>         | <span data-ttu-id="8b26e-418">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-418">Type</span></span>                                                     | <span data-ttu-id="8b26e-419">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="8b26e-419">Required</span></span>                | <span data-ttu-id="8b26e-420">Valor</span><span class="sxs-lookup"><span data-stu-id="8b26e-420">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="8b26e-421">resourceId</span><span class="sxs-lookup"><span data-stu-id="8b26e-421">resourceId</span></span>       | <span data-ttu-id="8b26e-422">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-422">String</span></span>                                                   | <span data-ttu-id="8b26e-423">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-423">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="8b26e-424">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="8b26e-424">roleDefinitionId</span></span> | <span data-ttu-id="8b26e-425">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-425">String</span></span>                                                   | <span data-ttu-id="8b26e-426">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-426">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="8b26e-427">subjectId</span><span class="sxs-lookup"><span data-stu-id="8b26e-427">subjectId</span></span>        | <span data-ttu-id="8b26e-428">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-428">String</span></span>                                                   | <span data-ttu-id="8b26e-429">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-429">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="8b26e-430">assignmentState</span><span class="sxs-lookup"><span data-stu-id="8b26e-430">assignmentState</span></span>  | <span data-ttu-id="8b26e-431">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-431">String</span></span>                                                   | <span data-ttu-id="8b26e-432">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-432">Yes</span></span>                     | <span data-ttu-id="8b26e-433">Qualificado / Ativo</span><span class="sxs-lookup"><span data-stu-id="8b26e-433">Eligible / Active</span></span> |
| <span data-ttu-id="8b26e-434">tipo</span><span class="sxs-lookup"><span data-stu-id="8b26e-434">type</span></span>             | <span data-ttu-id="8b26e-435">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-435">String</span></span>                                                   | <span data-ttu-id="8b26e-436">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-436">Yes</span></span>                     | <span data-ttu-id="8b26e-437">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="8b26e-437">AdminExtend</span></span> |
| <span data-ttu-id="8b26e-438">motivo</span><span class="sxs-lookup"><span data-stu-id="8b26e-438">reason</span></span>           | <span data-ttu-id="8b26e-439">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b26e-439">String</span></span>                                                   | <span data-ttu-id="8b26e-440">depende de roleSettings</span><span class="sxs-lookup"><span data-stu-id="8b26e-440">depends on roleSettings</span></span> |   |
| <span data-ttu-id="8b26e-441">Cronograma</span><span class="sxs-lookup"><span data-stu-id="8b26e-441">schedule</span></span>         | [<span data-ttu-id="8b26e-442">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8b26e-442">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="8b26e-443">Sim</span><span class="sxs-lookup"><span data-stu-id="8b26e-443">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="8b26e-444">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b26e-444">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b26e-445">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b26e-445">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post_6"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="8b26e-446">C#</span><span class="sxs-lookup"><span data-stu-id="8b26e-446">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b26e-447">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b26e-447">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b26e-448">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b26e-448">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b26e-449">Java</span><span class="sxs-lookup"><span data-stu-id="8b26e-449">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8b26e-450">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b26e-450">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


