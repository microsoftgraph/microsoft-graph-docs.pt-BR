---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: b038ca74eb8046e4ae77a8a31715a473a3518ba1
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218868"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="cc004-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="cc004-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc004-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc004-106">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="cc004-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="cc004-107">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="cc004-107">The following table lists the operations.</span></span>

| <span data-ttu-id="cc004-108">Operation</span><span class="sxs-lookup"><span data-stu-id="cc004-108">Operation</span></span>                                   | <span data-ttu-id="cc004-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="cc004-110">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="cc004-110">Assign a role assignment</span></span>                    | <span data-ttu-id="cc004-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="cc004-111">AdminAdd</span></span>    |
| <span data-ttu-id="cc004-112">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="cc004-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="cc004-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="cc004-113">UserAdd</span></span>     |
| <span data-ttu-id="cc004-114">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="cc004-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="cc004-115">Userremove</span><span class="sxs-lookup"><span data-stu-id="cc004-115">UserRemove</span></span>  |
| <span data-ttu-id="cc004-116">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="cc004-116">Remove a role assignment</span></span>                    | <span data-ttu-id="cc004-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="cc004-117">AdminRemove</span></span> |
| <span data-ttu-id="cc004-118">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="cc004-118">Update a role assignment</span></span>                    | <span data-ttu-id="cc004-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="cc004-119">AdminUpdate</span></span> |
| <span data-ttu-id="cc004-120">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="cc004-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="cc004-121">Userextend</span><span class="sxs-lookup"><span data-stu-id="cc004-121">UserExtend</span></span>  |
| <span data-ttu-id="cc004-122">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="cc004-122">Extend a role assignment</span></span>                    | <span data-ttu-id="cc004-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="cc004-123">AdminExtend</span></span> |
| <span data-ttu-id="cc004-124">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="cc004-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="cc004-125">Userrenew</span><span class="sxs-lookup"><span data-stu-id="cc004-125">UserRenew</span></span>   |
| <span data-ttu-id="cc004-126">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="cc004-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="cc004-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="cc004-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="cc004-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc004-128">Permissions</span></span>

<span data-ttu-id="cc004-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc004-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc004-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc004-131">Permission type</span></span>                        | <span data-ttu-id="cc004-132">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc004-132">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="cc004-133">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc004-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc004-134">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="cc004-134">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="cc004-135">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc004-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc004-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc004-136">Not supported.</span></span>                            |
| <span data-ttu-id="cc004-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc004-137">Application</span></span>                            | <span data-ttu-id="cc004-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc004-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc004-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc004-139">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="cc004-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc004-140">Request headers</span></span>

| <span data-ttu-id="cc004-141">Nome</span><span class="sxs-lookup"><span data-stu-id="cc004-141">Name</span></span>          | <span data-ttu-id="cc004-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc004-142">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="cc004-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc004-143">Authorization</span></span> | <span data-ttu-id="cc004-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="cc004-144">Bearer {code}</span></span>    |
| <span data-ttu-id="cc004-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="cc004-145">Content-type</span></span>  | <span data-ttu-id="cc004-146">application/json</span><span class="sxs-lookup"><span data-stu-id="cc004-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc004-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc004-147">Request body</span></span>

<span data-ttu-id="cc004-148">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="cc004-148">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="cc004-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc004-149">Property</span></span>         | <span data-ttu-id="cc004-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-150">Type</span></span>                                                     | <span data-ttu-id="cc004-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc004-151">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="cc004-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc004-152">resourceId</span></span>       | <span data-ttu-id="cc004-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-153">String</span></span>                                                   | <span data-ttu-id="cc004-154">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc004-154">The ID of the resource.</span></span> <span data-ttu-id="cc004-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc004-155">Required.</span></span> |
| <span data-ttu-id="cc004-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc004-156">roleDefinitionId</span></span> | <span data-ttu-id="cc004-157">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-157">String</span></span>                                                   | <span data-ttu-id="cc004-158">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="cc004-158">The ID of the role definition.</span></span> <span data-ttu-id="cc004-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc004-159">Required.</span></span> |
| <span data-ttu-id="cc004-160">SubjectID</span><span class="sxs-lookup"><span data-stu-id="cc004-160">subjectId</span></span>        | <span data-ttu-id="cc004-161">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-161">String</span></span>                                                   | <span data-ttu-id="cc004-162">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="cc004-162">The ID of the subject.</span></span> <span data-ttu-id="cc004-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc004-163">Required.</span></span> |
| <span data-ttu-id="cc004-164">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="cc004-164">assignmentState</span></span>  | <span data-ttu-id="cc004-165">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-165">String</span></span>                                                   | <span data-ttu-id="cc004-166">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="cc004-166">The state of assignment.</span></span> <span data-ttu-id="cc004-167">O valor pode ser `Eligible` e `Active`.</span><span class="sxs-lookup"><span data-stu-id="cc004-167">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="cc004-168">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc004-168">Required.</span></span> |
| <span data-ttu-id="cc004-169">tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-169">type</span></span>             | <span data-ttu-id="cc004-170">String</span><span class="sxs-lookup"><span data-stu-id="cc004-170">String</span></span>                                                   | <span data-ttu-id="cc004-171">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc004-171">The request type.</span></span> <span data-ttu-id="cc004-172">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew`,,,, `AdminRenew`e. `AdminExtend`</span><span class="sxs-lookup"><span data-stu-id="cc004-172">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="cc004-173">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc004-173">Required.</span></span> |
| <span data-ttu-id="cc004-174">motivo</span><span class="sxs-lookup"><span data-stu-id="cc004-174">reason</span></span>           | <span data-ttu-id="cc004-175">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-175">String</span></span>                                                   | <span data-ttu-id="cc004-176">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="cc004-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="cc004-177">Cronograma</span><span class="sxs-lookup"><span data-stu-id="cc004-177">schedule</span></span>         | [<span data-ttu-id="cc004-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc004-178">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="cc004-179">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="cc004-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="cc004-180">Para o tipo de `UserAdd`solicitação `AdminAdd`de `AdminUpdate`,, `AdminExtend`, e, é necessário.</span><span class="sxs-lookup"><span data-stu-id="cc004-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="cc004-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc004-181">Response</span></span>

<span data-ttu-id="cc004-182">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc004-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="cc004-183">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="cc004-183">Error codes</span></span>

<span data-ttu-id="cc004-184">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="cc004-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="cc004-185">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="cc004-185">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="cc004-186">Código de erro</span><span class="sxs-lookup"><span data-stu-id="cc004-186">Error code</span></span>     | <span data-ttu-id="cc004-187">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="cc004-187">Error message</span></span>                               | <span data-ttu-id="cc004-188">Detalhes</span><span class="sxs-lookup"><span data-stu-id="cc004-188">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="cc004-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-189">400 BadRequest</span></span> | <span data-ttu-id="cc004-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="cc004-190">RoleNotFound</span></span>                                | <span data-ttu-id="cc004-191">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="cc004-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="cc004-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-192">400 BadRequest</span></span> | <span data-ttu-id="cc004-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="cc004-193">ResourceIsLocked</span></span>                            | <span data-ttu-id="cc004-194">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="cc004-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="cc004-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-195">400 BadRequest</span></span> | <span data-ttu-id="cc004-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="cc004-196">SubjectNotFound</span></span>                             | <span data-ttu-id="cc004-197">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="cc004-197">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="cc004-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-198">400 BadRequest</span></span> | <span data-ttu-id="cc004-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-199">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="cc004-200">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="cc004-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="cc004-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-201">400 BadRequest</span></span> | <span data-ttu-id="cc004-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="cc004-202">RoleAssignmentExists</span></span>                        | <span data-ttu-id="cc004-203">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="cc004-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="cc004-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-204">400 BadRequest</span></span> | <span data-ttu-id="cc004-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="cc004-205">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="cc004-206">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="cc004-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="cc004-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="cc004-207">400 BadRequest</span></span> | <span data-ttu-id="cc004-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="cc004-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="cc004-209">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="cc004-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="cc004-210">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cc004-210">Examples</span></span>

<span data-ttu-id="cc004-211">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="cc004-211">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="cc004-212">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="cc004-212">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="cc004-213">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="cc004-213">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="cc004-214">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="cc004-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="cc004-215">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc004-215">Property</span></span>         | <span data-ttu-id="cc004-216">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-216">Type</span></span>                                                     | <span data-ttu-id="cc004-217">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cc004-217">Required</span></span>                 | <span data-ttu-id="cc004-218">Valor</span><span class="sxs-lookup"><span data-stu-id="cc004-218">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="cc004-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc004-219">resourceId</span></span>       | <span data-ttu-id="cc004-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-220">String</span></span>                                                   | <span data-ttu-id="cc004-221">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-221">Yes</span></span>                      | <span data-ttu-id="cc004-222">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc004-222">\<resourceId\></span></span> |
| <span data-ttu-id="cc004-223">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc004-223">roleDefinitionId</span></span> | <span data-ttu-id="cc004-224">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-224">String</span></span>                                                   | <span data-ttu-id="cc004-225">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-225">Yes</span></span>                      | <span data-ttu-id="cc004-226">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc004-226">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="cc004-227">SubjectID</span><span class="sxs-lookup"><span data-stu-id="cc004-227">subjectId</span></span>        | <span data-ttu-id="cc004-228">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-228">String</span></span>                                                   | <span data-ttu-id="cc004-229">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-229">Yes</span></span>                      | <span data-ttu-id="cc004-230">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="cc004-230">\<subjectId\></span></span> |
| <span data-ttu-id="cc004-231">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="cc004-231">assignmentState</span></span>  | <span data-ttu-id="cc004-232">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-232">String</span></span>                                                   | <span data-ttu-id="cc004-233">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-233">Yes</span></span>                      | <span data-ttu-id="cc004-234">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="cc004-234">Eligible / Active</span></span> |
| <span data-ttu-id="cc004-235">tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-235">type</span></span>             | <span data-ttu-id="cc004-236">String</span><span class="sxs-lookup"><span data-stu-id="cc004-236">String</span></span>                                                   | <span data-ttu-id="cc004-237">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-237">Yes</span></span>                      | <span data-ttu-id="cc004-238">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="cc004-238">AdminAdd</span></span> |
| <span data-ttu-id="cc004-239">motivo</span><span class="sxs-lookup"><span data-stu-id="cc004-239">reason</span></span>           | <span data-ttu-id="cc004-240">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-240">String</span></span>                                                   | <span data-ttu-id="cc004-241">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="cc004-241">depends on role Settings</span></span> |   |
| <span data-ttu-id="cc004-242">Cronograma</span><span class="sxs-lookup"><span data-stu-id="cc004-242">schedule</span></span>         | [<span data-ttu-id="cc004-243">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc004-243">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="cc004-244">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-244">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="cc004-245">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc004-245">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cc004-246">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc004-246">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="cc004-247">C#</span><span class="sxs-lookup"><span data-stu-id="cc004-247">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc004-248">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc004-248">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc004-249">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc004-249">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="cc004-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc004-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="cc004-251">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="cc004-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="cc004-252">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="cc004-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="cc004-253">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc004-253">Property</span></span>         | <span data-ttu-id="cc004-254">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-254">Type</span></span>                                                     | <span data-ttu-id="cc004-255">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cc004-255">Required</span></span>                 | <span data-ttu-id="cc004-256">Valor</span><span class="sxs-lookup"><span data-stu-id="cc004-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="cc004-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc004-257">resourceId</span></span>       | <span data-ttu-id="cc004-258">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-258">String</span></span>                                                   | <span data-ttu-id="cc004-259">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-259">Yes</span></span>                      | <span data-ttu-id="cc004-260">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc004-260">\<resourceId\></span></span> |
| <span data-ttu-id="cc004-261">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc004-261">roleDefinitionId</span></span> | <span data-ttu-id="cc004-262">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-262">String</span></span>                                                   | <span data-ttu-id="cc004-263">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-263">Yes</span></span>                      | <span data-ttu-id="cc004-264">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc004-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="cc004-265">SubjectID</span><span class="sxs-lookup"><span data-stu-id="cc004-265">subjectId</span></span>        | <span data-ttu-id="cc004-266">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-266">String</span></span>                                                   | <span data-ttu-id="cc004-267">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-267">Yes</span></span>                      | <span data-ttu-id="cc004-268">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="cc004-268">\<subjectId\></span></span> |
| <span data-ttu-id="cc004-269">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="cc004-269">assignmentState</span></span>  | <span data-ttu-id="cc004-270">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-270">String</span></span>                                                   | <span data-ttu-id="cc004-271">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-271">Yes</span></span>                      | <span data-ttu-id="cc004-272">Ativo</span><span class="sxs-lookup"><span data-stu-id="cc004-272">Active</span></span> |
| <span data-ttu-id="cc004-273">tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-273">type</span></span>             | <span data-ttu-id="cc004-274">String</span><span class="sxs-lookup"><span data-stu-id="cc004-274">String</span></span>                                                   | <span data-ttu-id="cc004-275">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-275">Yes</span></span>                      | <span data-ttu-id="cc004-276">UserAdd</span><span class="sxs-lookup"><span data-stu-id="cc004-276">UserAdd</span></span> |
| <span data-ttu-id="cc004-277">motivo</span><span class="sxs-lookup"><span data-stu-id="cc004-277">reason</span></span>           | <span data-ttu-id="cc004-278">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-278">String</span></span>                                                   | <span data-ttu-id="cc004-279">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="cc004-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="cc004-280">Cronograma</span><span class="sxs-lookup"><span data-stu-id="cc004-280">schedule</span></span>         | [<span data-ttu-id="cc004-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc004-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="cc004-282">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="cc004-283">Solicitar</span><span class="sxs-lookup"><span data-stu-id="cc004-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cc004-284">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc004-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="cc004-285">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="cc004-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="cc004-286">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="cc004-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="cc004-287">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc004-287">Property</span></span>         | <span data-ttu-id="cc004-288">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-288">Type</span></span>                                                     | <span data-ttu-id="cc004-289">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cc004-289">Required</span></span> | <span data-ttu-id="cc004-290">Valor</span><span class="sxs-lookup"><span data-stu-id="cc004-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="cc004-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc004-291">resourceId</span></span>       | <span data-ttu-id="cc004-292">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-292">String</span></span>                                                   | <span data-ttu-id="cc004-293">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-293">Yes</span></span>      | <span data-ttu-id="cc004-294">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc004-294">\<resourceId\></span></span> |
| <span data-ttu-id="cc004-295">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc004-295">roleDefinitionId</span></span> | <span data-ttu-id="cc004-296">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-296">String</span></span>                                                   | <span data-ttu-id="cc004-297">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-297">Yes</span></span>      | <span data-ttu-id="cc004-298">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc004-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="cc004-299">SubjectID</span><span class="sxs-lookup"><span data-stu-id="cc004-299">subjectId</span></span>        | <span data-ttu-id="cc004-300">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-300">String</span></span>                                                   | <span data-ttu-id="cc004-301">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-301">Yes</span></span>      | <span data-ttu-id="cc004-302">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="cc004-302">\<subjectId\></span></span> |
| <span data-ttu-id="cc004-303">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="cc004-303">assignmentState</span></span>  | <span data-ttu-id="cc004-304">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-304">String</span></span>                                                   | <span data-ttu-id="cc004-305">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-305">Yes</span></span>      | <span data-ttu-id="cc004-306">Ativo</span><span class="sxs-lookup"><span data-stu-id="cc004-306">Active</span></span> |
| <span data-ttu-id="cc004-307">tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-307">type</span></span>             | <span data-ttu-id="cc004-308">String</span><span class="sxs-lookup"><span data-stu-id="cc004-308">String</span></span>                                                   | <span data-ttu-id="cc004-309">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-309">Yes</span></span>      | <span data-ttu-id="cc004-310">Userremove</span><span class="sxs-lookup"><span data-stu-id="cc004-310">UserRemove</span></span> |
| <span data-ttu-id="cc004-311">motivo</span><span class="sxs-lookup"><span data-stu-id="cc004-311">reason</span></span>           | <span data-ttu-id="cc004-312">String</span><span class="sxs-lookup"><span data-stu-id="cc004-312">String</span></span>                                                   | <span data-ttu-id="cc004-313">Não</span><span class="sxs-lookup"><span data-stu-id="cc004-313">No</span></span>       |   |
| <span data-ttu-id="cc004-314">Cronograma</span><span class="sxs-lookup"><span data-stu-id="cc004-314">schedule</span></span>         | [<span data-ttu-id="cc004-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc004-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="cc004-316">Não</span><span class="sxs-lookup"><span data-stu-id="cc004-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="cc004-317">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc004-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cc004-318">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc004-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="cc004-319">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="cc004-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="cc004-320">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="cc004-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="cc004-321">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="cc004-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="cc004-322">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc004-322">Property</span></span>         | <span data-ttu-id="cc004-323">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-323">Type</span></span>                                                     | <span data-ttu-id="cc004-324">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cc004-324">Required</span></span> | <span data-ttu-id="cc004-325">Valor</span><span class="sxs-lookup"><span data-stu-id="cc004-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="cc004-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc004-326">resourceId</span></span>       | <span data-ttu-id="cc004-327">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-327">String</span></span>                                                   | <span data-ttu-id="cc004-328">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-328">Yes</span></span>      | <span data-ttu-id="cc004-329">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc004-329">\<resourceId\></span></span> |
| <span data-ttu-id="cc004-330">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc004-330">roleDefinitionId</span></span> | <span data-ttu-id="cc004-331">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-331">String</span></span>                                                   | <span data-ttu-id="cc004-332">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-332">Yes</span></span>      | <span data-ttu-id="cc004-333">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc004-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="cc004-334">SubjectID</span><span class="sxs-lookup"><span data-stu-id="cc004-334">subjectId</span></span>        | <span data-ttu-id="cc004-335">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-335">String</span></span>                                                   | <span data-ttu-id="cc004-336">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-336">Yes</span></span>      | <span data-ttu-id="cc004-337">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="cc004-337">\<subjectId\></span></span> |
| <span data-ttu-id="cc004-338">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="cc004-338">assignmentState</span></span>  | <span data-ttu-id="cc004-339">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-339">String</span></span>                                                   | <span data-ttu-id="cc004-340">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-340">Yes</span></span>      | <span data-ttu-id="cc004-341">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="cc004-341">Eligible / Active</span></span> |
| <span data-ttu-id="cc004-342">tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-342">type</span></span>             | <span data-ttu-id="cc004-343">String</span><span class="sxs-lookup"><span data-stu-id="cc004-343">String</span></span>                                                   | <span data-ttu-id="cc004-344">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-344">Yes</span></span>      | <span data-ttu-id="cc004-345">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="cc004-345">AdminRemove</span></span> |
| <span data-ttu-id="cc004-346">motivo</span><span class="sxs-lookup"><span data-stu-id="cc004-346">reason</span></span>           | <span data-ttu-id="cc004-347">String</span><span class="sxs-lookup"><span data-stu-id="cc004-347">String</span></span>                                                   | <span data-ttu-id="cc004-348">Não</span><span class="sxs-lookup"><span data-stu-id="cc004-348">No</span></span>       |   |
| <span data-ttu-id="cc004-349">Cronograma</span><span class="sxs-lookup"><span data-stu-id="cc004-349">schedule</span></span>         | [<span data-ttu-id="cc004-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc004-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="cc004-351">Não</span><span class="sxs-lookup"><span data-stu-id="cc004-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="cc004-352">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc004-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cc004-353">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc004-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="cc004-354">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="cc004-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="cc004-355">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="cc004-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="cc004-356">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="cc004-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="cc004-357">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc004-357">Property</span></span>         | <span data-ttu-id="cc004-358">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-358">Type</span></span>                                                     | <span data-ttu-id="cc004-359">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cc004-359">Required</span></span>                | <span data-ttu-id="cc004-360">Valor</span><span class="sxs-lookup"><span data-stu-id="cc004-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="cc004-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc004-361">resourceId</span></span>       | <span data-ttu-id="cc004-362">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-362">String</span></span>                                                   | <span data-ttu-id="cc004-363">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-363">Yes</span></span>                     | <span data-ttu-id="cc004-364">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc004-364">\<resourceId\></span></span> |
| <span data-ttu-id="cc004-365">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc004-365">roleDefinitionId</span></span> | <span data-ttu-id="cc004-366">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-366">String</span></span>                                                   | <span data-ttu-id="cc004-367">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-367">Yes</span></span>                     | <span data-ttu-id="cc004-368">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc004-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="cc004-369">SubjectID</span><span class="sxs-lookup"><span data-stu-id="cc004-369">subjectId</span></span>        | <span data-ttu-id="cc004-370">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-370">String</span></span>                                                   | <span data-ttu-id="cc004-371">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-371">Yes</span></span>                     | <span data-ttu-id="cc004-372">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="cc004-372">\<subjectId\></span></span> |
| <span data-ttu-id="cc004-373">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="cc004-373">assignmentState</span></span>  | <span data-ttu-id="cc004-374">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-374">String</span></span>                                                   | <span data-ttu-id="cc004-375">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-375">Yes</span></span>                     | <span data-ttu-id="cc004-376">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="cc004-376">Eligible / Active</span></span> |
| <span data-ttu-id="cc004-377">tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-377">type</span></span>             | <span data-ttu-id="cc004-378">String</span><span class="sxs-lookup"><span data-stu-id="cc004-378">String</span></span>                                                   | <span data-ttu-id="cc004-379">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-379">Yes</span></span>                     | <span data-ttu-id="cc004-380">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="cc004-380">AdminUpdate</span></span> |
| <span data-ttu-id="cc004-381">motivo</span><span class="sxs-lookup"><span data-stu-id="cc004-381">reason</span></span>           | <span data-ttu-id="cc004-382">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-382">String</span></span>                                                   | <span data-ttu-id="cc004-383">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="cc004-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="cc004-384">Cronograma</span><span class="sxs-lookup"><span data-stu-id="cc004-384">schedule</span></span>         | [<span data-ttu-id="cc004-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc004-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="cc004-386">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="cc004-387">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc004-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cc004-388">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc004-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="cc004-389">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="cc004-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="cc004-390">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="cc004-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="cc004-391">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="cc004-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="cc004-392">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc004-392">Property</span></span>         | <span data-ttu-id="cc004-393">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-393">Type</span></span>                                                     | <span data-ttu-id="cc004-394">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cc004-394">Required</span></span>                | <span data-ttu-id="cc004-395">Valor</span><span class="sxs-lookup"><span data-stu-id="cc004-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="cc004-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="cc004-396">resourceId</span></span>       | <span data-ttu-id="cc004-397">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-397">String</span></span>                                                   | <span data-ttu-id="cc004-398">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-398">Yes</span></span>                     | <span data-ttu-id="cc004-399">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="cc004-399">\<resourceId\></span></span> |
| <span data-ttu-id="cc004-400">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="cc004-400">roleDefinitionId</span></span> | <span data-ttu-id="cc004-401">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-401">String</span></span>                                                   | <span data-ttu-id="cc004-402">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-402">Yes</span></span>                     | <span data-ttu-id="cc004-403">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="cc004-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="cc004-404">SubjectID</span><span class="sxs-lookup"><span data-stu-id="cc004-404">subjectId</span></span>        | <span data-ttu-id="cc004-405">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-405">String</span></span>                                                   | <span data-ttu-id="cc004-406">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-406">Yes</span></span>                     | <span data-ttu-id="cc004-407">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="cc004-407">\<subjectId\></span></span> |
| <span data-ttu-id="cc004-408">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="cc004-408">assignmentState</span></span>  | <span data-ttu-id="cc004-409">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-409">String</span></span>                                                   | <span data-ttu-id="cc004-410">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-410">Yes</span></span>                     | <span data-ttu-id="cc004-411">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="cc004-411">Eligible / Active</span></span> |
| <span data-ttu-id="cc004-412">tipo</span><span class="sxs-lookup"><span data-stu-id="cc004-412">type</span></span>             | <span data-ttu-id="cc004-413">String</span><span class="sxs-lookup"><span data-stu-id="cc004-413">String</span></span>                                                   | <span data-ttu-id="cc004-414">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-414">Yes</span></span>                     | <span data-ttu-id="cc004-415">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="cc004-415">AdminExtend</span></span> |
| <span data-ttu-id="cc004-416">motivo</span><span class="sxs-lookup"><span data-stu-id="cc004-416">reason</span></span>           | <span data-ttu-id="cc004-417">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="cc004-417">String</span></span>                                                   | <span data-ttu-id="cc004-418">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="cc004-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="cc004-419">Cronograma</span><span class="sxs-lookup"><span data-stu-id="cc004-419">schedule</span></span>         | [<span data-ttu-id="cc004-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="cc004-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="cc004-421">Sim</span><span class="sxs-lookup"><span data-stu-id="cc004-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="cc004-422">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc004-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="cc004-423">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc004-423">Response</span></span>

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
