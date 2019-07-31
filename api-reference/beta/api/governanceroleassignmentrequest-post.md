---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 65ba674740fc7bc756d24fa3fc57b8db13d874b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954127"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="c4ec7-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-104">Create governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4ec7-105">Crie uma solicitação de atribuição de função para representar a operação desejada em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-105">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="c4ec7-106">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-106">The following table lists the operations.</span></span>

| <span data-ttu-id="c4ec7-107">Operation</span><span class="sxs-lookup"><span data-stu-id="c4ec7-107">Operation</span></span>                                   | <span data-ttu-id="c4ec7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-108">Type</span></span>        |
|:--------------------------------------------|:------------|
| <span data-ttu-id="c4ec7-109">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-109">Assign a role assignment</span></span>                    | <span data-ttu-id="c4ec7-110">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c4ec7-110">AdminAdd</span></span>    |
| <span data-ttu-id="c4ec7-111">Ativar uma atribuição de função qualificada</span><span class="sxs-lookup"><span data-stu-id="c4ec7-111">Activate an eligible role assignment</span></span>        | <span data-ttu-id="c4ec7-112">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c4ec7-112">UserAdd</span></span>     |
| <span data-ttu-id="c4ec7-113">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="c4ec7-113">Deactivate an activated role assignment</span></span>     | <span data-ttu-id="c4ec7-114">Userremove</span><span class="sxs-lookup"><span data-stu-id="c4ec7-114">UserRemove</span></span>  |
| <span data-ttu-id="c4ec7-115">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-115">Remove a role assignment</span></span>                    | <span data-ttu-id="c4ec7-116">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c4ec7-116">AdminRemove</span></span> |
| <span data-ttu-id="c4ec7-117">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-117">Update a role assignment</span></span>                    | <span data-ttu-id="c4ec7-118">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-118">AdminUpdate</span></span> |
| <span data-ttu-id="c4ec7-119">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-119">Request to extend my role assignment</span></span>        | <span data-ttu-id="c4ec7-120">Userextend</span><span class="sxs-lookup"><span data-stu-id="c4ec7-120">UserExtend</span></span>  |
| <span data-ttu-id="c4ec7-121">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-121">Extend a role assignment</span></span>                    | <span data-ttu-id="c4ec7-122">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c4ec7-122">AdminExtend</span></span> |
| <span data-ttu-id="c4ec7-123">Solicitação para renovar minha atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="c4ec7-123">Request to renew my expired role assignment</span></span> | <span data-ttu-id="c4ec7-124">Userrenew</span><span class="sxs-lookup"><span data-stu-id="c4ec7-124">UserRenew</span></span>   |
| <span data-ttu-id="c4ec7-125">Renovar uma atribuição de função expirada</span><span class="sxs-lookup"><span data-stu-id="c4ec7-125">Renew an expired role assignment</span></span>            | <span data-ttu-id="c4ec7-126">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="c4ec7-126">AdminRenew</span></span>  |

## <a name="permissions"></a><span data-ttu-id="c4ec7-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4ec7-127">Permissions</span></span>

<span data-ttu-id="c4ec7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4ec7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4ec7-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4ec7-130">Permission type</span></span>                        | <span data-ttu-id="c4ec7-131">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4ec7-131">Permissions</span></span>                               |
|:---------------------------------------|:------------------------------------------|
| <span data-ttu-id="c4ec7-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4ec7-132">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4ec7-133">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="c4ec7-133">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="c4ec7-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4ec7-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4ec7-135">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-135">Not supported.</span></span>                            |
| <span data-ttu-id="c4ec7-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-136">Application</span></span>                            | <span data-ttu-id="c4ec7-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-137">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4ec7-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ec7-138">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="c4ec7-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ec7-139">Request headers</span></span>

| <span data-ttu-id="c4ec7-140">Nome</span><span class="sxs-lookup"><span data-stu-id="c4ec7-140">Name</span></span>          | <span data-ttu-id="c4ec7-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4ec7-141">Description</span></span>      |
|:--------------|:-----------------|
| <span data-ttu-id="c4ec7-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4ec7-142">Authorization</span></span> | <span data-ttu-id="c4ec7-143">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c4ec7-143">Bearer {code}</span></span>    |
| <span data-ttu-id="c4ec7-144">Content-type</span><span class="sxs-lookup"><span data-stu-id="c4ec7-144">Content-type</span></span>  | <span data-ttu-id="c4ec7-145">application/json</span><span class="sxs-lookup"><span data-stu-id="c4ec7-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4ec7-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ec7-146">Request body</span></span>

<span data-ttu-id="c4ec7-147">No corpo da solicitação, forneça uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c4ec7-147">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span>

| <span data-ttu-id="c4ec7-148">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ec7-148">Property</span></span>         | <span data-ttu-id="c4ec7-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-149">Type</span></span>                                                     | <span data-ttu-id="c4ec7-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4ec7-150">Description</span></span> |
|:-----------------|:---------------------------------------------------------|:--|
| <span data-ttu-id="c4ec7-151">resourceId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-151">resourceId</span></span>       | <span data-ttu-id="c4ec7-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ec7-152">String</span></span>                                                   | <span data-ttu-id="c4ec7-153">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-153">The ID of the resource.</span></span> <span data-ttu-id="c4ec7-154">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-154">Required.</span></span> |
| <span data-ttu-id="c4ec7-155">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-155">roleDefinitionId</span></span> | <span data-ttu-id="c4ec7-156">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-156">String</span></span>                                                   | <span data-ttu-id="c4ec7-157">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-157">The ID of the role definition.</span></span> <span data-ttu-id="c4ec7-158">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-158">Required.</span></span> |
| <span data-ttu-id="c4ec7-159">SubjectID</span><span class="sxs-lookup"><span data-stu-id="c4ec7-159">subjectId</span></span>        | <span data-ttu-id="c4ec7-160">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-160">String</span></span>                                                   | <span data-ttu-id="c4ec7-161">A ID do assunto.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-161">The ID of the subject.</span></span> <span data-ttu-id="c4ec7-162">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-162">Required.</span></span> |
| <span data-ttu-id="c4ec7-163">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-163">assignmentState</span></span>  | <span data-ttu-id="c4ec7-164">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-164">String</span></span>                                                   | <span data-ttu-id="c4ec7-165">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-165">The state of assignment.</span></span> <span data-ttu-id="c4ec7-166">O valor pode ser `Eligible` e `Active`.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-166">The value can be `Eligible` and `Active`.</span></span> <span data-ttu-id="c4ec7-167">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-167">Required.</span></span> |
| <span data-ttu-id="c4ec7-168">type</span><span class="sxs-lookup"><span data-stu-id="c4ec7-168">type</span></span>             | <span data-ttu-id="c4ec7-169">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-169">String</span></span>                                                   | <span data-ttu-id="c4ec7-170">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-170">The request type.</span></span> <span data-ttu-id="c4ec7-171">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate` `AdminRemove` `UserRemove` `UserExtend` `UserRenew`,,,, `AdminRenew`e. `AdminExtend`</span><span class="sxs-lookup"><span data-stu-id="c4ec7-171">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span> <span data-ttu-id="c4ec7-172">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-172">Required.</span></span> |
| <span data-ttu-id="c4ec7-173">motivos</span><span class="sxs-lookup"><span data-stu-id="c4ec7-173">reason</span></span>           | <span data-ttu-id="c4ec7-174">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-174">String</span></span>                                                   | <span data-ttu-id="c4ec7-175">O motivo precisa ser fornecido para a solicitação de atribuição de função para fins de auditoria e análise.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-175">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span> |
| <span data-ttu-id="c4ec7-176">Cronograma</span><span class="sxs-lookup"><span data-stu-id="c4ec7-176">schedule</span></span>         | [<span data-ttu-id="c4ec7-177">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c4ec7-177">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c4ec7-178">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-178">The schedule of the role assignment request.</span></span> <span data-ttu-id="c4ec7-179">Para o tipo de `UserAdd`solicitação `AdminAdd`de `AdminUpdate`,, `AdminExtend`, e, é necessário.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-179">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span> |

## <a name="response"></a><span data-ttu-id="c4ec7-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ec7-180">Response</span></span>

<span data-ttu-id="c4ec7-181">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-181">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="c4ec7-182">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="c4ec7-182">Error codes</span></span>

<span data-ttu-id="c4ec7-183">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-183">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="c4ec7-184">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-184">In addition, it also returns the error codes listed in the following table.</span></span>

| <span data-ttu-id="c4ec7-185">Código de erro</span><span class="sxs-lookup"><span data-stu-id="c4ec7-185">Error code</span></span>     | <span data-ttu-id="c4ec7-186">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="c4ec7-186">Error message</span></span>                               | <span data-ttu-id="c4ec7-187">Detalhes</span><span class="sxs-lookup"><span data-stu-id="c4ec7-187">Details</span></span>       |
|:---------------|:--------------------------------------------|:--------------|
| <span data-ttu-id="c4ec7-188">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-188">400 BadRequest</span></span> | <span data-ttu-id="c4ec7-189">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="c4ec7-189">RoleNotFound</span></span>                                | <span data-ttu-id="c4ec7-190">O `roleDefinitionId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-190">The `roleDefinitionId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="c4ec7-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-191">400 BadRequest</span></span> | <span data-ttu-id="c4ec7-192">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="c4ec7-192">ResourceIsLocked</span></span>                            | <span data-ttu-id="c4ec7-193">O recurso fornecido no corpo da solicitação está no estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-193">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span> |
| <span data-ttu-id="c4ec7-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-194">400 BadRequest</span></span> | <span data-ttu-id="c4ec7-195">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="c4ec7-195">SubjectNotFound</span></span>                             | <span data-ttu-id="c4ec7-196">O `subjectId` corpo da solicitação fornecido não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-196">The `subjectId` provided in the request body cannot be found.</span></span> |
| <span data-ttu-id="c4ec7-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-197">400 BadRequest</span></span> | <span data-ttu-id="c4ec7-198">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-198">PendingRoleAssignmentRequest</span></span>                | <span data-ttu-id="c4ec7-199">Já existe um [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) pendente no sistema.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-199">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span> |
| <span data-ttu-id="c4ec7-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-200">400 BadRequest</span></span> | <span data-ttu-id="c4ec7-201">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="c4ec7-201">RoleAssignmentExists</span></span>                        | <span data-ttu-id="c4ec7-202">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criado já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-202">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span> |
| <span data-ttu-id="c4ec7-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-203">400 BadRequest</span></span> | <span data-ttu-id="c4ec7-204">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="c4ec7-204">RoleAssignmentDoesNotExist</span></span>                  | <span data-ttu-id="c4ec7-205">O [governanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span> |
| <span data-ttu-id="c4ec7-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c4ec7-206">400 BadRequest</span></span> | <span data-ttu-id="c4ec7-207">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="c4ec7-207">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="c4ec7-208">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-208">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span> |

## <a name="examples"></a><span data-ttu-id="c4ec7-209">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c4ec7-209">Examples</span></span>

<span data-ttu-id="c4ec7-210">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-210">The following examples show how to use this API.</span></span>

### <a name="example-1-administrator-assigns-user-to-a-role"></a><span data-ttu-id="c4ec7-211">Exemplo 1: o administrador atribui um usuário a uma função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-211">Example 1: Administrator assigns user to a role</span></span>

<span data-ttu-id="c4ec7-212">Neste exemplo, um administrador atribui o usuário nawu@fimdev.net à função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-212">In this example, an administrator assigns user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="c4ec7-213">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-213">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c4ec7-214">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ec7-214">Property</span></span>         | <span data-ttu-id="c4ec7-215">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-215">Type</span></span>                                                     | <span data-ttu-id="c4ec7-216">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c4ec7-216">Required</span></span>                 | <span data-ttu-id="c4ec7-217">Valor</span><span class="sxs-lookup"><span data-stu-id="c4ec7-217">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="c4ec7-218">resourceId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-218">resourceId</span></span>       | <span data-ttu-id="c4ec7-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ec7-219">String</span></span>                                                   | <span data-ttu-id="c4ec7-220">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-220">Yes</span></span>                      | <span data-ttu-id="c4ec7-221">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-221">\<resourceId\></span></span> |
| <span data-ttu-id="c4ec7-222">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-222">roleDefinitionId</span></span> | <span data-ttu-id="c4ec7-223">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-223">String</span></span>                                                   | <span data-ttu-id="c4ec7-224">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-224">Yes</span></span>                      | <span data-ttu-id="c4ec7-225">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-225">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c4ec7-226">SubjectID</span><span class="sxs-lookup"><span data-stu-id="c4ec7-226">subjectId</span></span>        | <span data-ttu-id="c4ec7-227">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-227">String</span></span>                                                   | <span data-ttu-id="c4ec7-228">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-228">Yes</span></span>                      | <span data-ttu-id="c4ec7-229">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-229">\<subjectId\></span></span> |
| <span data-ttu-id="c4ec7-230">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-230">assignmentState</span></span>  | <span data-ttu-id="c4ec7-231">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-231">String</span></span>                                                   | <span data-ttu-id="c4ec7-232">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-232">Yes</span></span>                      | <span data-ttu-id="c4ec7-233">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-233">Eligible / Active</span></span> |
| <span data-ttu-id="c4ec7-234">type</span><span class="sxs-lookup"><span data-stu-id="c4ec7-234">type</span></span>             | <span data-ttu-id="c4ec7-235">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-235">String</span></span>                                                   | <span data-ttu-id="c4ec7-236">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-236">Yes</span></span>                      | <span data-ttu-id="c4ec7-237">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="c4ec7-237">AdminAdd</span></span> |
| <span data-ttu-id="c4ec7-238">motivos</span><span class="sxs-lookup"><span data-stu-id="c4ec7-238">reason</span></span>           | <span data-ttu-id="c4ec7-239">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-239">String</span></span>                                                   | <span data-ttu-id="c4ec7-240">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-240">depends on role Settings</span></span> |   |
| <span data-ttu-id="c4ec7-241">Cronograma</span><span class="sxs-lookup"><span data-stu-id="c4ec7-241">schedule</span></span>         | [<span data-ttu-id="c4ec7-242">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c4ec7-242">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c4ec7-243">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-243">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="c4ec7-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ec7-244">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4ec7-245">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4ec7-245">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4ec7-246">C#</span><span class="sxs-lookup"><span data-stu-id="c4ec7-246">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/governanceroleassignmentrequest-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4ec7-247">Javascript</span><span class="sxs-lookup"><span data-stu-id="c4ec7-247">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/governanceroleassignmentrequest-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4ec7-248">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c4ec7-248">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/governanceroleassignmentrequest-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c4ec7-249">Java</span><span class="sxs-lookup"><span data-stu-id="c4ec7-249">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/governanceroleassignmentrequest-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c4ec7-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ec7-250">Response</span></span>

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

### <a name="example-2-user-activates-eligible-role"></a><span data-ttu-id="c4ec7-251">Exemplo 2: o usuário ativa a função qualificada</span><span class="sxs-lookup"><span data-stu-id="c4ec7-251">Example 2: User activates eligible role</span></span>

<span data-ttu-id="c4ec7-252">Neste exemplo, o usuário nawu@fimdev.net ativa a função de leitor de cobrança qualificado.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-252">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="c4ec7-253">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ec7-253">Property</span></span>         | <span data-ttu-id="c4ec7-254">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-254">Type</span></span>                                                     | <span data-ttu-id="c4ec7-255">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c4ec7-255">Required</span></span>                 | <span data-ttu-id="c4ec7-256">Valor</span><span class="sxs-lookup"><span data-stu-id="c4ec7-256">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| <span data-ttu-id="c4ec7-257">resourceId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-257">resourceId</span></span>       | <span data-ttu-id="c4ec7-258">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ec7-258">String</span></span>                                                   | <span data-ttu-id="c4ec7-259">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-259">Yes</span></span>                      | <span data-ttu-id="c4ec7-260">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-260">\<resourceId\></span></span> |
| <span data-ttu-id="c4ec7-261">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-261">roleDefinitionId</span></span> | <span data-ttu-id="c4ec7-262">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-262">String</span></span>                                                   | <span data-ttu-id="c4ec7-263">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-263">Yes</span></span>                      | <span data-ttu-id="c4ec7-264">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-264">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c4ec7-265">SubjectID</span><span class="sxs-lookup"><span data-stu-id="c4ec7-265">subjectId</span></span>        | <span data-ttu-id="c4ec7-266">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-266">String</span></span>                                                   | <span data-ttu-id="c4ec7-267">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-267">Yes</span></span>                      | <span data-ttu-id="c4ec7-268">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-268">\<subjectId\></span></span> |
| <span data-ttu-id="c4ec7-269">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-269">assignmentState</span></span>  | <span data-ttu-id="c4ec7-270">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-270">String</span></span>                                                   | <span data-ttu-id="c4ec7-271">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-271">Yes</span></span>                      | <span data-ttu-id="c4ec7-272">Ativo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-272">Active</span></span> |
| <span data-ttu-id="c4ec7-273">type</span><span class="sxs-lookup"><span data-stu-id="c4ec7-273">type</span></span>             | <span data-ttu-id="c4ec7-274">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-274">String</span></span>                                                   | <span data-ttu-id="c4ec7-275">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-275">Yes</span></span>                      | <span data-ttu-id="c4ec7-276">UserAdd</span><span class="sxs-lookup"><span data-stu-id="c4ec7-276">UserAdd</span></span> |
| <span data-ttu-id="c4ec7-277">motivos</span><span class="sxs-lookup"><span data-stu-id="c4ec7-277">reason</span></span>           | <span data-ttu-id="c4ec7-278">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-278">String</span></span>                                                   | <span data-ttu-id="c4ec7-279">depende das configurações de função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-279">depends on role Settings</span></span> |   |
| <span data-ttu-id="c4ec7-280">Cronograma</span><span class="sxs-lookup"><span data-stu-id="c4ec7-280">schedule</span></span>         | [<span data-ttu-id="c4ec7-281">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c4ec7-281">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c4ec7-282">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-282">Yes</span></span>                      |   |

#### <a name="request"></a><span data-ttu-id="c4ec7-283">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ec7-283">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c4ec7-284">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ec7-284">Response</span></span>

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

### <a name="example-3-user-deactivates-an-assigned-role"></a><span data-ttu-id="c4ec7-285">Exemplo 3: o usuário desativa uma função atribuída</span><span class="sxs-lookup"><span data-stu-id="c4ec7-285">Example 3: User deactivates an assigned role</span></span>

<span data-ttu-id="c4ec7-286">Neste exemplo, o usuário nawu@fimdev.net desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-286">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="c4ec7-287">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ec7-287">Property</span></span>         | <span data-ttu-id="c4ec7-288">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-288">Type</span></span>                                                     | <span data-ttu-id="c4ec7-289">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c4ec7-289">Required</span></span> | <span data-ttu-id="c4ec7-290">Valor</span><span class="sxs-lookup"><span data-stu-id="c4ec7-290">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="c4ec7-291">resourceId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-291">resourceId</span></span>       | <span data-ttu-id="c4ec7-292">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c4ec7-292">String</span></span>                                                   | <span data-ttu-id="c4ec7-293">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-293">Yes</span></span>      | <span data-ttu-id="c4ec7-294">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-294">\<resourceId\></span></span> |
| <span data-ttu-id="c4ec7-295">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-295">roleDefinitionId</span></span> | <span data-ttu-id="c4ec7-296">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-296">String</span></span>                                                   | <span data-ttu-id="c4ec7-297">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-297">Yes</span></span>      | <span data-ttu-id="c4ec7-298">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-298">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c4ec7-299">SubjectID</span><span class="sxs-lookup"><span data-stu-id="c4ec7-299">subjectId</span></span>        | <span data-ttu-id="c4ec7-300">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-300">String</span></span>                                                   | <span data-ttu-id="c4ec7-301">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-301">Yes</span></span>      | <span data-ttu-id="c4ec7-302">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-302">\<subjectId\></span></span> |
| <span data-ttu-id="c4ec7-303">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-303">assignmentState</span></span>  | <span data-ttu-id="c4ec7-304">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-304">String</span></span>                                                   | <span data-ttu-id="c4ec7-305">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-305">Yes</span></span>      | <span data-ttu-id="c4ec7-306">Ativo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-306">Active</span></span> |
| <span data-ttu-id="c4ec7-307">type</span><span class="sxs-lookup"><span data-stu-id="c4ec7-307">type</span></span>             | <span data-ttu-id="c4ec7-308">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-308">String</span></span>                                                   | <span data-ttu-id="c4ec7-309">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-309">Yes</span></span>      | <span data-ttu-id="c4ec7-310">Userremove</span><span class="sxs-lookup"><span data-stu-id="c4ec7-310">UserRemove</span></span> |
| <span data-ttu-id="c4ec7-311">motivos</span><span class="sxs-lookup"><span data-stu-id="c4ec7-311">reason</span></span>           | <span data-ttu-id="c4ec7-312">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-312">String</span></span>                                                   | <span data-ttu-id="c4ec7-313">Não</span><span class="sxs-lookup"><span data-stu-id="c4ec7-313">No</span></span>       |   |
| <span data-ttu-id="c4ec7-314">Cronograma</span><span class="sxs-lookup"><span data-stu-id="c4ec7-314">schedule</span></span>         | [<span data-ttu-id="c4ec7-315">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c4ec7-315">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c4ec7-316">Não</span><span class="sxs-lookup"><span data-stu-id="c4ec7-316">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="c4ec7-317">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ec7-317">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c4ec7-318">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ec7-318">Response</span></span>

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

### <a name="example-4-administrator-removes-user-from-a-role"></a><span data-ttu-id="c4ec7-319">Exemplo 4: o administrador remove o usuário de uma função</span><span class="sxs-lookup"><span data-stu-id="c4ec7-319">Example 4: Administrator removes user from a role</span></span>

<span data-ttu-id="c4ec7-320">Neste exemplo, um administrador remove o usuário nawu@fimdev.net da função leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-320">In this example, an administrator removes the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="c4ec7-321">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-321">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c4ec7-322">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ec7-322">Property</span></span>         | <span data-ttu-id="c4ec7-323">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-323">Type</span></span>                                                     | <span data-ttu-id="c4ec7-324">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c4ec7-324">Required</span></span> | <span data-ttu-id="c4ec7-325">Valor</span><span class="sxs-lookup"><span data-stu-id="c4ec7-325">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| <span data-ttu-id="c4ec7-326">resourceId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-326">resourceId</span></span>       | <span data-ttu-id="c4ec7-327">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-327">String</span></span>                                                   | <span data-ttu-id="c4ec7-328">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-328">Yes</span></span>      | <span data-ttu-id="c4ec7-329">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-329">\<resourceId\></span></span> |
| <span data-ttu-id="c4ec7-330">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-330">roleDefinitionId</span></span> | <span data-ttu-id="c4ec7-331">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-331">String</span></span>                                                   | <span data-ttu-id="c4ec7-332">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-332">Yes</span></span>      | <span data-ttu-id="c4ec7-333">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-333">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c4ec7-334">SubjectID</span><span class="sxs-lookup"><span data-stu-id="c4ec7-334">subjectId</span></span>        | <span data-ttu-id="c4ec7-335">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-335">String</span></span>                                                   | <span data-ttu-id="c4ec7-336">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-336">Yes</span></span>      | <span data-ttu-id="c4ec7-337">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-337">\<subjectId\></span></span> |
| <span data-ttu-id="c4ec7-338">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-338">assignmentState</span></span>  | <span data-ttu-id="c4ec7-339">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-339">String</span></span>                                                   | <span data-ttu-id="c4ec7-340">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-340">Yes</span></span>      | <span data-ttu-id="c4ec7-341">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-341">Eligible / Active</span></span> |
| <span data-ttu-id="c4ec7-342">type</span><span class="sxs-lookup"><span data-stu-id="c4ec7-342">type</span></span>             | <span data-ttu-id="c4ec7-343">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-343">String</span></span>                                                   | <span data-ttu-id="c4ec7-344">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-344">Yes</span></span>      | <span data-ttu-id="c4ec7-345">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="c4ec7-345">AdminRemove</span></span> |
| <span data-ttu-id="c4ec7-346">motivos</span><span class="sxs-lookup"><span data-stu-id="c4ec7-346">reason</span></span>           | <span data-ttu-id="c4ec7-347">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-347">String</span></span>                                                   | <span data-ttu-id="c4ec7-348">Não</span><span class="sxs-lookup"><span data-stu-id="c4ec7-348">No</span></span>       |   |
| <span data-ttu-id="c4ec7-349">Cronograma</span><span class="sxs-lookup"><span data-stu-id="c4ec7-349">schedule</span></span>         | [<span data-ttu-id="c4ec7-350">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c4ec7-350">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c4ec7-351">Não</span><span class="sxs-lookup"><span data-stu-id="c4ec7-351">No</span></span>       |   |

#### <a name="request"></a><span data-ttu-id="c4ec7-352">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ec7-352">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c4ec7-353">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ec7-353">Response</span></span>

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

### <a name="example-5-administrator-updates-role-assignment"></a><span data-ttu-id="c4ec7-354">Exemplo 5: atribuição de função de atualização do administrador</span><span class="sxs-lookup"><span data-stu-id="c4ec7-354">Example 5: Administrator updates role assignment</span></span>

<span data-ttu-id="c4ec7-355">Neste exemplo, os administradores atualizam a atribuição de função para o usuário nawu@fimdev.net para o proprietário.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-355">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="c4ec7-356">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-356">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c4ec7-357">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ec7-357">Property</span></span>         | <span data-ttu-id="c4ec7-358">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-358">Type</span></span>                                                     | <span data-ttu-id="c4ec7-359">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c4ec7-359">Required</span></span>                | <span data-ttu-id="c4ec7-360">Valor</span><span class="sxs-lookup"><span data-stu-id="c4ec7-360">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="c4ec7-361">resourceId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-361">resourceId</span></span>       | <span data-ttu-id="c4ec7-362">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-362">String</span></span>                                                   | <span data-ttu-id="c4ec7-363">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-363">Yes</span></span>                     | <span data-ttu-id="c4ec7-364">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-364">\<resourceId\></span></span> |
| <span data-ttu-id="c4ec7-365">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-365">roleDefinitionId</span></span> | <span data-ttu-id="c4ec7-366">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-366">String</span></span>                                                   | <span data-ttu-id="c4ec7-367">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-367">Yes</span></span>                     | <span data-ttu-id="c4ec7-368">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-368">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c4ec7-369">SubjectID</span><span class="sxs-lookup"><span data-stu-id="c4ec7-369">subjectId</span></span>        | <span data-ttu-id="c4ec7-370">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-370">String</span></span>                                                   | <span data-ttu-id="c4ec7-371">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-371">Yes</span></span>                     | <span data-ttu-id="c4ec7-372">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-372">\<subjectId\></span></span> |
| <span data-ttu-id="c4ec7-373">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-373">assignmentState</span></span>  | <span data-ttu-id="c4ec7-374">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-374">String</span></span>                                                   | <span data-ttu-id="c4ec7-375">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-375">Yes</span></span>                     | <span data-ttu-id="c4ec7-376">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-376">Eligible / Active</span></span> |
| <span data-ttu-id="c4ec7-377">type</span><span class="sxs-lookup"><span data-stu-id="c4ec7-377">type</span></span>             | <span data-ttu-id="c4ec7-378">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-378">String</span></span>                                                   | <span data-ttu-id="c4ec7-379">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-379">Yes</span></span>                     | <span data-ttu-id="c4ec7-380">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-380">AdminUpdate</span></span> |
| <span data-ttu-id="c4ec7-381">motivos</span><span class="sxs-lookup"><span data-stu-id="c4ec7-381">reason</span></span>           | <span data-ttu-id="c4ec7-382">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-382">String</span></span>                                                   | <span data-ttu-id="c4ec7-383">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="c4ec7-383">depends on roleSettings</span></span> |   |
| <span data-ttu-id="c4ec7-384">Cronograma</span><span class="sxs-lookup"><span data-stu-id="c4ec7-384">schedule</span></span>         | [<span data-ttu-id="c4ec7-385">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c4ec7-385">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c4ec7-386">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-386">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="c4ec7-387">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ec7-387">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c4ec7-388">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ec7-388">Response</span></span>

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

### <a name="example-6-administrator-extends-expiring-role-assignment"></a><span data-ttu-id="c4ec7-389">Exemplo 6: administrador estende a atribuição de função de expiração</span><span class="sxs-lookup"><span data-stu-id="c4ec7-389">Example 6: Administrator extends expiring role assignment</span></span>

<span data-ttu-id="c4ec7-390">Este exemplo estende a atribuição de função de expiração para o usuário ANUJCUSER para o colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-390">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="c4ec7-391">**Observação:** Além da permissão, este exemplo requer que o solicitante tenha pelo menos uma `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="c4ec7-391">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

| <span data-ttu-id="c4ec7-392">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4ec7-392">Property</span></span>         | <span data-ttu-id="c4ec7-393">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-393">Type</span></span>                                                     | <span data-ttu-id="c4ec7-394">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="c4ec7-394">Required</span></span>                | <span data-ttu-id="c4ec7-395">Valor</span><span class="sxs-lookup"><span data-stu-id="c4ec7-395">Value</span></span> |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| <span data-ttu-id="c4ec7-396">resourceId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-396">resourceId</span></span>       | <span data-ttu-id="c4ec7-397">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-397">String</span></span>                                                   | <span data-ttu-id="c4ec7-398">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-398">Yes</span></span>                     | <span data-ttu-id="c4ec7-399">\<Identificação\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-399">\<resourceId\></span></span> |
| <span data-ttu-id="c4ec7-400">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c4ec7-400">roleDefinitionId</span></span> | <span data-ttu-id="c4ec7-401">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-401">String</span></span>                                                   | <span data-ttu-id="c4ec7-402">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-402">Yes</span></span>                     | <span data-ttu-id="c4ec7-403">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-403">\<roleDefinitionId\></span></span> |
| <span data-ttu-id="c4ec7-404">SubjectID</span><span class="sxs-lookup"><span data-stu-id="c4ec7-404">subjectId</span></span>        | <span data-ttu-id="c4ec7-405">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-405">String</span></span>                                                   | <span data-ttu-id="c4ec7-406">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-406">Yes</span></span>                     | <span data-ttu-id="c4ec7-407">\<SubjectID\></span><span class="sxs-lookup"><span data-stu-id="c4ec7-407">\<subjectId\></span></span> |
| <span data-ttu-id="c4ec7-408">assignmentstate</span><span class="sxs-lookup"><span data-stu-id="c4ec7-408">assignmentState</span></span>  | <span data-ttu-id="c4ec7-409">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-409">String</span></span>                                                   | <span data-ttu-id="c4ec7-410">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-410">Yes</span></span>                     | <span data-ttu-id="c4ec7-411">Qualificado/ativo</span><span class="sxs-lookup"><span data-stu-id="c4ec7-411">Eligible / Active</span></span> |
| <span data-ttu-id="c4ec7-412">type</span><span class="sxs-lookup"><span data-stu-id="c4ec7-412">type</span></span>             | <span data-ttu-id="c4ec7-413">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-413">String</span></span>                                                   | <span data-ttu-id="c4ec7-414">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-414">Yes</span></span>                     | <span data-ttu-id="c4ec7-415">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="c4ec7-415">AdminExtend</span></span> |
| <span data-ttu-id="c4ec7-416">motivos</span><span class="sxs-lookup"><span data-stu-id="c4ec7-416">reason</span></span>           | <span data-ttu-id="c4ec7-417">String</span><span class="sxs-lookup"><span data-stu-id="c4ec7-417">String</span></span>                                                   | <span data-ttu-id="c4ec7-418">depende do roleSettings</span><span class="sxs-lookup"><span data-stu-id="c4ec7-418">depends on roleSettings</span></span> |   |
| <span data-ttu-id="c4ec7-419">Cronograma</span><span class="sxs-lookup"><span data-stu-id="c4ec7-419">schedule</span></span>         | [<span data-ttu-id="c4ec7-420">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="c4ec7-420">governanceSchedule</span></span>](../resources/governanceschedule.md) | <span data-ttu-id="c4ec7-421">Sim</span><span class="sxs-lookup"><span data-stu-id="c4ec7-421">Yes</span></span>                     |   |

#### <a name="request"></a><span data-ttu-id="c4ec7-422">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4ec7-422">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="c4ec7-423">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4ec7-423">Response</span></span>

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
