---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 7bff2d2ae8e6a122621e3d17de7f7acc3f4e24df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991105"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="28b18-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-104">Create governanceRoleAssignmentRequest</span></span>

<span data-ttu-id="28b18-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28b18-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b18-106">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="28b18-106">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="28b18-107">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="28b18-107">The following table lists the operations.</span></span>

| <span data-ttu-id="28b18-108">Operação</span><span class="sxs-lookup"><span data-stu-id="28b18-108">Operation</span></span>                                   | <span data-ttu-id="28b18-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-109">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="28b18-110">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="28b18-110">Assign a role assignment</span></span>                    | <span data-ttu-id="28b18-111">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="28b18-111">AdminAdd</span></span>    |
| <span data-ttu-id="28b18-112">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="28b18-112">Activate an eligible role assignment</span></span>        | <span data-ttu-id="28b18-113">UserAdd</span><span class="sxs-lookup"><span data-stu-id="28b18-113">UserAdd</span></span>     |
| <span data-ttu-id="28b18-114">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="28b18-114">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="28b18-115">Userremove</span><span class="sxs-lookup"><span data-stu-id="28b18-115">UserRemove</span></span>  |
| <span data-ttu-id="28b18-116">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="28b18-116">Remove a role assignment</span></span>                    | <span data-ttu-id="28b18-117">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="28b18-117">AdminRemove</span></span> |
| <span data-ttu-id="28b18-118">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="28b18-118">Update a role assignment</span></span>                    | <span data-ttu-id="28b18-119">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="28b18-119">AdminUpdate</span></span> |
| <span data-ttu-id="28b18-120">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="28b18-120">Request to extend my role assignment</span></span>        | <span data-ttu-id="28b18-121">Userextend</span><span class="sxs-lookup"><span data-stu-id="28b18-121">UserExtend</span></span>  |
| <span data-ttu-id="28b18-122">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="28b18-122">Extend a role assignment</span></span>                    | <span data-ttu-id="28b18-123">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="28b18-123">AdminExtend</span></span> |
| <span data-ttu-id="28b18-124">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="28b18-124">Request to renew my expired role assignment</span></span> | <span data-ttu-id="28b18-125">Userrenew</span><span class="sxs-lookup"><span data-stu-id="28b18-125">UserRenew</span></span>   |
| <span data-ttu-id="28b18-126">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="28b18-126">Renew an expired role assignment</span></span>            | <span data-ttu-id="28b18-127">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="28b18-127">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="28b18-128">Permissões</span><span class="sxs-lookup"><span data-stu-id="28b18-128">Permissions</span></span>

<span data-ttu-id="28b18-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28b18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28b18-131">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28b18-131">Permission type</span></span>                        | <span data-ttu-id="28b18-132">Permissões</span><span class="sxs-lookup"><span data-stu-id="28b18-132">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="28b18-133">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28b18-133">Delegated (work or school account)</span></span>     | <span data-ttu-id="28b18-134">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="28b18-134">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="28b18-135">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28b18-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28b18-136">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28b18-136">Not supported.</span></span>                            |
| <span data-ttu-id="28b18-137">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28b18-137">Application</span></span>                            | <span data-ttu-id="28b18-138">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28b18-138">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28b18-139">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28b18-139">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="28b18-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28b18-140">Request headers</span></span>

| <span data-ttu-id="28b18-141">Nome</span><span class="sxs-lookup"><span data-stu-id="28b18-141">Name</span></span>          | <span data-ttu-id="28b18-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b18-142">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="28b18-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="28b18-143">Authorization</span></span> | <span data-ttu-id="28b18-144">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="28b18-144">Bearer {code}</span></span>    |
| <span data-ttu-id="28b18-145">Content-type</span><span class="sxs-lookup"><span data-stu-id="28b18-145">Content-type</span></span>  | <span data-ttu-id="28b18-146">application/json</span><span class="sxs-lookup"><span data-stu-id="28b18-146">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="28b18-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28b18-147">Request body</span></span>

<span data-ttu-id="28b18-148">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="28b18-148">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="28b18-149">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b18-149">Property</span></span>         | <span data-ttu-id="28b18-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-150">Type</span></span>                                                     | <span data-ttu-id="28b18-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="28b18-151">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="28b18-152">resourceId</span><span class="sxs-lookup"><span data-stu-id="28b18-152">resourceId</span></span>       | <span data-ttu-id="28b18-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b18-153">String</span></span>                                                   | <span data-ttu-id="28b18-154">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="28b18-154">The ID of the resource.</span></span> <span data-ttu-id="28b18-155">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b18-155">Required.</span></span> |
| <span data-ttu-id="28b18-156">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="28b18-156">roleDefinitionId</span></span> | <span data-ttu-id="28b18-157">String</span><span class="sxs-lookup"><span data-stu-id="28b18-157">String</span></span>                                                   | <span data-ttu-id="28b18-158">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="28b18-158">The ID of the role definition.</span></span> <span data-ttu-id="28b18-159">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b18-159">Required.</span></span> |
| <span data-ttu-id="28b18-160">SubjectID</span><span class="sxs-lookup"><span data-stu-id="28b18-160">subjectId</span></span>        | <span data-ttu-id="28b18-161">String</span><span class="sxs-lookup"><span data-stu-id="28b18-161">String</span></span>                                                   | <span data-ttu-id="28b18-162">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="28b18-162">The ID of the subject.</span></span> <span data-ttu-id="28b18-163">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b18-163">Required.</span></span> |
| <span data-ttu-id="28b18-164">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="28b18-164">assignmentState</span></span>  | <span data-ttu-id="28b18-165">String</span><span class="sxs-lookup"><span data-stu-id="28b18-165">String</span></span>                                                   | <span data-ttu-id="28b18-166">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="28b18-166">The state of assignment.</span></span> <span data-ttu-id="28b18-167">O valor pode ser `Eligible` e `Active` .</span><span class="sxs-lookup"><span data-stu-id="28b18-167">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="28b18-168">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b18-168">Required.</span></span> |
| <span data-ttu-id="28b18-169">tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-169">type</span></span>             | <span data-ttu-id="28b18-170">String</span><span class="sxs-lookup"><span data-stu-id="28b18-170">String</span></span>                                                   | <span data-ttu-id="28b18-171">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28b18-171">The request type.</span></span> <span data-ttu-id="28b18-172">O valor pode ser,,,,,, `AdminAdd` `UserAdd` `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew` `AdminRenew` e `AdminExtend` .</span><span class="sxs-lookup"><span data-stu-id="28b18-172">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="28b18-173">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28b18-173">Required.</span></span> |
| <span data-ttu-id="28b18-174">motivo</span><span class="sxs-lookup"><span data-stu-id="28b18-174">reason</span></span>           | <span data-ttu-id="28b18-175">String</span><span class="sxs-lookup"><span data-stu-id="28b18-175">String</span></span>                                                   | <span data-ttu-id="28b18-176">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="28b18-176">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="28b18-177">Cronograma</span><span class="sxs-lookup"><span data-stu-id="28b18-177">schedule</span></span>         | [<span data-ttu-id="28b18-178">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28b18-178">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="28b18-179">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="28b18-179">The schedule of the role assignment request.</span></span> <span data-ttu-id="28b18-180">Para o tipo de solicitação de,,, `UserAdd` `AdminAdd` `AdminUpdate` e `AdminExtend` , é necessário.</span><span class="sxs-lookup"><span data-stu-id="28b18-180">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="28b18-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b18-181">Response</span></span>

<span data-ttu-id="28b18-182">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28b18-182">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="28b18-183">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="28b18-183">Error codes</span></span>

<span data-ttu-id="28b18-184">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="28b18-184">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="28b18-185">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="28b18-185">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="28b18-186">Código de erro</span><span class="sxs-lookup"><span data-stu-id="28b18-186">Error code</span></span>     | <span data-ttu-id="28b18-187">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="28b18-187">Error message</span></span>                               | <span data-ttu-id="28b18-188">Detalhes</span><span class="sxs-lookup"><span data-stu-id="28b18-188">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="28b18-189">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-189">400 BadRequest</span></span> | <span data-ttu-id="28b18-190">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="28b18-190">RoleNotFound</span></span>                                | <span data-ttu-id="28b18-191">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="28b18-191">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="28b18-192">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-192">400 BadRequest</span></span> | <span data-ttu-id="28b18-193">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="28b18-193">ResourceIsLocked</span></span>                            | <span data-ttu-id="28b18-194">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="28b18-194">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="28b18-195">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-195">400 BadRequest</span></span> | <span data-ttu-id="28b18-196">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="28b18-196">SubjectNotFound</span></span>                             | <span data-ttu-id="28b18-197">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="28b18-197">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="28b18-198">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-198">400 BadRequest</span></span> | <span data-ttu-id="28b18-199">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-199">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="28b18-200">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="28b18-200">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="28b18-201">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-201">400 BadRequest</span></span> | <span data-ttu-id="28b18-202">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="28b18-202">RoleAssignmentExists</span></span>                        | <span data-ttu-id="28b18-203">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="28b18-203">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="28b18-204">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-204">400 BadRequest</span></span> | <span data-ttu-id="28b18-205">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="28b18-205">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="28b18-206">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="28b18-206">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="28b18-207">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="28b18-207">400 BadRequest</span></span> | <span data-ttu-id="28b18-208">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="28b18-208">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="28b18-209">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="28b18-209">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="28b18-210">Exemplos</span><span class="sxs-lookup"><span data-stu-id="28b18-210">Examples</span></span>

<span data-ttu-id="28b18-211">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="28b18-211">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="28b18-212">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="28b18-212">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="28b18-213">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="28b18-213">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="28b18-214">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="28b18-214">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="28b18-215">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b18-215">Property</span></span>         | <span data-ttu-id="28b18-216">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-216">Type</span></span>                                                     | <span data-ttu-id="28b18-217">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="28b18-217">Required</span></span>                 | <span data-ttu-id="28b18-218">Valor</span><span class="sxs-lookup"><span data-stu-id="28b18-218">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="28b18-219">resourceId</span><span class="sxs-lookup"><span data-stu-id="28b18-219">resourceId</span></span>       | <span data-ttu-id="28b18-220">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b18-220">String</span></span>                                                   | <span data-ttu-id="28b18-221">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-221">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="28b18-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="28b18-222">roleDefinitionId</span></span> | <span data-ttu-id="28b18-223">String</span><span class="sxs-lookup"><span data-stu-id="28b18-223">String</span></span>                                                   | <span data-ttu-id="28b18-224">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-224">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="28b18-225">SubjectID</span><span class="sxs-lookup"><span data-stu-id="28b18-225">subjectId</span></span>        | <span data-ttu-id="28b18-226">String</span><span class="sxs-lookup"><span data-stu-id="28b18-226">String</span></span>                                                   | <span data-ttu-id="28b18-227">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-227">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="28b18-228">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="28b18-228">assignmentState</span></span>  | <span data-ttu-id="28b18-229">String</span><span class="sxs-lookup"><span data-stu-id="28b18-229">String</span></span>                                                   | <span data-ttu-id="28b18-230">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-230">Yes</span></span>                      | <span data-ttu-id="28b18-231">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="28b18-231">Eligible / Active</span></span> |
| <span data-ttu-id="28b18-232">tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-232">type</span></span>             | <span data-ttu-id="28b18-233">String</span><span class="sxs-lookup"><span data-stu-id="28b18-233">String</span></span>                                                   | <span data-ttu-id="28b18-234">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-234">Yes</span></span>                      | <span data-ttu-id="28b18-235">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="28b18-235">AdminAdd</span></span> |
| <span data-ttu-id="28b18-236">motivo</span><span class="sxs-lookup"><span data-stu-id="28b18-236">reason</span></span>           | <span data-ttu-id="28b18-237">String</span><span class="sxs-lookup"><span data-stu-id="28b18-237">String</span></span>                                                   | <span data-ttu-id="28b18-238">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="28b18-238">depends on role Settings</span></span> |   |
| <span data-ttu-id="28b18-239">Cronograma</span><span class="sxs-lookup"><span data-stu-id="28b18-239">schedule</span></span>         | [<span data-ttu-id="28b18-240">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28b18-240">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="28b18-241">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-241">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="28b18-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b18-242">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="28b18-243">HTTP</span><span class="sxs-lookup"><span data-stu-id="28b18-243">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="28b18-244">C#</span><span class="sxs-lookup"><span data-stu-id="28b18-244">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28b18-245">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28b18-245">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28b18-246">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28b18-246">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="28b18-247">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b18-247">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="28b18-248">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="28b18-248">Example 2: User activates eligible role</span></span>

<span data-ttu-id="28b18-249">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="28b18-249">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="28b18-250">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b18-250">Property</span></span>         | <span data-ttu-id="28b18-251">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-251">Type</span></span>                                                     | <span data-ttu-id="28b18-252">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="28b18-252">Required</span></span>                 | <span data-ttu-id="28b18-253">Valor</span><span class="sxs-lookup"><span data-stu-id="28b18-253">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="28b18-254">resourceId</span><span class="sxs-lookup"><span data-stu-id="28b18-254">resourceId</span></span>       | <span data-ttu-id="28b18-255">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b18-255">String</span></span>                                                   | <span data-ttu-id="28b18-256">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-256">Yes</span></span>                      | \<resourceId\> |
| <span data-ttu-id="28b18-257">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="28b18-257">roleDefinitionId</span></span> | <span data-ttu-id="28b18-258">String</span><span class="sxs-lookup"><span data-stu-id="28b18-258">String</span></span>                                                   | <span data-ttu-id="28b18-259">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-259">Yes</span></span>                      | \<roleDefinitionId\> |
| <span data-ttu-id="28b18-260">SubjectID</span><span class="sxs-lookup"><span data-stu-id="28b18-260">subjectId</span></span>        | <span data-ttu-id="28b18-261">String</span><span class="sxs-lookup"><span data-stu-id="28b18-261">String</span></span>                                                   | <span data-ttu-id="28b18-262">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-262">Yes</span></span>                      | \<subjectId\> |
| <span data-ttu-id="28b18-263">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="28b18-263">assignmentState</span></span>  | <span data-ttu-id="28b18-264">String</span><span class="sxs-lookup"><span data-stu-id="28b18-264">String</span></span>                                                   | <span data-ttu-id="28b18-265">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-265">Yes</span></span>                      | <span data-ttu-id="28b18-266">Ativo</span><span class="sxs-lookup"><span data-stu-id="28b18-266">Active</span></span> |
| <span data-ttu-id="28b18-267">tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-267">type</span></span>             | <span data-ttu-id="28b18-268">String</span><span class="sxs-lookup"><span data-stu-id="28b18-268">String</span></span>                                                   | <span data-ttu-id="28b18-269">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-269">Yes</span></span>                      | <span data-ttu-id="28b18-270">UserAdd</span><span class="sxs-lookup"><span data-stu-id="28b18-270">UserAdd</span></span> |
| <span data-ttu-id="28b18-271">motivo</span><span class="sxs-lookup"><span data-stu-id="28b18-271">reason</span></span>           | <span data-ttu-id="28b18-272">String</span><span class="sxs-lookup"><span data-stu-id="28b18-272">String</span></span>                                                   | <span data-ttu-id="28b18-273">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="28b18-273">depends on role Settings</span></span> |   |
| <span data-ttu-id="28b18-274">Cronograma</span><span class="sxs-lookup"><span data-stu-id="28b18-274">schedule</span></span>         | [<span data-ttu-id="28b18-275">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28b18-275">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="28b18-276">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-276">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="28b18-277">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b18-277">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="28b18-278">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b18-278">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="28b18-279">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="28b18-279">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="28b18-280">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="28b18-280">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="28b18-281">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b18-281">Property</span></span>         | <span data-ttu-id="28b18-282">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-282">Type</span></span>                                                     | <span data-ttu-id="28b18-283">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="28b18-283">Required</span></span> | <span data-ttu-id="28b18-284">Valor</span><span class="sxs-lookup"><span data-stu-id="28b18-284">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="28b18-285">resourceId</span><span class="sxs-lookup"><span data-stu-id="28b18-285">resourceId</span></span>       | <span data-ttu-id="28b18-286">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b18-286">String</span></span>                                                   | <span data-ttu-id="28b18-287">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-287">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="28b18-288">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="28b18-288">roleDefinitionId</span></span> | <span data-ttu-id="28b18-289">String</span><span class="sxs-lookup"><span data-stu-id="28b18-289">String</span></span>                                                   | <span data-ttu-id="28b18-290">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-290">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="28b18-291">SubjectID</span><span class="sxs-lookup"><span data-stu-id="28b18-291">subjectId</span></span>        | <span data-ttu-id="28b18-292">String</span><span class="sxs-lookup"><span data-stu-id="28b18-292">String</span></span>                                                   | <span data-ttu-id="28b18-293">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-293">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="28b18-294">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="28b18-294">assignmentState</span></span>  | <span data-ttu-id="28b18-295">String</span><span class="sxs-lookup"><span data-stu-id="28b18-295">String</span></span>                                                   | <span data-ttu-id="28b18-296">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-296">Yes</span></span>      | <span data-ttu-id="28b18-297">Ativo</span><span class="sxs-lookup"><span data-stu-id="28b18-297">Active</span></span> |
| <span data-ttu-id="28b18-298">tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-298">type</span></span>             | <span data-ttu-id="28b18-299">String</span><span class="sxs-lookup"><span data-stu-id="28b18-299">String</span></span>                                                   | <span data-ttu-id="28b18-300">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-300">Yes</span></span>      | <span data-ttu-id="28b18-301">Userremove</span><span class="sxs-lookup"><span data-stu-id="28b18-301">UserRemove</span></span> |
| <span data-ttu-id="28b18-302">motivo</span><span class="sxs-lookup"><span data-stu-id="28b18-302">reason</span></span>           | <span data-ttu-id="28b18-303">String</span><span class="sxs-lookup"><span data-stu-id="28b18-303">String</span></span>                                                   | <span data-ttu-id="28b18-304">Não</span><span class="sxs-lookup"><span data-stu-id="28b18-304">No</span></span>       |   |
| <span data-ttu-id="28b18-305">Cronograma</span><span class="sxs-lookup"><span data-stu-id="28b18-305">schedule</span></span>         | [<span data-ttu-id="28b18-306">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28b18-306">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="28b18-307">Não</span><span class="sxs-lookup"><span data-stu-id="28b18-307">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="28b18-308">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b18-308">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="28b18-309">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b18-309">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="28b18-310">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="28b18-310">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="28b18-311">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="28b18-311">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="28b18-312">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="28b18-312">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="28b18-313">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b18-313">Property</span></span>         | <span data-ttu-id="28b18-314">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-314">Type</span></span>                                                     | <span data-ttu-id="28b18-315">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="28b18-315">Required</span></span> | <span data-ttu-id="28b18-316">Valor</span><span class="sxs-lookup"><span data-stu-id="28b18-316">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="28b18-317">resourceId</span><span class="sxs-lookup"><span data-stu-id="28b18-317">resourceId</span></span>       | <span data-ttu-id="28b18-318">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b18-318">String</span></span>                                                   | <span data-ttu-id="28b18-319">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-319">Yes</span></span>      | \<resourceId\> |
| <span data-ttu-id="28b18-320">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="28b18-320">roleDefinitionId</span></span> | <span data-ttu-id="28b18-321">String</span><span class="sxs-lookup"><span data-stu-id="28b18-321">String</span></span>                                                   | <span data-ttu-id="28b18-322">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-322">Yes</span></span>      | \<roleDefinitionId\> |
| <span data-ttu-id="28b18-323">SubjectID</span><span class="sxs-lookup"><span data-stu-id="28b18-323">subjectId</span></span>        | <span data-ttu-id="28b18-324">String</span><span class="sxs-lookup"><span data-stu-id="28b18-324">String</span></span>                                                   | <span data-ttu-id="28b18-325">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-325">Yes</span></span>      | \<subjectId\> |
| <span data-ttu-id="28b18-326">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="28b18-326">assignmentState</span></span>  | <span data-ttu-id="28b18-327">String</span><span class="sxs-lookup"><span data-stu-id="28b18-327">String</span></span>                                                   | <span data-ttu-id="28b18-328">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-328">Yes</span></span>      | <span data-ttu-id="28b18-329">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="28b18-329">Eligible / Active</span></span> |
| <span data-ttu-id="28b18-330">tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-330">type</span></span>             | <span data-ttu-id="28b18-331">String</span><span class="sxs-lookup"><span data-stu-id="28b18-331">String</span></span>                                                   | <span data-ttu-id="28b18-332">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-332">Yes</span></span>      | <span data-ttu-id="28b18-333">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="28b18-333">AdminRemove</span></span> |
| <span data-ttu-id="28b18-334">motivo</span><span class="sxs-lookup"><span data-stu-id="28b18-334">reason</span></span>           | <span data-ttu-id="28b18-335">String</span><span class="sxs-lookup"><span data-stu-id="28b18-335">String</span></span>                                                   | <span data-ttu-id="28b18-336">Não</span><span class="sxs-lookup"><span data-stu-id="28b18-336">No</span></span>       |   |
| <span data-ttu-id="28b18-337">Cronograma</span><span class="sxs-lookup"><span data-stu-id="28b18-337">schedule</span></span>         | [<span data-ttu-id="28b18-338">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28b18-338">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="28b18-339">Não</span><span class="sxs-lookup"><span data-stu-id="28b18-339">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="28b18-340">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b18-340">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="28b18-341">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b18-341">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="28b18-342">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="28b18-342">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="28b18-343">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="28b18-343">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="28b18-344">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="28b18-344">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="28b18-345">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b18-345">Property</span></span>         | <span data-ttu-id="28b18-346">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-346">Type</span></span>                                                     | <span data-ttu-id="28b18-347">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="28b18-347">Required</span></span>                | <span data-ttu-id="28b18-348">Valor</span><span class="sxs-lookup"><span data-stu-id="28b18-348">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="28b18-349">resourceId</span><span class="sxs-lookup"><span data-stu-id="28b18-349">resourceId</span></span>       | <span data-ttu-id="28b18-350">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b18-350">String</span></span>                                                   | <span data-ttu-id="28b18-351">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-351">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="28b18-352">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="28b18-352">roleDefinitionId</span></span> | <span data-ttu-id="28b18-353">String</span><span class="sxs-lookup"><span data-stu-id="28b18-353">String</span></span>                                                   | <span data-ttu-id="28b18-354">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-354">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="28b18-355">SubjectID</span><span class="sxs-lookup"><span data-stu-id="28b18-355">subjectId</span></span>        | <span data-ttu-id="28b18-356">String</span><span class="sxs-lookup"><span data-stu-id="28b18-356">String</span></span>                                                   | <span data-ttu-id="28b18-357">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-357">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="28b18-358">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="28b18-358">assignmentState</span></span>  | <span data-ttu-id="28b18-359">String</span><span class="sxs-lookup"><span data-stu-id="28b18-359">String</span></span>                                                   | <span data-ttu-id="28b18-360">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-360">Yes</span></span>                     | <span data-ttu-id="28b18-361">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="28b18-361">Eligible / Active</span></span> |
| <span data-ttu-id="28b18-362">tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-362">type</span></span>             | <span data-ttu-id="28b18-363">String</span><span class="sxs-lookup"><span data-stu-id="28b18-363">String</span></span>                                                   | <span data-ttu-id="28b18-364">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-364">Yes</span></span>                     | <span data-ttu-id="28b18-365">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="28b18-365">AdminUpdate</span></span> |
| <span data-ttu-id="28b18-366">motivo</span><span class="sxs-lookup"><span data-stu-id="28b18-366">reason</span></span>           | <span data-ttu-id="28b18-367">String</span><span class="sxs-lookup"><span data-stu-id="28b18-367">String</span></span>                                                   | <span data-ttu-id="28b18-368">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="28b18-368">depends on roleSettings</span></span> |   |
| <span data-ttu-id="28b18-369">Cronograma</span><span class="sxs-lookup"><span data-stu-id="28b18-369">schedule</span></span>         | [<span data-ttu-id="28b18-370">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28b18-370">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="28b18-371">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-371">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="28b18-372">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b18-372">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="28b18-373">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b18-373">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="28b18-374">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="28b18-374">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="28b18-375">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="28b18-375">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="28b18-376">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma atribuição de `Active` função de administrador ( `owner` ou `user access administrator` ) no recurso.</span><span class="sxs-lookup"><span data-stu-id="28b18-376">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="28b18-377">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28b18-377">Property</span></span>         | <span data-ttu-id="28b18-378">Tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-378">Type</span></span>                                                     | <span data-ttu-id="28b18-379">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="28b18-379">Required</span></span>                | <span data-ttu-id="28b18-380">Valor</span><span class="sxs-lookup"><span data-stu-id="28b18-380">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="28b18-381">resourceId</span><span class="sxs-lookup"><span data-stu-id="28b18-381">resourceId</span></span>       | <span data-ttu-id="28b18-382">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28b18-382">String</span></span>                                                   | <span data-ttu-id="28b18-383">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-383">Yes</span></span>                     | \<resourceId\> |
| <span data-ttu-id="28b18-384">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="28b18-384">roleDefinitionId</span></span> | <span data-ttu-id="28b18-385">String</span><span class="sxs-lookup"><span data-stu-id="28b18-385">String</span></span>                                                   | <span data-ttu-id="28b18-386">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-386">Yes</span></span>                     | \<roleDefinitionId\> |
| <span data-ttu-id="28b18-387">SubjectID</span><span class="sxs-lookup"><span data-stu-id="28b18-387">subjectId</span></span>        | <span data-ttu-id="28b18-388">String</span><span class="sxs-lookup"><span data-stu-id="28b18-388">String</span></span>                                                   | <span data-ttu-id="28b18-389">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-389">Yes</span></span>                     | \<subjectId\> |
| <span data-ttu-id="28b18-390">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="28b18-390">assignmentState</span></span>  | <span data-ttu-id="28b18-391">String</span><span class="sxs-lookup"><span data-stu-id="28b18-391">String</span></span>                                                   | <span data-ttu-id="28b18-392">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-392">Yes</span></span>                     | <span data-ttu-id="28b18-393">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="28b18-393">Eligible / Active</span></span> |
| <span data-ttu-id="28b18-394">tipo</span><span class="sxs-lookup"><span data-stu-id="28b18-394">type</span></span>             | <span data-ttu-id="28b18-395">String</span><span class="sxs-lookup"><span data-stu-id="28b18-395">String</span></span>                                                   | <span data-ttu-id="28b18-396">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-396">Yes</span></span>                     | <span data-ttu-id="28b18-397">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="28b18-397">AdminExtend</span></span> |
| <span data-ttu-id="28b18-398">motivo</span><span class="sxs-lookup"><span data-stu-id="28b18-398">reason</span></span>           | <span data-ttu-id="28b18-399">String</span><span class="sxs-lookup"><span data-stu-id="28b18-399">String</span></span>                                                   | <span data-ttu-id="28b18-400">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="28b18-400">depends on roleSettings</span></span> |   |
| <span data-ttu-id="28b18-401">Cronograma</span><span class="sxs-lookup"><span data-stu-id="28b18-401">schedule</span></span>         | [<span data-ttu-id="28b18-402">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="28b18-402">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="28b18-403">Sim</span><span class="sxs-lookup"><span data-stu-id="28b18-403">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="28b18-404">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28b18-404">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="28b18-405">Resposta</span><span class="sxs-lookup"><span data-stu-id="28b18-405">Response</span></span>

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


