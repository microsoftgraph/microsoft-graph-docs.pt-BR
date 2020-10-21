---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: a76727ffd927f7d91b953c313b11a59e4512a65e
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634995"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="ec2f6-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="ec2f6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec2f6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec2f6-106">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="ec2f6-107">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-107">The following table lists the operations.</span></span>

| <span data-ttu-id="ec2f6-108">Operation</span><span class="sxs-lookup"><span data-stu-id="ec2f6-108">Operation</span></span>                                   | <span data-ttu-id="ec2f6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="ec2f6-110">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-110">Assign a role assignment</span></span>                    | <span data-ttu-id="ec2f6-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="ec2f6-111">AdminAdd</span></span>    |
| <span data-ttu-id="ec2f6-112">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="ec2f6-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="ec2f6-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="ec2f6-113">UserAdd</span></span>     |
| <span data-ttu-id="ec2f6-114">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="ec2f6-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="ec2f6-115">Userremove</span><span class="sxs-lookup"><span data-stu-id="ec2f6-115">UserRemove</span></span>  |
| <span data-ttu-id="ec2f6-116">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-116">Remove a role assignment</span></span>                    | <span data-ttu-id="ec2f6-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="ec2f6-117">AdminRemove</span></span> |
| <span data-ttu-id="ec2f6-118">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-118">Update a role assignment</span></span>                    | <span data-ttu-id="ec2f6-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-119">AdminUpdate</span></span> |
| <span data-ttu-id="ec2f6-120">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="ec2f6-121">Userextend</span><span class="sxs-lookup"><span data-stu-id="ec2f6-121">UserExtend</span></span>  |
| <span data-ttu-id="ec2f6-122">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-122">Extend a role assignment</span></span>                    | <span data-ttu-id="ec2f6-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="ec2f6-123">AdminExtend</span></span> |
| <span data-ttu-id="ec2f6-124">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="ec2f6-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="ec2f6-125">Userrenew</span><span class="sxs-lookup"><span data-stu-id="ec2f6-125">UserRenew</span></span>   |
| <span data-ttu-id="ec2f6-126">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="ec2f6-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="ec2f6-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="ec2f6-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="ec2f6-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec2f6-128">Permissions</span></span>

<span data-ttu-id="ec2f6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference#privileged-access-permissions).</span><span class="sxs-lookup"><span data-stu-id="ec2f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

### <a name="azure-resources"></a><span data-ttu-id="ec2f6-131">Recursos do Azure</span><span class="sxs-lookup"><span data-stu-id="ec2f6-131">Azure resources</span></span>

| <span data-ttu-id="ec2f6-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec2f6-132">Permission type</span></span> | <span data-ttu-id="ec2f6-133">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec2f6-133">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="ec2f6-134">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec2f6-134">Delegated (work or school account)</span></span> | <span data-ttu-id="ec2f6-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="ec2f6-135">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="ec2f6-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec2f6-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec2f6-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-137">Not supported.</span></span> |
| <span data-ttu-id="ec2f6-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-138">Application</span></span> | <span data-ttu-id="ec2f6-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-139">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="ec2f6-140">Azure AD</span><span class="sxs-lookup"><span data-stu-id="ec2f6-140">Azure AD</span></span>

| <span data-ttu-id="ec2f6-141">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec2f6-141">Permission type</span></span> | <span data-ttu-id="ec2f6-142">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec2f6-142">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="ec2f6-143">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec2f6-143">Delegated (work or school account)</span></span> | <span data-ttu-id="ec2f6-144">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="ec2f6-144">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="ec2f6-145">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec2f6-145">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec2f6-146">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-146">Not supported.</span></span> |
| <span data-ttu-id="ec2f6-147">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-147">Application</span></span> | <span data-ttu-id="ec2f6-148">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-148">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="ec2f6-149">Grupos</span><span class="sxs-lookup"><span data-stu-id="ec2f6-149">Groups</span></span>

|<span data-ttu-id="ec2f6-150">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec2f6-150">Permission type</span></span> | <span data-ttu-id="ec2f6-151">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec2f6-151">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="ec2f6-152">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec2f6-152">Delegated (work or school account)</span></span> | <span data-ttu-id="ec2f6-153">PrivilegedAccess. ReadWrite. AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="ec2f6-153">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="ec2f6-154">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec2f6-154">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec2f6-155">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-155">Not supported.</span></span> |
| <span data-ttu-id="ec2f6-156">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-156">Application</span></span> | <span data-ttu-id="ec2f6-157">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-157">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec2f6-158">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec2f6-158">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="ec2f6-159">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec2f6-159">Request headers</span></span>

| <span data-ttu-id="ec2f6-160">Nome</span><span class="sxs-lookup"><span data-stu-id="ec2f6-160">Name</span></span>          | <span data-ttu-id="ec2f6-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec2f6-161">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="ec2f6-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec2f6-162">Authorization</span></span> | <span data-ttu-id="ec2f6-163">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="ec2f6-163">Bearer {code}</span></span>    |
| <span data-ttu-id="ec2f6-164">Content-type</span><span class="sxs-lookup"><span data-stu-id="ec2f6-164">Content-type</span></span>  | <span data-ttu-id="ec2f6-165">application/json</span><span class="sxs-lookup"><span data-stu-id="ec2f6-165">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec2f6-166">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec2f6-166">Request body</span></span>

<span data-ttu-id="ec2f6-167">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ec2f6-167">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="ec2f6-168">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec2f6-168">Property</span></span>         | <span data-ttu-id="ec2f6-169">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-169">Type</span></span>                                                     | <span data-ttu-id="ec2f6-170">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec2f6-170">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="ec2f6-171">resourceId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-171">resourceId</span></span>       | <span data-ttu-id="ec2f6-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec2f6-172">String</span></span>                                                   | <span data-ttu-id="ec2f6-173">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-173">The ID of the resource.</span></span> <span data-ttu-id="ec2f6-174">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-174">Required.</span></span> |
| <span data-ttu-id="ec2f6-175">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-175">roleDefinitionId</span></span> | <span data-ttu-id="ec2f6-176">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-176">String</span></span>                                                   | <span data-ttu-id="ec2f6-177">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-177">The ID of the role definition.</span></span> <span data-ttu-id="ec2f6-178">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-178">Required.</span></span> |
| <span data-ttu-id="ec2f6-179">SubjectID</span><span class="sxs-lookup"><span data-stu-id="ec2f6-179">subjectId</span></span>        | <span data-ttu-id="ec2f6-180">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-180">String</span></span>                                                   | <span data-ttu-id="ec2f6-181">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-181">The ID of the subject.</span></span> <span data-ttu-id="ec2f6-182">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-182">Required.</span></span> |
| <span data-ttu-id="ec2f6-183">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-183">assignmentState</span></span>  | <span data-ttu-id="ec2f6-184">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-184">String</span></span>                                                   | <span data-ttu-id="ec2f6-185">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-185">The state of assignment.</span></span> <span data-ttu-id="ec2f6-186">O valor pode ser `Eligible` e `Active` .</span><span class="sxs-lookup"><span data-stu-id="ec2f6-186">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="ec2f6-187">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-187">Required.</span></span> |
| <span data-ttu-id="ec2f6-188">type</span><span class="sxs-lookup"><span data-stu-id="ec2f6-188">type</span></span>             | <span data-ttu-id="ec2f6-189">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-189">String</span></span>                                                   | <span data-ttu-id="ec2f6-190">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-190">The request type.</span></span> <span data-ttu-id="ec2f6-191">O valor pode ser,,,,,, `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` e `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="ec2f6-191">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="ec2f6-192">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-192">Required.</span></span> |
| <span data-ttu-id="ec2f6-193">motivo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-193">reason</span></span>           | <span data-ttu-id="ec2f6-194">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-194">String</span></span>                                                   | <span data-ttu-id="ec2f6-195">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-195">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="ec2f6-196">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ec2f6-196">schedule</span></span>         | [<span data-ttu-id="ec2f6-197">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ec2f6-197">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="ec2f6-198">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-198">The schedule of the role assignment request.</span></span> <span data-ttu-id="ec2f6-199">Para o tipo de solicitação de,,, `UserAdd` `AdminAdd` `AdminUpdate` e `AdminExtend` , é necessário.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-199">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="ec2f6-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec2f6-200">Response</span></span>

<span data-ttu-id="ec2f6-201">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-201">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="ec2f6-202">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="ec2f6-202">Error codes</span></span>

<span data-ttu-id="ec2f6-203">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-203">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="ec2f6-204">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-204">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="ec2f6-205">Código de erro</span><span class="sxs-lookup"><span data-stu-id="ec2f6-205">Error code</span></span>     | <span data-ttu-id="ec2f6-206">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="ec2f6-206">Error message</span></span>                               | <span data-ttu-id="ec2f6-207">Detalhes</span><span class="sxs-lookup"><span data-stu-id="ec2f6-207">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="ec2f6-208">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-208">400 BadRequest</span></span> | <span data-ttu-id="ec2f6-209">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="ec2f6-209">RoleNotFound</span></span>                                | <span data-ttu-id="ec2f6-210">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-210">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="ec2f6-211">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-211">400 BadRequest</span></span> | <span data-ttu-id="ec2f6-212">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="ec2f6-212">ResourceIsLocked</span></span>                            | <span data-ttu-id="ec2f6-213">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-213">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="ec2f6-214">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-214">400 BadRequest</span></span> | <span data-ttu-id="ec2f6-215">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="ec2f6-215">SubjectNotFound</span></span>                             | <span data-ttu-id="ec2f6-216">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-216">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="ec2f6-217">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-217">400 BadRequest</span></span> | <span data-ttu-id="ec2f6-218">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-218">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="ec2f6-219">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-219">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="ec2f6-220">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-220">400 BadRequest</span></span> | <span data-ttu-id="ec2f6-221">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="ec2f6-221">RoleAssignmentExists</span></span>                        | <span data-ttu-id="ec2f6-222">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-222">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="ec2f6-223">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-223">400 BadRequest</span></span> | <span data-ttu-id="ec2f6-224">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="ec2f6-224">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="ec2f6-225">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-225">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="ec2f6-226">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="ec2f6-226">400 BadRequest</span></span> | <span data-ttu-id="ec2f6-227">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="ec2f6-227">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="ec2f6-228">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-228">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="ec2f6-229">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ec2f6-229">Examples</span></span>

<span data-ttu-id="ec2f6-230">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-230">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="ec2f6-231">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-231">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="ec2f6-232">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-232">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="ec2f6-233">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-233">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="ec2f6-234">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec2f6-234">Property</span></span>         | <span data-ttu-id="ec2f6-235">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-235">Type</span></span>                                                     | <span data-ttu-id="ec2f6-236">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="ec2f6-236">Required</span></span>                 | <span data-ttu-id="ec2f6-237">Valor</span><span class="sxs-lookup"><span data-stu-id="ec2f6-237">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="ec2f6-238">resourceId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-238">resourceId</span></span>       | <span data-ttu-id="ec2f6-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec2f6-239">String</span></span>                                                   | <span data-ttu-id="ec2f6-240">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-240">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="ec2f6-241">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-241">roleDefinitionId</span></span> | <span data-ttu-id="ec2f6-242">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-242">String</span></span>                                                   | <span data-ttu-id="ec2f6-243">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-243">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="ec2f6-244">SubjectID</span><span class="sxs-lookup"><span data-stu-id="ec2f6-244">subjectId</span></span>        | <span data-ttu-id="ec2f6-245">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-245">String</span></span>                                                   | <span data-ttu-id="ec2f6-246">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-246">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="ec2f6-247">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-247">assignmentState</span></span>  | <span data-ttu-id="ec2f6-248">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-248">String</span></span>                                                   | <span data-ttu-id="ec2f6-249">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-249">Yes</span></span>                      | <span data-ttu-id="ec2f6-250">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-250">Eligible / Active</span></span> |
| <span data-ttu-id="ec2f6-251">type</span><span class="sxs-lookup"><span data-stu-id="ec2f6-251">type</span></span>             | <span data-ttu-id="ec2f6-252">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-252">String</span></span>                                                   | <span data-ttu-id="ec2f6-253">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-253">Yes</span></span>                      | <span data-ttu-id="ec2f6-254">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="ec2f6-254">AdminAdd</span></span> |
| <span data-ttu-id="ec2f6-255">motivo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-255">reason</span></span>           | <span data-ttu-id="ec2f6-256">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-256">String</span></span>                                                   | <span data-ttu-id="ec2f6-257">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-257">depends on role Settings</span></span> |   |
| <span data-ttu-id="ec2f6-258">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ec2f6-258">schedule</span></span>         | [<span data-ttu-id="ec2f6-259">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ec2f6-259">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="ec2f6-260">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-260">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="ec2f6-261">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec2f6-261">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ec2f6-262">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec2f6-262">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ec2f6-263">C#</span><span class="sxs-lookup"><span data-stu-id="ec2f6-263">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec2f6-264">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec2f6-264">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec2f6-265">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec2f6-265">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="ec2f6-266">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec2f6-266">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="ec2f6-267">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="ec2f6-267">Example 2: User activates eligible role</span></span>

<span data-ttu-id="ec2f6-268">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-268">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="ec2f6-269">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec2f6-269">Property</span></span>         | <span data-ttu-id="ec2f6-270">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-270">Type</span></span>                                                     | <span data-ttu-id="ec2f6-271">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="ec2f6-271">Required</span></span>                 | <span data-ttu-id="ec2f6-272">Valor</span><span class="sxs-lookup"><span data-stu-id="ec2f6-272">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="ec2f6-273">resourceId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-273">resourceId</span></span>       | <span data-ttu-id="ec2f6-274">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec2f6-274">String</span></span>                                                   | <span data-ttu-id="ec2f6-275">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-275">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="ec2f6-276">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-276">roleDefinitionId</span></span> | <span data-ttu-id="ec2f6-277">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-277">String</span></span>                                                   | <span data-ttu-id="ec2f6-278">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-278">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="ec2f6-279">SubjectID</span><span class="sxs-lookup"><span data-stu-id="ec2f6-279">subjectId</span></span>        | <span data-ttu-id="ec2f6-280">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-280">String</span></span>                                                   | <span data-ttu-id="ec2f6-281">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-281">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="ec2f6-282">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-282">assignmentState</span></span>  | <span data-ttu-id="ec2f6-283">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-283">String</span></span>                                                   | <span data-ttu-id="ec2f6-284">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-284">Yes</span></span>                      | <span data-ttu-id="ec2f6-285">Ativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-285">Active</span></span> |
| <span data-ttu-id="ec2f6-286">type</span><span class="sxs-lookup"><span data-stu-id="ec2f6-286">type</span></span>             | <span data-ttu-id="ec2f6-287">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-287">String</span></span>                                                   | <span data-ttu-id="ec2f6-288">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-288">Yes</span></span>                      | <span data-ttu-id="ec2f6-289">UserAdd</span><span class="sxs-lookup"><span data-stu-id="ec2f6-289">UserAdd</span></span> |
| <span data-ttu-id="ec2f6-290">motivo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-290">reason</span></span>           | <span data-ttu-id="ec2f6-291">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-291">String</span></span>                                                   | <span data-ttu-id="ec2f6-292">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-292">depends on role Settings</span></span> |   |
| <span data-ttu-id="ec2f6-293">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ec2f6-293">schedule</span></span>         | [<span data-ttu-id="ec2f6-294">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ec2f6-294">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="ec2f6-295">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-295">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="ec2f6-296">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec2f6-296">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="ec2f6-297">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec2f6-297">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="ec2f6-298">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="ec2f6-298">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="ec2f6-299">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-299">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="ec2f6-300">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec2f6-300">Property</span></span>         | <span data-ttu-id="ec2f6-301">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-301">Type</span></span>                                                     | <span data-ttu-id="ec2f6-302">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="ec2f6-302">Required</span></span> | <span data-ttu-id="ec2f6-303">Valor</span><span class="sxs-lookup"><span data-stu-id="ec2f6-303">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="ec2f6-304">resourceId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-304">resourceId</span></span>       | <span data-ttu-id="ec2f6-305">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec2f6-305">String</span></span>                                                   | <span data-ttu-id="ec2f6-306">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-306">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="ec2f6-307">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-307">roleDefinitionId</span></span> | <span data-ttu-id="ec2f6-308">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-308">String</span></span>                                                   | <span data-ttu-id="ec2f6-309">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-309">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="ec2f6-310">SubjectID</span><span class="sxs-lookup"><span data-stu-id="ec2f6-310">subjectId</span></span>        | <span data-ttu-id="ec2f6-311">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-311">String</span></span>                                                   | <span data-ttu-id="ec2f6-312">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-312">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="ec2f6-313">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-313">assignmentState</span></span>  | <span data-ttu-id="ec2f6-314">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-314">String</span></span>                                                   | <span data-ttu-id="ec2f6-315">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-315">Yes</span></span>      | <span data-ttu-id="ec2f6-316">Ativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-316">Active</span></span> |
| <span data-ttu-id="ec2f6-317">type</span><span class="sxs-lookup"><span data-stu-id="ec2f6-317">type</span></span>             | <span data-ttu-id="ec2f6-318">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-318">String</span></span>                                                   | <span data-ttu-id="ec2f6-319">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-319">Yes</span></span>      | <span data-ttu-id="ec2f6-320">Userremove</span><span class="sxs-lookup"><span data-stu-id="ec2f6-320">UserRemove</span></span> |
| <span data-ttu-id="ec2f6-321">motivo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-321">reason</span></span>           | <span data-ttu-id="ec2f6-322">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-322">String</span></span>                                                   | <span data-ttu-id="ec2f6-323">Não</span><span class="sxs-lookup"><span data-stu-id="ec2f6-323">No</span></span>       |   |
| <span data-ttu-id="ec2f6-324">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ec2f6-324">schedule</span></span>         | [<span data-ttu-id="ec2f6-325">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ec2f6-325">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="ec2f6-326">Não</span><span class="sxs-lookup"><span data-stu-id="ec2f6-326">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="ec2f6-327">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec2f6-327">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="ec2f6-328">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec2f6-328">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="ec2f6-329">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="ec2f6-329">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="ec2f6-330">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-330">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="ec2f6-331">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-331">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="ec2f6-332">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec2f6-332">Property</span></span>         | <span data-ttu-id="ec2f6-333">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-333">Type</span></span>                                                     | <span data-ttu-id="ec2f6-334">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="ec2f6-334">Required</span></span> | <span data-ttu-id="ec2f6-335">Valor</span><span class="sxs-lookup"><span data-stu-id="ec2f6-335">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="ec2f6-336">resourceId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-336">resourceId</span></span>       | <span data-ttu-id="ec2f6-337">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec2f6-337">String</span></span>                                                   | <span data-ttu-id="ec2f6-338">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-338">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="ec2f6-339">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-339">roleDefinitionId</span></span> | <span data-ttu-id="ec2f6-340">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-340">String</span></span>                                                   | <span data-ttu-id="ec2f6-341">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-341">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="ec2f6-342">SubjectID</span><span class="sxs-lookup"><span data-stu-id="ec2f6-342">subjectId</span></span>        | <span data-ttu-id="ec2f6-343">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-343">String</span></span>                                                   | <span data-ttu-id="ec2f6-344">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-344">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="ec2f6-345">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-345">assignmentState</span></span>  | <span data-ttu-id="ec2f6-346">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-346">String</span></span>                                                   | <span data-ttu-id="ec2f6-347">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-347">Yes</span></span>      | <span data-ttu-id="ec2f6-348">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-348">Eligible / Active</span></span> |
| <span data-ttu-id="ec2f6-349">type</span><span class="sxs-lookup"><span data-stu-id="ec2f6-349">type</span></span>             | <span data-ttu-id="ec2f6-350">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-350">String</span></span>                                                   | <span data-ttu-id="ec2f6-351">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-351">Yes</span></span>      | <span data-ttu-id="ec2f6-352">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="ec2f6-352">AdminRemove</span></span> |
| <span data-ttu-id="ec2f6-353">motivo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-353">reason</span></span>           | <span data-ttu-id="ec2f6-354">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-354">String</span></span>                                                   | <span data-ttu-id="ec2f6-355">Não</span><span class="sxs-lookup"><span data-stu-id="ec2f6-355">No</span></span>       |   |
| <span data-ttu-id="ec2f6-356">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ec2f6-356">schedule</span></span>         | [<span data-ttu-id="ec2f6-357">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ec2f6-357">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="ec2f6-358">Não</span><span class="sxs-lookup"><span data-stu-id="ec2f6-358">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="ec2f6-359">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec2f6-359">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="ec2f6-360">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec2f6-360">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="ec2f6-361">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="ec2f6-361">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="ec2f6-362">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-362">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="ec2f6-363">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-363">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="ec2f6-364">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec2f6-364">Property</span></span>         | <span data-ttu-id="ec2f6-365">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-365">Type</span></span>                                                     | <span data-ttu-id="ec2f6-366">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="ec2f6-366">Required</span></span>                | <span data-ttu-id="ec2f6-367">Valor</span><span class="sxs-lookup"><span data-stu-id="ec2f6-367">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="ec2f6-368">resourceId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-368">resourceId</span></span>       | <span data-ttu-id="ec2f6-369">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec2f6-369">String</span></span>                                                   | <span data-ttu-id="ec2f6-370">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-370">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="ec2f6-371">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-371">roleDefinitionId</span></span> | <span data-ttu-id="ec2f6-372">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-372">String</span></span>                                                   | <span data-ttu-id="ec2f6-373">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-373">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="ec2f6-374">SubjectID</span><span class="sxs-lookup"><span data-stu-id="ec2f6-374">subjectId</span></span>        | <span data-ttu-id="ec2f6-375">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-375">String</span></span>                                                   | <span data-ttu-id="ec2f6-376">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-376">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="ec2f6-377">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-377">assignmentState</span></span>  | <span data-ttu-id="ec2f6-378">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-378">String</span></span>                                                   | <span data-ttu-id="ec2f6-379">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-379">Yes</span></span>                     | <span data-ttu-id="ec2f6-380">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-380">Eligible / Active</span></span> |
| <span data-ttu-id="ec2f6-381">type</span><span class="sxs-lookup"><span data-stu-id="ec2f6-381">type</span></span>             | <span data-ttu-id="ec2f6-382">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-382">String</span></span>                                                   | <span data-ttu-id="ec2f6-383">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-383">Yes</span></span>                     | <span data-ttu-id="ec2f6-384">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-384">AdminUpdate</span></span> |
| <span data-ttu-id="ec2f6-385">motivo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-385">reason</span></span>           | <span data-ttu-id="ec2f6-386">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-386">String</span></span>                                                   | <span data-ttu-id="ec2f6-387">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="ec2f6-387">depends on roleSettings</span></span> |   |
| <span data-ttu-id="ec2f6-388">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ec2f6-388">schedule</span></span>         | [<span data-ttu-id="ec2f6-389">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ec2f6-389">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="ec2f6-390">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-390">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="ec2f6-391">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec2f6-391">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="ec2f6-392">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec2f6-392">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="ec2f6-393">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="ec2f6-393">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="ec2f6-394">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-394">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="ec2f6-395">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="ec2f6-395">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="ec2f6-396">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec2f6-396">Property</span></span>         | <span data-ttu-id="ec2f6-397">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-397">Type</span></span>                                                     | <span data-ttu-id="ec2f6-398">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="ec2f6-398">Required</span></span>                | <span data-ttu-id="ec2f6-399">Valor</span><span class="sxs-lookup"><span data-stu-id="ec2f6-399">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="ec2f6-400">resourceId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-400">resourceId</span></span>       | <span data-ttu-id="ec2f6-401">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec2f6-401">String</span></span>                                                   | <span data-ttu-id="ec2f6-402">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-402">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="ec2f6-403">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ec2f6-403">roleDefinitionId</span></span> | <span data-ttu-id="ec2f6-404">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-404">String</span></span>                                                   | <span data-ttu-id="ec2f6-405">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-405">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="ec2f6-406">SubjectID</span><span class="sxs-lookup"><span data-stu-id="ec2f6-406">subjectId</span></span>        | <span data-ttu-id="ec2f6-407">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-407">String</span></span>                                                   | <span data-ttu-id="ec2f6-408">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-408">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="ec2f6-409">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="ec2f6-409">assignmentState</span></span>  | <span data-ttu-id="ec2f6-410">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-410">String</span></span>                                                   | <span data-ttu-id="ec2f6-411">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-411">Yes</span></span>                     | <span data-ttu-id="ec2f6-412">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-412">Eligible / Active</span></span> |
| <span data-ttu-id="ec2f6-413">type</span><span class="sxs-lookup"><span data-stu-id="ec2f6-413">type</span></span>             | <span data-ttu-id="ec2f6-414">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-414">String</span></span>                                                   | <span data-ttu-id="ec2f6-415">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-415">Yes</span></span>                     | <span data-ttu-id="ec2f6-416">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="ec2f6-416">AdminExtend</span></span> |
| <span data-ttu-id="ec2f6-417">motivo</span><span class="sxs-lookup"><span data-stu-id="ec2f6-417">reason</span></span>           | <span data-ttu-id="ec2f6-418">String</span><span class="sxs-lookup"><span data-stu-id="ec2f6-418">String</span></span>                                                   | <span data-ttu-id="ec2f6-419">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="ec2f6-419">depends on roleSettings</span></span> |   |
| <span data-ttu-id="ec2f6-420">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ec2f6-420">schedule</span></span>         | [<span data-ttu-id="ec2f6-421">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="ec2f6-421">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="ec2f6-422">Sim</span><span class="sxs-lookup"><span data-stu-id="ec2f6-422">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="ec2f6-423">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec2f6-423">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="ec2f6-424">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec2f6-424">Response</span></span>

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


