---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação que você deseja em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 2cb6ee71c888e90ee082c1f70ecced2c21199939
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435858"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="7bce8-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="7bce8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bce8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bce8-106">Crie uma solicitação de atribuição de função para representar a operação que você deseja em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7bce8-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="7bce8-107">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="7bce8-107">The following table lists the operations.</span></span>

| <span data-ttu-id="7bce8-108">Operation</span><span class="sxs-lookup"><span data-stu-id="7bce8-108">Operation</span></span>                                   | <span data-ttu-id="7bce8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bce8-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="7bce8-110">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="7bce8-110">Assign a role assignment</span></span>                    | <span data-ttu-id="7bce8-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="7bce8-111">AdminAdd</span></span>    |
| <span data-ttu-id="7bce8-112">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="7bce8-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="7bce8-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="7bce8-113">UserAdd</span></span>     |
| <span data-ttu-id="7bce8-114">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="7bce8-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="7bce8-115">UserRemove</span><span class="sxs-lookup"><span data-stu-id="7bce8-115">UserRemove</span></span>  |
| <span data-ttu-id="7bce8-116">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="7bce8-116">Remove a role assignment</span></span>                    | <span data-ttu-id="7bce8-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="7bce8-117">AdminRemove</span></span> |
| <span data-ttu-id="7bce8-118">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="7bce8-118">Update a role assignment</span></span>                    | <span data-ttu-id="7bce8-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="7bce8-119">AdminUpdate</span></span> |
| <span data-ttu-id="7bce8-120">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="7bce8-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="7bce8-121">UserExtend</span><span class="sxs-lookup"><span data-stu-id="7bce8-121">UserExtend</span></span>  |
| <span data-ttu-id="7bce8-122">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="7bce8-122">Extend a role assignment</span></span>                    | <span data-ttu-id="7bce8-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="7bce8-123">AdminExtend</span></span> |
| <span data-ttu-id="7bce8-124">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="7bce8-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="7bce8-125">UserRenew</span><span class="sxs-lookup"><span data-stu-id="7bce8-125">UserRenew</span></span>   |
| <span data-ttu-id="7bce8-126">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="7bce8-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="7bce8-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="7bce8-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="7bce8-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bce8-128">Permissions</span></span>

<span data-ttu-id="7bce8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="7bce8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="7bce8-131">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="7bce8-131">Azure resources</span></span>

| <span data-ttu-id="7bce8-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bce8-132">Permission type</span></span> | <span data-ttu-id="7bce8-133">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bce8-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="7bce8-134">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bce8-134">Delegated (work or school account)</span></span> | <span data-ttu-id="7bce8-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7bce8-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="7bce8-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bce8-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bce8-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bce8-137">Not supported.</span></span> |
| <span data-ttu-id="7bce8-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-138">Application</span></span> | <span data-ttu-id="7bce8-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bce8-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="7bce8-140">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7bce8-140">Azure AD</span></span>

| <span data-ttu-id="7bce8-141">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bce8-141">Permission type</span></span> | <span data-ttu-id="7bce8-142">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bce8-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="7bce8-143">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bce8-143">Delegated (work or school account)</span></span> | <span data-ttu-id="7bce8-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="7bce8-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="7bce8-145">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bce8-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bce8-146">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bce8-146">Not supported.</span></span> |
| <span data-ttu-id="7bce8-147">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-147">Application</span></span> | <span data-ttu-id="7bce8-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bce8-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="7bce8-149">Grupos</span><span class="sxs-lookup"><span data-stu-id="7bce8-149">Groups</span></span>

|<span data-ttu-id="7bce8-150">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bce8-150">Permission type</span></span> | <span data-ttu-id="7bce8-151">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bce8-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="7bce8-152">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bce8-152">Delegated (work or school account)</span></span> | <span data-ttu-id="7bce8-153">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="7bce8-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="7bce8-154">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bce8-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bce8-155">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bce8-155">Not supported.</span></span> |
| <span data-ttu-id="7bce8-156">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-156">Application</span></span> | <span data-ttu-id="7bce8-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7bce8-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bce8-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bce8-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="7bce8-159">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bce8-159">Request headers</span></span>

| <span data-ttu-id="7bce8-160">Nome</span><span class="sxs-lookup"><span data-stu-id="7bce8-160">Name</span></span>          | <span data-ttu-id="7bce8-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bce8-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="7bce8-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bce8-162">Authorization</span></span> | <span data-ttu-id="7bce8-163">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7bce8-163">Bearer {code}</span></span>    |
| <span data-ttu-id="7bce8-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="7bce8-164">Content-type</span></span>  | <span data-ttu-id="7bce8-165">application/json</span><span class="sxs-lookup"><span data-stu-id="7bce8-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bce8-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bce8-166">Request body</span></span>

<span data-ttu-id="7bce8-167">No corpo da solicitação, fornece uma representação JSON de um [objeto governanceRoleAssignmentRequest.](../resources/governanceroleassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="7bce8-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="7bce8-168">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bce8-168">Property</span></span>         | <span data-ttu-id="7bce8-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bce8-169">Type</span></span>                                                     | <span data-ttu-id="7bce8-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bce8-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="7bce8-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="7bce8-171">resourceId</span></span>       | <span data-ttu-id="7bce8-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bce8-172">String</span></span>                                                   | <span data-ttu-id="7bce8-173">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bce8-173">The ID of the resource.</span></span> <span data-ttu-id="7bce8-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bce8-174">Required.</span></span> |
| <span data-ttu-id="7bce8-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7bce8-175">roleDefinitionId</span></span> | <span data-ttu-id="7bce8-176">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-176">String</span></span>                                                   | <span data-ttu-id="7bce8-177">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="7bce8-177">The ID of the role definition.</span></span> <span data-ttu-id="7bce8-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bce8-178">Required.</span></span> |
| <span data-ttu-id="7bce8-179">subjectId</span><span class="sxs-lookup"><span data-stu-id="7bce8-179">subjectId</span></span>        | <span data-ttu-id="7bce8-180">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-180">String</span></span>                                                   | <span data-ttu-id="7bce8-181">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="7bce8-181">The ID of the subject.</span></span> <span data-ttu-id="7bce8-182">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bce8-182">Required.</span></span> |
| <span data-ttu-id="7bce8-183">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7bce8-183">assignmentState</span></span>  | <span data-ttu-id="7bce8-184">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-184">String</span></span>                                                   | <span data-ttu-id="7bce8-185">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="7bce8-185">The state of assignment.</span></span> <span data-ttu-id="7bce8-186">O valor pode ser `Eligible` e `Active` .</span><span class="sxs-lookup"><span data-stu-id="7bce8-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="7bce8-187">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bce8-187">Required.</span></span> |
| <span data-ttu-id="7bce8-188">type</span><span class="sxs-lookup"><span data-stu-id="7bce8-188">type</span></span>             | <span data-ttu-id="7bce8-189">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-189">String</span></span>                                                   | <span data-ttu-id="7bce8-190">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7bce8-190">The request type.</span></span> <span data-ttu-id="7bce8-191">O valor pode `AdminAdd` ser , , , , , , `UserAdd` e `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="7bce8-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="7bce8-192">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bce8-192">Required.</span></span> |
| <span data-ttu-id="7bce8-193">motivo</span><span class="sxs-lookup"><span data-stu-id="7bce8-193">reason</span></span>           | <span data-ttu-id="7bce8-194">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-194">String</span></span>                                                   | <span data-ttu-id="7bce8-195">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e revisão.</span><span class="sxs-lookup"><span data-stu-id="7bce8-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="7bce8-196">Cronograma</span><span class="sxs-lookup"><span data-stu-id="7bce8-196">schedule</span></span>         | [<span data-ttu-id="7bce8-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7bce8-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7bce8-198">O cronograma da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7bce8-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="7bce8-199">Para o tipo de `UserAdd` `AdminAdd` solicitação de , `AdminUpdate` , e , é `AdminExtend` necessário.</span><span class="sxs-lookup"><span data-stu-id="7bce8-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="7bce8-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bce8-200">Response</span></span>

<span data-ttu-id="7bce8-201">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bce8-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="7bce8-202">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="7bce8-202">Error codes</span></span>

<span data-ttu-id="7bce8-203">Esta API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="7bce8-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="7bce8-204">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7bce8-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="7bce8-205">Código de erro</span><span class="sxs-lookup"><span data-stu-id="7bce8-205">Error code</span></span>     | <span data-ttu-id="7bce8-206">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="7bce8-206">Error message</span></span>                               | <span data-ttu-id="7bce8-207">Detalhes</span><span class="sxs-lookup"><span data-stu-id="7bce8-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="7bce8-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-208">400 BadRequest</span></span> | <span data-ttu-id="7bce8-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="7bce8-209">RoleNotFound</span></span>                                | <span data-ttu-id="7bce8-210">O `roleDefinitionId` fornecido no corpo da solicitação não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="7bce8-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="7bce8-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-211">400 BadRequest</span></span> | <span data-ttu-id="7bce8-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="7bce8-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="7bce8-213">O recurso fornecido no corpo da solicitação está em estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="7bce8-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="7bce8-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-214">400 BadRequest</span></span> | <span data-ttu-id="7bce8-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="7bce8-215">SubjectNotFound</span></span>                             | <span data-ttu-id="7bce8-216">O `subjectId` fornecido no corpo da solicitação não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="7bce8-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="7bce8-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-217">400 BadRequest</span></span> | <span data-ttu-id="7bce8-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="7bce8-219">Já existe uma [governança pendenteRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema.</span><span class="sxs-lookup"><span data-stu-id="7bce8-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="7bce8-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-220">400 BadRequest</span></span> | <span data-ttu-id="7bce8-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="7bce8-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="7bce8-222">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="7bce8-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="7bce8-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-223">400 BadRequest</span></span> | <span data-ttu-id="7bce8-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="7bce8-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="7bce8-225">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="7bce8-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="7bce8-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="7bce8-226">400 BadRequest</span></span> | <span data-ttu-id="7bce8-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="7bce8-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="7bce8-228">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atendem a políticas internas e não podem ser criados.</span><span class="sxs-lookup"><span data-stu-id="7bce8-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="7bce8-229">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7bce8-229">Examples</span></span>

<span data-ttu-id="7bce8-230">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="7bce8-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="7bce8-231">Exemplo 1: Administrador atribui usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="7bce8-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="7bce8-232">Neste exemplo, um administrador atribui nawu@contoso.com usuário à função Leitor de Cobrança.</span><span class="sxs-lookup"><span data-stu-id="7bce8-232">In this example, an administrator assigns user nawu@contoso.com to the Billing Reader role.</span></span>

 ><span data-ttu-id="7bce8-233">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="7bce8-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7bce8-234">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bce8-234">Property</span></span>         | <span data-ttu-id="7bce8-235">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bce8-235">Type</span></span>                                                     | <span data-ttu-id="7bce8-236">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7bce8-236">Required</span></span>                 | <span data-ttu-id="7bce8-237">Valor</span><span class="sxs-lookup"><span data-stu-id="7bce8-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="7bce8-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="7bce8-238">resourceId</span></span>       | <span data-ttu-id="7bce8-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bce8-239">String</span></span>                                                   | <span data-ttu-id="7bce8-240">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="7bce8-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7bce8-241">roleDefinitionId</span></span> | <span data-ttu-id="7bce8-242">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-242">String</span></span>                                                   | <span data-ttu-id="7bce8-243">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="7bce8-244">subjectId</span><span class="sxs-lookup"><span data-stu-id="7bce8-244">subjectId</span></span>        | <span data-ttu-id="7bce8-245">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-245">String</span></span>                                                   | <span data-ttu-id="7bce8-246">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="7bce8-247">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7bce8-247">assignmentState</span></span>  | <span data-ttu-id="7bce8-248">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-248">String</span></span>                                                   | <span data-ttu-id="7bce8-249">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-249">Yes</span></span>                      | <span data-ttu-id="7bce8-250">Qualificado / Ativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-250">Eligible / Active</span></span> |
| <span data-ttu-id="7bce8-251">type</span><span class="sxs-lookup"><span data-stu-id="7bce8-251">type</span></span>             | <span data-ttu-id="7bce8-252">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-252">String</span></span>                                                   | <span data-ttu-id="7bce8-253">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-253">Yes</span></span>                      | <span data-ttu-id="7bce8-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="7bce8-254">AdminAdd</span></span> |
| <span data-ttu-id="7bce8-255">motivo</span><span class="sxs-lookup"><span data-stu-id="7bce8-255">reason</span></span>           | <span data-ttu-id="7bce8-256">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-256">String</span></span>                                                   | <span data-ttu-id="7bce8-257">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="7bce8-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="7bce8-258">Cronograma</span><span class="sxs-lookup"><span data-stu-id="7bce8-258">schedule</span></span>         | [<span data-ttu-id="7bce8-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7bce8-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7bce8-260">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="7bce8-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bce8-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7bce8-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bce8-262">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
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
# <a name="c"></a>[<span data-ttu-id="7bce8-263">C#</span><span class="sxs-lookup"><span data-stu-id="7bce8-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7bce8-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bce8-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7bce8-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7bce8-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7bce8-266">Java</span><span class="sxs-lookup"><span data-stu-id="7bce8-266">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="7bce8-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bce8-267">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="7bce8-268">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="7bce8-268">Example 2: User activates eligible role</span></span>

<span data-ttu-id="7bce8-269">Neste exemplo, o usuário nawu@contoso.com ativa a função leitor de cobrança qualificada.</span><span class="sxs-lookup"><span data-stu-id="7bce8-269">In this example, the user nawu@contoso.com activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="7bce8-270">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bce8-270">Property</span></span>         | <span data-ttu-id="7bce8-271">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bce8-271">Type</span></span>                                                     | <span data-ttu-id="7bce8-272">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7bce8-272">Required</span></span>                 | <span data-ttu-id="7bce8-273">Valor</span><span class="sxs-lookup"><span data-stu-id="7bce8-273">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="7bce8-274">resourceId</span><span class="sxs-lookup"><span data-stu-id="7bce8-274">resourceId</span></span>       | <span data-ttu-id="7bce8-275">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bce8-275">String</span></span>                                                   | <span data-ttu-id="7bce8-276">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-276">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="7bce8-277">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7bce8-277">roleDefinitionId</span></span> | <span data-ttu-id="7bce8-278">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-278">String</span></span>                                                   | <span data-ttu-id="7bce8-279">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-279">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="7bce8-280">subjectId</span><span class="sxs-lookup"><span data-stu-id="7bce8-280">subjectId</span></span>        | <span data-ttu-id="7bce8-281">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-281">String</span></span>                                                   | <span data-ttu-id="7bce8-282">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-282">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="7bce8-283">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7bce8-283">assignmentState</span></span>  | <span data-ttu-id="7bce8-284">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-284">String</span></span>                                                   | <span data-ttu-id="7bce8-285">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-285">Yes</span></span>                      | <span data-ttu-id="7bce8-286">Ativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-286">Active</span></span> |
| <span data-ttu-id="7bce8-287">type</span><span class="sxs-lookup"><span data-stu-id="7bce8-287">type</span></span>             | <span data-ttu-id="7bce8-288">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-288">String</span></span>                                                   | <span data-ttu-id="7bce8-289">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-289">Yes</span></span>                      | <span data-ttu-id="7bce8-290">UserAdd</span><span class="sxs-lookup"><span data-stu-id="7bce8-290">UserAdd</span></span> |
| <span data-ttu-id="7bce8-291">motivo</span><span class="sxs-lookup"><span data-stu-id="7bce8-291">reason</span></span>           | <span data-ttu-id="7bce8-292">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-292">String</span></span>                                                   | <span data-ttu-id="7bce8-293">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="7bce8-293">depends on role Settings</span></span> |   |
| <span data-ttu-id="7bce8-294">Cronograma</span><span class="sxs-lookup"><span data-stu-id="7bce8-294">schedule</span></span>         | [<span data-ttu-id="7bce8-295">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7bce8-295">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7bce8-296">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-296">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="7bce8-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bce8-297">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
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

#### <a name="response"></a><span data-ttu-id="7bce8-298">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bce8-298">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="7bce8-299">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="7bce8-299">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="7bce8-300">Neste exemplo, o usuário nawu@contoso.com desativa a função leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="7bce8-300">In this example, the user nawu@contoso.com deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="7bce8-301">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bce8-301">Property</span></span>         | <span data-ttu-id="7bce8-302">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bce8-302">Type</span></span>                                                     | <span data-ttu-id="7bce8-303">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7bce8-303">Required</span></span> | <span data-ttu-id="7bce8-304">Valor</span><span class="sxs-lookup"><span data-stu-id="7bce8-304">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="7bce8-305">resourceId</span><span class="sxs-lookup"><span data-stu-id="7bce8-305">resourceId</span></span>       | <span data-ttu-id="7bce8-306">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bce8-306">String</span></span>                                                   | <span data-ttu-id="7bce8-307">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-307">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="7bce8-308">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7bce8-308">roleDefinitionId</span></span> | <span data-ttu-id="7bce8-309">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-309">String</span></span>                                                   | <span data-ttu-id="7bce8-310">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-310">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="7bce8-311">subjectId</span><span class="sxs-lookup"><span data-stu-id="7bce8-311">subjectId</span></span>        | <span data-ttu-id="7bce8-312">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-312">String</span></span>                                                   | <span data-ttu-id="7bce8-313">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-313">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="7bce8-314">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7bce8-314">assignmentState</span></span>  | <span data-ttu-id="7bce8-315">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-315">String</span></span>                                                   | <span data-ttu-id="7bce8-316">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-316">Yes</span></span>      | <span data-ttu-id="7bce8-317">Ativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-317">Active</span></span> |
| <span data-ttu-id="7bce8-318">type</span><span class="sxs-lookup"><span data-stu-id="7bce8-318">type</span></span>             | <span data-ttu-id="7bce8-319">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-319">String</span></span>                                                   | <span data-ttu-id="7bce8-320">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-320">Yes</span></span>      | <span data-ttu-id="7bce8-321">UserRemove</span><span class="sxs-lookup"><span data-stu-id="7bce8-321">UserRemove</span></span> |
| <span data-ttu-id="7bce8-322">motivo</span><span class="sxs-lookup"><span data-stu-id="7bce8-322">reason</span></span>           | <span data-ttu-id="7bce8-323">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-323">String</span></span>                                                   | <span data-ttu-id="7bce8-324">Não</span><span class="sxs-lookup"><span data-stu-id="7bce8-324">No</span></span>       |   |
| <span data-ttu-id="7bce8-325">Cronograma</span><span class="sxs-lookup"><span data-stu-id="7bce8-325">schedule</span></span>         | [<span data-ttu-id="7bce8-326">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7bce8-326">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7bce8-327">Não</span><span class="sxs-lookup"><span data-stu-id="7bce8-327">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="7bce8-328">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bce8-328">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
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

#### <a name="response"></a><span data-ttu-id="7bce8-329">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bce8-329">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="7bce8-330">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="7bce8-330">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="7bce8-331">Neste exemplo, um administrador remove o usuário nawu@contoso.com da função Leitor de Cobrança.</span><span class="sxs-lookup"><span data-stu-id="7bce8-331">In this example, an administrator removes the user nawu@contoso.com from the Billing Reader role.</span></span>

 ><span data-ttu-id="7bce8-332">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="7bce8-332">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7bce8-333">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bce8-333">Property</span></span>         | <span data-ttu-id="7bce8-334">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bce8-334">Type</span></span>                                                     | <span data-ttu-id="7bce8-335">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7bce8-335">Required</span></span> | <span data-ttu-id="7bce8-336">Valor</span><span class="sxs-lookup"><span data-stu-id="7bce8-336">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="7bce8-337">resourceId</span><span class="sxs-lookup"><span data-stu-id="7bce8-337">resourceId</span></span>       | <span data-ttu-id="7bce8-338">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bce8-338">String</span></span>                                                   | <span data-ttu-id="7bce8-339">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-339">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="7bce8-340">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7bce8-340">roleDefinitionId</span></span> | <span data-ttu-id="7bce8-341">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-341">String</span></span>                                                   | <span data-ttu-id="7bce8-342">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-342">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="7bce8-343">subjectId</span><span class="sxs-lookup"><span data-stu-id="7bce8-343">subjectId</span></span>        | <span data-ttu-id="7bce8-344">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-344">String</span></span>                                                   | <span data-ttu-id="7bce8-345">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-345">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="7bce8-346">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7bce8-346">assignmentState</span></span>  | <span data-ttu-id="7bce8-347">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-347">String</span></span>                                                   | <span data-ttu-id="7bce8-348">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-348">Yes</span></span>      | <span data-ttu-id="7bce8-349">Qualificado / Ativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-349">Eligible / Active</span></span> |
| <span data-ttu-id="7bce8-350">type</span><span class="sxs-lookup"><span data-stu-id="7bce8-350">type</span></span>             | <span data-ttu-id="7bce8-351">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-351">String</span></span>                                                   | <span data-ttu-id="7bce8-352">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-352">Yes</span></span>      | <span data-ttu-id="7bce8-353">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="7bce8-353">AdminRemove</span></span> |
| <span data-ttu-id="7bce8-354">motivo</span><span class="sxs-lookup"><span data-stu-id="7bce8-354">reason</span></span>           | <span data-ttu-id="7bce8-355">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-355">String</span></span>                                                   | <span data-ttu-id="7bce8-356">Não</span><span class="sxs-lookup"><span data-stu-id="7bce8-356">No</span></span>       |   |
| <span data-ttu-id="7bce8-357">Cronograma</span><span class="sxs-lookup"><span data-stu-id="7bce8-357">schedule</span></span>         | [<span data-ttu-id="7bce8-358">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7bce8-358">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7bce8-359">Não</span><span class="sxs-lookup"><span data-stu-id="7bce8-359">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="7bce8-360">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bce8-360">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
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

#### <a name="response"></a><span data-ttu-id="7bce8-361">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bce8-361">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="7bce8-362">Exemplo 5: atribuição de função de atualização de administrador</span><span class="sxs-lookup"><span data-stu-id="7bce8-362">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="7bce8-363">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@contoso.com para Proprietário.</span><span class="sxs-lookup"><span data-stu-id="7bce8-363">In this example, administrators update the role assignment for the user nawu@contoso.com to Owner.</span></span>

 ><span data-ttu-id="7bce8-364">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="7bce8-364">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7bce8-365">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bce8-365">Property</span></span>         | <span data-ttu-id="7bce8-366">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bce8-366">Type</span></span>                                                     | <span data-ttu-id="7bce8-367">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7bce8-367">Required</span></span>                | <span data-ttu-id="7bce8-368">Valor</span><span class="sxs-lookup"><span data-stu-id="7bce8-368">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="7bce8-369">resourceId</span><span class="sxs-lookup"><span data-stu-id="7bce8-369">resourceId</span></span>       | <span data-ttu-id="7bce8-370">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bce8-370">String</span></span>                                                   | <span data-ttu-id="7bce8-371">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-371">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="7bce8-372">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7bce8-372">roleDefinitionId</span></span> | <span data-ttu-id="7bce8-373">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-373">String</span></span>                                                   | <span data-ttu-id="7bce8-374">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-374">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="7bce8-375">subjectId</span><span class="sxs-lookup"><span data-stu-id="7bce8-375">subjectId</span></span>        | <span data-ttu-id="7bce8-376">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-376">String</span></span>                                                   | <span data-ttu-id="7bce8-377">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-377">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="7bce8-378">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7bce8-378">assignmentState</span></span>  | <span data-ttu-id="7bce8-379">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-379">String</span></span>                                                   | <span data-ttu-id="7bce8-380">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-380">Yes</span></span>                     | <span data-ttu-id="7bce8-381">Qualificado / Ativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-381">Eligible / Active</span></span> |
| <span data-ttu-id="7bce8-382">type</span><span class="sxs-lookup"><span data-stu-id="7bce8-382">type</span></span>             | <span data-ttu-id="7bce8-383">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-383">String</span></span>                                                   | <span data-ttu-id="7bce8-384">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-384">Yes</span></span>                     | <span data-ttu-id="7bce8-385">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="7bce8-385">AdminUpdate</span></span> |
| <span data-ttu-id="7bce8-386">motivo</span><span class="sxs-lookup"><span data-stu-id="7bce8-386">reason</span></span>           | <span data-ttu-id="7bce8-387">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-387">String</span></span>                                                   | <span data-ttu-id="7bce8-388">depende de roleSettings</span><span class="sxs-lookup"><span data-stu-id="7bce8-388">depends on roleSettings</span></span> |   |
| <span data-ttu-id="7bce8-389">Cronograma</span><span class="sxs-lookup"><span data-stu-id="7bce8-389">schedule</span></span>         | [<span data-ttu-id="7bce8-390">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7bce8-390">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7bce8-391">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-391">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="7bce8-392">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bce8-392">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
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

#### <a name="response"></a><span data-ttu-id="7bce8-393">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bce8-393">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="7bce8-394">Exemplo 6: o administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="7bce8-394">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="7bce8-395">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o Colaborador do Serviço de Gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="7bce8-395">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="7bce8-396">**Observação:** Além da permissão, este exemplo exige que o solicitante tenha pelo menos uma atribuição de função de administrador `Active` ( ou ) no `owner` `user access administrator` recurso.</span><span class="sxs-lookup"><span data-stu-id="7bce8-396">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="7bce8-397">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bce8-397">Property</span></span>         | <span data-ttu-id="7bce8-398">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bce8-398">Type</span></span>                                                     | <span data-ttu-id="7bce8-399">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7bce8-399">Required</span></span>                | <span data-ttu-id="7bce8-400">Valor</span><span class="sxs-lookup"><span data-stu-id="7bce8-400">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="7bce8-401">resourceId</span><span class="sxs-lookup"><span data-stu-id="7bce8-401">resourceId</span></span>       | <span data-ttu-id="7bce8-402">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7bce8-402">String</span></span>                                                   | <span data-ttu-id="7bce8-403">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-403">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="7bce8-404">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7bce8-404">roleDefinitionId</span></span> | <span data-ttu-id="7bce8-405">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-405">String</span></span>                                                   | <span data-ttu-id="7bce8-406">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-406">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="7bce8-407">subjectId</span><span class="sxs-lookup"><span data-stu-id="7bce8-407">subjectId</span></span>        | <span data-ttu-id="7bce8-408">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-408">String</span></span>                                                   | <span data-ttu-id="7bce8-409">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-409">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="7bce8-410">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7bce8-410">assignmentState</span></span>  | <span data-ttu-id="7bce8-411">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-411">String</span></span>                                                   | <span data-ttu-id="7bce8-412">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-412">Yes</span></span>                     | <span data-ttu-id="7bce8-413">Qualificado / Ativo</span><span class="sxs-lookup"><span data-stu-id="7bce8-413">Eligible / Active</span></span> |
| <span data-ttu-id="7bce8-414">type</span><span class="sxs-lookup"><span data-stu-id="7bce8-414">type</span></span>             | <span data-ttu-id="7bce8-415">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-415">String</span></span>                                                   | <span data-ttu-id="7bce8-416">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-416">Yes</span></span>                     | <span data-ttu-id="7bce8-417">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="7bce8-417">AdminExtend</span></span> |
| <span data-ttu-id="7bce8-418">motivo</span><span class="sxs-lookup"><span data-stu-id="7bce8-418">reason</span></span>           | <span data-ttu-id="7bce8-419">String</span><span class="sxs-lookup"><span data-stu-id="7bce8-419">String</span></span>                                                   | <span data-ttu-id="7bce8-420">depende de roleSettings</span><span class="sxs-lookup"><span data-stu-id="7bce8-420">depends on roleSettings</span></span> |   |
| <span data-ttu-id="7bce8-421">Cronograma</span><span class="sxs-lookup"><span data-stu-id="7bce8-421">schedule</span></span>         | [<span data-ttu-id="7bce8-422">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7bce8-422">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="7bce8-423">Sim</span><span class="sxs-lookup"><span data-stu-id="7bce8-423">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="7bce8-424">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bce8-424">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
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

#### <a name="response"></a><span data-ttu-id="7bce8-425">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bce8-425">Response</span></span>

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


