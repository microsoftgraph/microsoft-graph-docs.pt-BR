---
title: Criar governanceRoleAssignmentRequest
description: Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função. A tabela a seguir lista as operações.
localization_priority: Normal
ms.openlocfilehash: 09adb824147dba745649efc7589ca763f815278d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823769"
---
# <a name="create-governanceroleassignmentrequest"></a><span data-ttu-id="a55f4-104">Criar governanceRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-104">Create governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="a55f4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a55f4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a55f4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a55f4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a55f4-107">Crie uma solicitação de atribuição de função para representar a operação desejado em uma atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a55f4-107">Create a role assignment request to represent the operation you want on a role assignment.</span></span> <span data-ttu-id="a55f4-108">A tabela a seguir lista as operações.</span><span class="sxs-lookup"><span data-stu-id="a55f4-108">The following table lists the operations.</span></span>

| <span data-ttu-id="a55f4-109">Operação</span><span class="sxs-lookup"><span data-stu-id="a55f4-109">Operation</span></span>       | <span data-ttu-id="a55f4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a55f4-110">Type</span></span> | 
|:---------------|:----------|
| <span data-ttu-id="a55f4-111">Atribuir uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="a55f4-111">Assign a role assignment</span></span>| <span data-ttu-id="a55f4-112">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="a55f4-112">AdminAdd</span></span> |
| <span data-ttu-id="a55f4-113">Ativar uma atribuição de função elegíveis</span><span class="sxs-lookup"><span data-stu-id="a55f4-113">Activate an eligible role assignment</span></span>| <span data-ttu-id="a55f4-114">UserAdd</span><span class="sxs-lookup"><span data-stu-id="a55f4-114">UserAdd</span></span> | 
| <span data-ttu-id="a55f4-115">Desativar uma atribuição de função ativada</span><span class="sxs-lookup"><span data-stu-id="a55f4-115">Deactivate an activated role assignment</span></span>| <span data-ttu-id="a55f4-116">UserRemove</span><span class="sxs-lookup"><span data-stu-id="a55f4-116">UserRemove</span></span> | 
| <span data-ttu-id="a55f4-117">Remover uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="a55f4-117">Remove a role assignment</span></span>| <span data-ttu-id="a55f4-118">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="a55f4-118">AdminRemove</span></span> |
| <span data-ttu-id="a55f4-119">Atualizar uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="a55f4-119">Update a role assignment</span></span>| <span data-ttu-id="a55f4-120">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="a55f4-120">AdminUpdate</span></span> |
| <span data-ttu-id="a55f4-121">Solicitação para estender minha atribuição de função</span><span class="sxs-lookup"><span data-stu-id="a55f4-121">Request to extend my role assignment</span></span>| <span data-ttu-id="a55f4-122">UserExtend</span><span class="sxs-lookup"><span data-stu-id="a55f4-122">UserExtend</span></span> | 
| <span data-ttu-id="a55f4-123">Estender uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="a55f4-123">Extend a role assignment</span></span>| <span data-ttu-id="a55f4-124">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="a55f4-124">AdminExtend</span></span> | 
| <span data-ttu-id="a55f4-125">Solicitação de renovação minha atribuição de função expirados</span><span class="sxs-lookup"><span data-stu-id="a55f4-125">Request to renew my expired role assignment</span></span>| <span data-ttu-id="a55f4-126">UserRenew</span><span class="sxs-lookup"><span data-stu-id="a55f4-126">UserRenew</span></span> | 
| <span data-ttu-id="a55f4-127">Renovar uma atribuição de função expirados</span><span class="sxs-lookup"><span data-stu-id="a55f4-127">Renew an expired role assignment</span></span>| <span data-ttu-id="a55f4-128">AdminRenew</span><span class="sxs-lookup"><span data-stu-id="a55f4-128">AdminRenew</span></span> | 

 
## <a name="permissions"></a><span data-ttu-id="a55f4-129">Permissions</span><span class="sxs-lookup"><span data-stu-id="a55f4-129">Permissions</span></span>
<span data-ttu-id="a55f4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a55f4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a55f4-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a55f4-132">Permission type</span></span>      | <span data-ttu-id="a55f4-133">Permissions</span><span class="sxs-lookup"><span data-stu-id="a55f4-133">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a55f4-134">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a55f4-134">Delegated (work or school account)</span></span> | <span data-ttu-id="a55f4-135">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a55f4-135">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a55f4-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a55f4-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a55f4-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a55f4-137">Not supported.</span></span>    |
|<span data-ttu-id="a55f4-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a55f4-138">Application</span></span> | <span data-ttu-id="a55f4-139">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a55f4-139">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="a55f4-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a55f4-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="a55f4-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a55f4-141">Request headers</span></span>
| <span data-ttu-id="a55f4-142">Nome</span><span class="sxs-lookup"><span data-stu-id="a55f4-142">Name</span></span>       | <span data-ttu-id="a55f4-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a55f4-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a55f4-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="a55f4-144">Authorization</span></span>  | <span data-ttu-id="a55f4-145">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a55f4-145">Bearer {code}</span></span>|
| <span data-ttu-id="a55f4-146">Content-type</span><span class="sxs-lookup"><span data-stu-id="a55f4-146">Content-type</span></span>  | <span data-ttu-id="a55f4-147">application/json</span><span class="sxs-lookup"><span data-stu-id="a55f4-147">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a55f4-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a55f4-148">Request body</span></span>
<span data-ttu-id="a55f4-149">No corpo da solicitação, fornece uma representação JSON de um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="a55f4-149">In the request body, supply a JSON representation of a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object.</span></span> 

| <span data-ttu-id="a55f4-150">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a55f4-150">Property</span></span>     | <span data-ttu-id="a55f4-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="a55f4-151">Type</span></span>    |<span data-ttu-id="a55f4-152">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a55f4-152">Required</span></span>|  <span data-ttu-id="a55f4-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="a55f4-153">Description</span></span>|
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="a55f4-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="a55f4-154">resourceId</span></span>|<span data-ttu-id="a55f4-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-155">String</span></span>|<span data-ttu-id="a55f4-156">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-156">Yes</span></span>|<span data-ttu-id="a55f4-157">A ID do recurso.</span><span class="sxs-lookup"><span data-stu-id="a55f4-157">The ID of the resource.</span></span>|
|<span data-ttu-id="a55f4-158">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a55f4-158">roleDefinitionId</span></span>|<span data-ttu-id="a55f4-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-159">String</span></span>|<span data-ttu-id="a55f4-160">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-160">Yes</span></span>|<span data-ttu-id="a55f4-161">A ID da definição de função.</span><span class="sxs-lookup"><span data-stu-id="a55f4-161">The ID of the role definition.</span></span>|
|<span data-ttu-id="a55f4-162">subjectId</span><span class="sxs-lookup"><span data-stu-id="a55f4-162">subjectId</span></span>|<span data-ttu-id="a55f4-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-163">String</span></span>|<span data-ttu-id="a55f4-164">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-164">Yes</span></span>|<span data-ttu-id="a55f4-165">A identificação do assunto.</span><span class="sxs-lookup"><span data-stu-id="a55f4-165">The ID of the subject.</span></span>|
|<span data-ttu-id="a55f4-166">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a55f4-166">assignmentState</span></span>|<span data-ttu-id="a55f4-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-167">String</span></span>|<span data-ttu-id="a55f4-168">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-168">Yes</span></span>|<span data-ttu-id="a55f4-169">O estado da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a55f4-169">The state of assignment.</span></span> <span data-ttu-id="a55f4-170">O valor pode ser ``Eligible`` e ``Active``.</span><span class="sxs-lookup"><span data-stu-id="a55f4-170">The value can be ``Eligible`` and ``Active``.</span></span>|
|<span data-ttu-id="a55f4-171">type</span><span class="sxs-lookup"><span data-stu-id="a55f4-171">type</span></span>|<span data-ttu-id="a55f4-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-172">String</span></span>|<span data-ttu-id="a55f4-173">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-173">Yes</span></span>|<span data-ttu-id="a55f4-174">O tipo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a55f4-174">The request type.</span></span> <span data-ttu-id="a55f4-175">O valor pode ser `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`e `AdminExtend`.</span><span class="sxs-lookup"><span data-stu-id="a55f4-175">The value can be `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`and `AdminExtend`.</span></span>|
|<span data-ttu-id="a55f4-176">motivo</span><span class="sxs-lookup"><span data-stu-id="a55f4-176">reason</span></span>|<span data-ttu-id="a55f4-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-177">String</span></span>| |<span data-ttu-id="a55f4-178">O motivo pelo qual deve ser fornecido para a solicitação de atribuição de função de auditoria e revise finalidade.</span><span class="sxs-lookup"><span data-stu-id="a55f4-178">The reason needs to be provided for the role assignment request for audit and review purpose.</span></span>|
|<span data-ttu-id="a55f4-179">agenda</span><span class="sxs-lookup"><span data-stu-id="a55f4-179">schedule</span></span>|[<span data-ttu-id="a55f4-180">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a55f4-180">governanceSchedule</span></span>](../resources/governanceschedule.md)| | <span data-ttu-id="a55f4-181">O agendamento da solicitação de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a55f4-181">The schedule of the role assignment request.</span></span> <span data-ttu-id="a55f4-182">Tipo de solicitação de `UserAdd`, `AdminAdd`, `AdminUpdate`, e `AdminExtend`, é necessário.</span><span class="sxs-lookup"><span data-stu-id="a55f4-182">For request type of `UserAdd`, `AdminAdd`, `AdminUpdate`, and `AdminExtend`, it is required.</span></span>|

## <a name="response"></a><span data-ttu-id="a55f4-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55f4-183">Response</span></span>
<span data-ttu-id="a55f4-184">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a55f4-184">If successful, this method returns a `201 Created` response code and a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) object in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="a55f4-185">Códigos de erro</span><span class="sxs-lookup"><span data-stu-id="a55f4-185">Error codes</span></span>
<span data-ttu-id="a55f4-186">Essa API retorna os códigos de erro HTTP padrão.</span><span class="sxs-lookup"><span data-stu-id="a55f4-186">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="a55f4-187">Além disso, ele também retorna os códigos de erro listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a55f4-187">In addition, it also returns the error codes listed in the following table.</span></span>

|<span data-ttu-id="a55f4-188">Código de erro</span><span class="sxs-lookup"><span data-stu-id="a55f4-188">Error code</span></span>     | <span data-ttu-id="a55f4-189">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="a55f4-189">Error message</span></span>              | <span data-ttu-id="a55f4-190">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a55f4-190">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="a55f4-191">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-191">400 BadRequest</span></span> | <span data-ttu-id="a55f4-192">RoleNotFound</span><span class="sxs-lookup"><span data-stu-id="a55f4-192">RoleNotFound</span></span>    | <span data-ttu-id="a55f4-193">O `roleDefinitionId` fornecida na solicitação de corpo não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="a55f4-193">The `roleDefinitionId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="a55f4-194">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-194">400 BadRequest</span></span> | <span data-ttu-id="a55f4-195">ResourceIsLocked</span><span class="sxs-lookup"><span data-stu-id="a55f4-195">ResourceIsLocked</span></span>    | <span data-ttu-id="a55f4-196">O recurso fornecido no corpo da solicitação está em estado de `Locked` e não pode criar solicitações de atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="a55f4-196">The resource provided in the request body is in state of `Locked` and cannot create role assignment requests.</span></span>
| <span data-ttu-id="a55f4-197">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-197">400 BadRequest</span></span> | <span data-ttu-id="a55f4-198">SubjectNotFound</span><span class="sxs-lookup"><span data-stu-id="a55f4-198">SubjectNotFound</span></span>    | <span data-ttu-id="a55f4-199">O `subjectId` fornecida na solicitação de corpo não pode ser encontrado.</span><span class="sxs-lookup"><span data-stu-id="a55f4-199">The `subjectId` provided in the request body cannot be found.</span></span>
| <span data-ttu-id="a55f4-200">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-200">400 BadRequest</span></span> | <span data-ttu-id="a55f4-201">PendingRoleAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-201">PendingRoleAssignmentRequest</span></span>    | <span data-ttu-id="a55f4-202">Já existe uma pendente [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) no sistema.</span><span class="sxs-lookup"><span data-stu-id="a55f4-202">There already exists a pending [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) in the system.</span></span>
| <span data-ttu-id="a55f4-203">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-203">400 BadRequest</span></span> | <span data-ttu-id="a55f4-204">RoleAssignmentExists</span><span class="sxs-lookup"><span data-stu-id="a55f4-204">RoleAssignmentExists</span></span>    | <span data-ttu-id="a55f4-205">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser criada já existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="a55f4-205">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be created already exists in the system.</span></span>
| <span data-ttu-id="a55f4-206">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-206">400 BadRequest</span></span> | <span data-ttu-id="a55f4-207">RoleAssignmentDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="a55f4-207">RoleAssignmentDoesNotExist</span></span>    | <span data-ttu-id="a55f4-208">[GovernanceRoleAssignment](../resources/governanceroleassignment.md) solicitado a ser atualizado/estendido não existe no sistema.</span><span class="sxs-lookup"><span data-stu-id="a55f4-208">The [governanceRoleAssignment](../resources/governanceroleassignment.md) requested to be updated/extended does not exist in the system.</span></span>
| <span data-ttu-id="a55f4-209">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a55f4-209">400 BadRequest</span></span> | <span data-ttu-id="a55f4-210">RoleAssignmentRequestPolicyValidationFailed</span><span class="sxs-lookup"><span data-stu-id="a55f4-210">RoleAssignmentRequestPolicyValidationFailed</span></span> | <span data-ttu-id="a55f4-211">O [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) não atende às políticas internas e não pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="a55f4-211">The [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) does not meet internal policies and cannot be created.</span></span>

## <a name="examples"></a><span data-ttu-id="a55f4-212">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a55f4-212">Examples</span></span>
<span data-ttu-id="a55f4-213">Os exemplos a seguir mostram como usar essa API.</span><span class="sxs-lookup"><span data-stu-id="a55f4-213">The following examples show how to use this API.</span></span>

### <a name="example-1"></a><span data-ttu-id="a55f4-214">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="a55f4-214">Example 1</span></span>
<span data-ttu-id="a55f4-215">Neste exemplo, os administradores atribuem nawu@fimdev.net usuário à função Leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="a55f4-215">In this example, administrators assign user nawu@fimdev.net to the Billing Reader role.</span></span>

 ><span data-ttu-id="a55f4-216">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="a55f4-216">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="a55f4-217">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a55f4-217">Property</span></span>     | <span data-ttu-id="a55f4-218">Tipo</span><span class="sxs-lookup"><span data-stu-id="a55f4-218">Type</span></span>    |<span data-ttu-id="a55f4-219">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a55f4-219">Required</span></span>|  <span data-ttu-id="a55f4-220">Valor</span><span class="sxs-lookup"><span data-stu-id="a55f4-220">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="a55f4-221">resourceId</span><span class="sxs-lookup"><span data-stu-id="a55f4-221">resourceId</span></span>|<span data-ttu-id="a55f4-222">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-222">String</span></span>|<span data-ttu-id="a55f4-223">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-223">Yes</span></span>|<span data-ttu-id="a55f4-224">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-224">\<resourceId\></span></span>|
|<span data-ttu-id="a55f4-225">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a55f4-225">roleDefinitionId</span></span>|<span data-ttu-id="a55f4-226">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-226">String</span></span>|<span data-ttu-id="a55f4-227">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-227">Yes</span></span>|<span data-ttu-id="a55f4-228">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-228">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="a55f4-229">subjectId</span><span class="sxs-lookup"><span data-stu-id="a55f4-229">subjectId</span></span>|<span data-ttu-id="a55f4-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-230">String</span></span>|<span data-ttu-id="a55f4-231">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-231">Yes</span></span>|<span data-ttu-id="a55f4-232">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-232">\<subjectId\></span></span>|
|<span data-ttu-id="a55f4-233">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a55f4-233">assignmentState</span></span>|<span data-ttu-id="a55f4-234">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-234">String</span></span>|<span data-ttu-id="a55f4-235">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-235">Yes</span></span>| <span data-ttu-id="a55f4-236">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="a55f4-236">Eligible / Active</span></span>|
|<span data-ttu-id="a55f4-237">type</span><span class="sxs-lookup"><span data-stu-id="a55f4-237">type</span></span>|<span data-ttu-id="a55f4-238">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-238">String</span></span>|<span data-ttu-id="a55f4-239">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-239">Yes</span></span>| <span data-ttu-id="a55f4-240">AdminAdd</span><span class="sxs-lookup"><span data-stu-id="a55f4-240">AdminAdd</span></span>|
|<span data-ttu-id="a55f4-241">motivo</span><span class="sxs-lookup"><span data-stu-id="a55f4-241">reason</span></span>|<span data-ttu-id="a55f4-242">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-242">String</span></span>| <span data-ttu-id="a55f4-243">depende de configurações de função</span><span class="sxs-lookup"><span data-stu-id="a55f4-243">depends on role Settings</span></span>||
|<span data-ttu-id="a55f4-244">agenda</span><span class="sxs-lookup"><span data-stu-id="a55f4-244">schedule</span></span>|[<span data-ttu-id="a55f4-245">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a55f4-245">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a55f4-246">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-246">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="a55f4-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a55f4-247">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Eligible",
"type":"AdminAdd",
"reason":"Assign an eligible role",
"schedule":{
  "startDateTime":"2018-05-12T23:37:43.356Z",
  "endDateTime":"2018-11-08T23:37:43.356Z",
  "type":"Once"
  }
}
```
##### <a name="response"></a><span data-ttu-id="a55f4-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55f4-248">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

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

### <a name="example-2"></a><span data-ttu-id="a55f4-249">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="a55f4-249">Example 2</span></span>
<span data-ttu-id="a55f4-250">Neste exemplo, nawu@fimdev.net o usuário ativa a função de leitor de faturamento elegível.</span><span class="sxs-lookup"><span data-stu-id="a55f4-250">In this example, the user nawu@fimdev.net activates the eligible Billing Reader role.</span></span>

| <span data-ttu-id="a55f4-251">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a55f4-251">Property</span></span>     | <span data-ttu-id="a55f4-252">Tipo</span><span class="sxs-lookup"><span data-stu-id="a55f4-252">Type</span></span>    |<span data-ttu-id="a55f4-253">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a55f4-253">Required</span></span>|  <span data-ttu-id="a55f4-254">Valor</span><span class="sxs-lookup"><span data-stu-id="a55f4-254">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="a55f4-255">resourceId</span><span class="sxs-lookup"><span data-stu-id="a55f4-255">resourceId</span></span>|<span data-ttu-id="a55f4-256">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-256">String</span></span>|<span data-ttu-id="a55f4-257">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-257">Yes</span></span>|<span data-ttu-id="a55f4-258">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-258">\<resourceId\></span></span>|
|<span data-ttu-id="a55f4-259">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a55f4-259">roleDefinitionId</span></span>|<span data-ttu-id="a55f4-260">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-260">String</span></span>|<span data-ttu-id="a55f4-261">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-261">Yes</span></span>|<span data-ttu-id="a55f4-262">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-262">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="a55f4-263">subjectId</span><span class="sxs-lookup"><span data-stu-id="a55f4-263">subjectId</span></span>|<span data-ttu-id="a55f4-264">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-264">String</span></span>|<span data-ttu-id="a55f4-265">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-265">Yes</span></span>|<span data-ttu-id="a55f4-266">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-266">\<subjectId\></span></span>|
|<span data-ttu-id="a55f4-267">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a55f4-267">assignmentState</span></span>|<span data-ttu-id="a55f4-268">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-268">String</span></span>|<span data-ttu-id="a55f4-269">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-269">Yes</span></span>| <span data-ttu-id="a55f4-270">Ativo</span><span class="sxs-lookup"><span data-stu-id="a55f4-270">Active</span></span>|
|<span data-ttu-id="a55f4-271">type</span><span class="sxs-lookup"><span data-stu-id="a55f4-271">type</span></span>|<span data-ttu-id="a55f4-272">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-272">String</span></span>|<span data-ttu-id="a55f4-273">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-273">Yes</span></span>| <span data-ttu-id="a55f4-274">UserAdd</span><span class="sxs-lookup"><span data-stu-id="a55f4-274">UserAdd</span></span>|
|<span data-ttu-id="a55f4-275">motivo</span><span class="sxs-lookup"><span data-stu-id="a55f4-275">reason</span></span>|<span data-ttu-id="a55f4-276">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-276">String</span></span>| <span data-ttu-id="a55f4-277">depende de configurações de função</span><span class="sxs-lookup"><span data-stu-id="a55f4-277">depends on role Settings</span></span>||
|<span data-ttu-id="a55f4-278">agenda</span><span class="sxs-lookup"><span data-stu-id="a55f4-278">schedule</span></span>|[<span data-ttu-id="a55f4-279">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a55f4-279">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a55f4-280">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-280">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="a55f4-281">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a55f4-281">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"8b4d1d51-08e9-4254-b0a6-b16177aae376",
"resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserAdd",
"reason": "Activate the owner role",
"schedule":{
  "type":"Once",
  "startDateTime":"2018-05-12T23:28:43.537Z",
  "duration":"PT9H"
  },
"linkedEligibleRoleAssignmentId":"e327f4be-42a0-47a2-8579-0a39b025b394"
}
```
##### <a name="response"></a><span data-ttu-id="a55f4-282">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55f4-282">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
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

### <a name="example-3"></a><span data-ttu-id="a55f4-283">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="a55f4-283">Example 3</span></span>
<span data-ttu-id="a55f4-284">Neste exemplo, o nawu@fimdev.net usuário desativa a função de leitor de cobrança ativa.</span><span class="sxs-lookup"><span data-stu-id="a55f4-284">In this example, the user nawu@fimdev.net deactivates the active Billing Reader role.</span></span>

| <span data-ttu-id="a55f4-285">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a55f4-285">Property</span></span>     | <span data-ttu-id="a55f4-286">Tipo</span><span class="sxs-lookup"><span data-stu-id="a55f4-286">Type</span></span>    |<span data-ttu-id="a55f4-287">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a55f4-287">Required</span></span>|  <span data-ttu-id="a55f4-288">Valor</span><span class="sxs-lookup"><span data-stu-id="a55f4-288">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="a55f4-289">resourceId</span><span class="sxs-lookup"><span data-stu-id="a55f4-289">resourceId</span></span>|<span data-ttu-id="a55f4-290">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-290">String</span></span>|<span data-ttu-id="a55f4-291">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-291">Yes</span></span>|<span data-ttu-id="a55f4-292">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-292">\<resourceId\></span></span>|
|<span data-ttu-id="a55f4-293">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a55f4-293">roleDefinitionId</span></span>|<span data-ttu-id="a55f4-294">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-294">String</span></span>|<span data-ttu-id="a55f4-295">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-295">Yes</span></span>|<span data-ttu-id="a55f4-296">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-296">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="a55f4-297">subjectId</span><span class="sxs-lookup"><span data-stu-id="a55f4-297">subjectId</span></span>|<span data-ttu-id="a55f4-298">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-298">String</span></span>|<span data-ttu-id="a55f4-299">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-299">Yes</span></span>|<span data-ttu-id="a55f4-300">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-300">\<subjectId\></span></span>|
|<span data-ttu-id="a55f4-301">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a55f4-301">assignmentState</span></span>|<span data-ttu-id="a55f4-302">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-302">String</span></span>|<span data-ttu-id="a55f4-303">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-303">Yes</span></span>| <span data-ttu-id="a55f4-304">Ativo</span><span class="sxs-lookup"><span data-stu-id="a55f4-304">Active</span></span>|
|<span data-ttu-id="a55f4-305">type</span><span class="sxs-lookup"><span data-stu-id="a55f4-305">type</span></span>|<span data-ttu-id="a55f4-306">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-306">String</span></span>|<span data-ttu-id="a55f4-307">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-307">Yes</span></span>| <span data-ttu-id="a55f4-308">UserRemove</span><span class="sxs-lookup"><span data-stu-id="a55f4-308">UserRemove</span></span>|
|<span data-ttu-id="a55f4-309">motivo</span><span class="sxs-lookup"><span data-stu-id="a55f4-309">reason</span></span>|<span data-ttu-id="a55f4-310">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-310">String</span></span>| <span data-ttu-id="a55f4-311">Não</span><span class="sxs-lookup"><span data-stu-id="a55f4-311">No</span></span>||
|<span data-ttu-id="a55f4-312">agenda</span><span class="sxs-lookup"><span data-stu-id="a55f4-312">schedule</span></span>|[<span data-ttu-id="a55f4-313">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a55f4-313">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a55f4-314">Não</span><span class="sxs-lookup"><span data-stu-id="a55f4-314">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="a55f4-315">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a55f4-315">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{"roleDefinitionId":"bc75b4e6-7403-4243-bf2f-d1f6990be122",
"resourceId":"fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
"subjectId":"918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
"assignmentState":"Active",
"type":"UserRemove",
"reason":"Deactivate the role",
"linkedEligibleRoleAssignmentId":"cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```
##### <a name="response"></a><span data-ttu-id="a55f4-316">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55f4-316">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

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

### <a name="example-4"></a><span data-ttu-id="a55f4-317">Exemplo 4</span><span class="sxs-lookup"><span data-stu-id="a55f4-317">Example 4</span></span>
<span data-ttu-id="a55f4-318">Neste exemplo, os administradores remover nawu@fimdev.net o usuário da função Leitor de cobrança.</span><span class="sxs-lookup"><span data-stu-id="a55f4-318">In this example, administrators remove the user nawu@fimdev.net from the Billing Reader role.</span></span>

 ><span data-ttu-id="a55f4-319">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="a55f4-319">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="a55f4-320">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a55f4-320">Property</span></span>     | <span data-ttu-id="a55f4-321">Tipo</span><span class="sxs-lookup"><span data-stu-id="a55f4-321">Type</span></span>    |<span data-ttu-id="a55f4-322">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a55f4-322">Required</span></span>|  <span data-ttu-id="a55f4-323">Valor</span><span class="sxs-lookup"><span data-stu-id="a55f4-323">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="a55f4-324">resourceId</span><span class="sxs-lookup"><span data-stu-id="a55f4-324">resourceId</span></span>|<span data-ttu-id="a55f4-325">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-325">String</span></span>|<span data-ttu-id="a55f4-326">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-326">Yes</span></span>|<span data-ttu-id="a55f4-327">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-327">\<resourceId\></span></span>|
|<span data-ttu-id="a55f4-328">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a55f4-328">roleDefinitionId</span></span>|<span data-ttu-id="a55f4-329">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-329">String</span></span>|<span data-ttu-id="a55f4-330">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-330">Yes</span></span>|<span data-ttu-id="a55f4-331">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-331">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="a55f4-332">subjectId</span><span class="sxs-lookup"><span data-stu-id="a55f4-332">subjectId</span></span>|<span data-ttu-id="a55f4-333">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-333">String</span></span>|<span data-ttu-id="a55f4-334">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-334">Yes</span></span>|<span data-ttu-id="a55f4-335">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-335">\<subjectId\></span></span>|
|<span data-ttu-id="a55f4-336">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a55f4-336">assignmentState</span></span>|<span data-ttu-id="a55f4-337">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-337">String</span></span>|<span data-ttu-id="a55f4-338">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-338">Yes</span></span>| <span data-ttu-id="a55f4-339">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="a55f4-339">Eligible / Active</span></span>|
|<span data-ttu-id="a55f4-340">type</span><span class="sxs-lookup"><span data-stu-id="a55f4-340">type</span></span>|<span data-ttu-id="a55f4-341">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-341">String</span></span>|<span data-ttu-id="a55f4-342">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-342">Yes</span></span>| <span data-ttu-id="a55f4-343">AdminRemove</span><span class="sxs-lookup"><span data-stu-id="a55f4-343">AdminRemove</span></span>|
|<span data-ttu-id="a55f4-344">motivo</span><span class="sxs-lookup"><span data-stu-id="a55f4-344">reason</span></span>|<span data-ttu-id="a55f4-345">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-345">String</span></span>| <span data-ttu-id="a55f4-346">Não</span><span class="sxs-lookup"><span data-stu-id="a55f4-346">No</span></span>||
|<span data-ttu-id="a55f4-347">agenda</span><span class="sxs-lookup"><span data-stu-id="a55f4-347">schedule</span></span>|[<span data-ttu-id="a55f4-348">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a55f4-348">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a55f4-349">Não</span><span class="sxs-lookup"><span data-stu-id="a55f4-349">No</span></span>|        |
##### <a name="request"></a><span data-ttu-id="a55f4-350">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a55f4-350">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminRemove"
}
```
##### <a name="response"></a><span data-ttu-id="a55f4-351">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55f4-351">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminRemove",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"Closed",
    "subStatus":"Revoked",
    "statusDetails":[]
  },
  "schedule":null
}
```

### <a name="example-5"></a><span data-ttu-id="a55f4-352">Exemplo 5</span><span class="sxs-lookup"><span data-stu-id="a55f4-352">Example 5</span></span>
<span data-ttu-id="a55f4-353">Neste exemplo, os administradores atualizar a atribuição de função para o usuário de nawu@fimdev.net ao proprietário.</span><span class="sxs-lookup"><span data-stu-id="a55f4-353">In this example, administrators update the role assignment for the user nawu@fimdev.net to Owner.</span></span>

 ><span data-ttu-id="a55f4-354">**Observação:** Além de permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="a55f4-354">**Note:** In addition to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span> 

| <span data-ttu-id="a55f4-355">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a55f4-355">Property</span></span>     | <span data-ttu-id="a55f4-356">Tipo</span><span class="sxs-lookup"><span data-stu-id="a55f4-356">Type</span></span>    |<span data-ttu-id="a55f4-357">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a55f4-357">Required</span></span>|  <span data-ttu-id="a55f4-358">Valor</span><span class="sxs-lookup"><span data-stu-id="a55f4-358">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="a55f4-359">resourceId</span><span class="sxs-lookup"><span data-stu-id="a55f4-359">resourceId</span></span>|<span data-ttu-id="a55f4-360">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-360">String</span></span>|<span data-ttu-id="a55f4-361">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-361">Yes</span></span>|<span data-ttu-id="a55f4-362">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-362">\<resourceId\></span></span>|
|<span data-ttu-id="a55f4-363">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a55f4-363">roleDefinitionId</span></span>|<span data-ttu-id="a55f4-364">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-364">String</span></span>|<span data-ttu-id="a55f4-365">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-365">Yes</span></span>|<span data-ttu-id="a55f4-366">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-366">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="a55f4-367">subjectId</span><span class="sxs-lookup"><span data-stu-id="a55f4-367">subjectId</span></span>|<span data-ttu-id="a55f4-368">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-368">String</span></span>|<span data-ttu-id="a55f4-369">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-369">Yes</span></span>|<span data-ttu-id="a55f4-370">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-370">\<subjectId\></span></span>|
|<span data-ttu-id="a55f4-371">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a55f4-371">assignmentState</span></span>|<span data-ttu-id="a55f4-372">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-372">String</span></span>|<span data-ttu-id="a55f4-373">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-373">Yes</span></span>| <span data-ttu-id="a55f4-374">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="a55f4-374">Eligible / Active</span></span>|
|<span data-ttu-id="a55f4-375">type</span><span class="sxs-lookup"><span data-stu-id="a55f4-375">type</span></span>|<span data-ttu-id="a55f4-376">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-376">String</span></span>|<span data-ttu-id="a55f4-377">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-377">Yes</span></span>| <span data-ttu-id="a55f4-378">AdminUpdate</span><span class="sxs-lookup"><span data-stu-id="a55f4-378">AdminUpdate</span></span>|
|<span data-ttu-id="a55f4-379">motivo</span><span class="sxs-lookup"><span data-stu-id="a55f4-379">reason</span></span>|<span data-ttu-id="a55f4-380">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-380">String</span></span>| <span data-ttu-id="a55f4-381">depende roleSettings</span><span class="sxs-lookup"><span data-stu-id="a55f4-381">depends on roleSettings</span></span>||
|<span data-ttu-id="a55f4-382">agenda</span><span class="sxs-lookup"><span data-stu-id="a55f4-382">schedule</span></span>|[<span data-ttu-id="a55f4-383">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a55f4-383">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a55f4-384">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-384">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="a55f4-385">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a55f4-385">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState":"Eligible",
  "type":"AdminUpdate",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31.000Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="a55f4-386">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55f4-386">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId":"1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminUpdate",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":null,
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-03-08T05:42:45.317Z",
    "endDateTime":"2018-06-05T05:42:31Z",
    "duration":"PT0S"
  }
}
```

### <a name="example-6"></a><span data-ttu-id="a55f4-387">Exemplo 6</span><span class="sxs-lookup"><span data-stu-id="a55f4-387">Example 6</span></span>
<span data-ttu-id="a55f4-388">Este exemplo estende a atribuição de função expirar para usuário ANUJCUSER Colaborador do serviço de gerenciamento de API.</span><span class="sxs-lookup"><span data-stu-id="a55f4-388">This example extends the expiring role assignment for user ANUJCUSER to API Management Service Contributor.</span></span>

 ><span data-ttu-id="a55f4-389">**Observação:** Additon à permissão, este exemplo exige que o solicitante tem pelo menos um `Active` atribuição de função de administrador (`owner` ou `user access administrator`) no recurso.</span><span class="sxs-lookup"><span data-stu-id="a55f4-389">**Note:** In additon to the permission, this example requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
 
| <span data-ttu-id="a55f4-390">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a55f4-390">Property</span></span>     | <span data-ttu-id="a55f4-391">Tipo</span><span class="sxs-lookup"><span data-stu-id="a55f4-391">Type</span></span>    |<span data-ttu-id="a55f4-392">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="a55f4-392">Required</span></span>|  <span data-ttu-id="a55f4-393">Valor</span><span class="sxs-lookup"><span data-stu-id="a55f4-393">Value</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="a55f4-394">resourceId</span><span class="sxs-lookup"><span data-stu-id="a55f4-394">resourceId</span></span>|<span data-ttu-id="a55f4-395">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-395">String</span></span>|<span data-ttu-id="a55f4-396">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-396">Yes</span></span>|<span data-ttu-id="a55f4-397">\<resourceId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-397">\<resourceId\></span></span>|
|<span data-ttu-id="a55f4-398">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="a55f4-398">roleDefinitionId</span></span>|<span data-ttu-id="a55f4-399">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-399">String</span></span>|<span data-ttu-id="a55f4-400">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-400">Yes</span></span>|<span data-ttu-id="a55f4-401">\<roleDefinitionId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-401">\<roleDefinitionId\></span></span>|
|<span data-ttu-id="a55f4-402">subjectId</span><span class="sxs-lookup"><span data-stu-id="a55f4-402">subjectId</span></span>|<span data-ttu-id="a55f4-403">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-403">String</span></span>|<span data-ttu-id="a55f4-404">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-404">Yes</span></span>|<span data-ttu-id="a55f4-405">\<subjectId\></span><span class="sxs-lookup"><span data-stu-id="a55f4-405">\<subjectId\></span></span>|
|<span data-ttu-id="a55f4-406">assignmentState</span><span class="sxs-lookup"><span data-stu-id="a55f4-406">assignmentState</span></span>|<span data-ttu-id="a55f4-407">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-407">String</span></span>|<span data-ttu-id="a55f4-408">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-408">Yes</span></span>| <span data-ttu-id="a55f4-409">Elegíveis / ativo</span><span class="sxs-lookup"><span data-stu-id="a55f4-409">Eligible / Active</span></span> |
|<span data-ttu-id="a55f4-410">type</span><span class="sxs-lookup"><span data-stu-id="a55f4-410">type</span></span>|<span data-ttu-id="a55f4-411">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-411">String</span></span>|<span data-ttu-id="a55f4-412">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-412">Yes</span></span>| <span data-ttu-id="a55f4-413">AdminExtend</span><span class="sxs-lookup"><span data-stu-id="a55f4-413">AdminExtend</span></span>|
|<span data-ttu-id="a55f4-414">motivo</span><span class="sxs-lookup"><span data-stu-id="a55f4-414">reason</span></span>|<span data-ttu-id="a55f4-415">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a55f4-415">String</span></span>| <span data-ttu-id="a55f4-416">depende roleSettings</span><span class="sxs-lookup"><span data-stu-id="a55f4-416">depends on roleSettings</span></span>||
|<span data-ttu-id="a55f4-417">agenda</span><span class="sxs-lookup"><span data-stu-id="a55f4-417">schedule</span></span>|[<span data-ttu-id="a55f4-418">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a55f4-418">governanceSchedule</span></span>](../resources/governanceschedule.md)|<span data-ttu-id="a55f4-419">Sim</span><span class="sxs-lookup"><span data-stu-id="a55f4-419">Yes</span></span>|        |
##### <a name="request"></a><span data-ttu-id="a55f4-420">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a55f4-420">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState":"Eligible",
  "type":"AdminExtend",
  "reason":"extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z"
  }
}
```
##### <a name="response"></a><span data-ttu-id="a55f4-421">Resposta</span><span class="sxs-lookup"><span data-stu-id="a55f4-421">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->
```json
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 226

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id":"486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId":"e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId":"0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId":"74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId":"",
  "type":"AdminExtend",
  "assignmentState":"Eligible",
  "requestedDateTime":"0001-01-01T00:00:00Z",
  "reason":"extend role assignment",
  "status":{
    "status":"InProgress",
    "subStatus":"Granted",
    "statusDetails":[
      {
        "key":"AdminRequestRule","value":"Grant"
      },{
        "key":"ExpirationRule","value":"Grant"
      },{
        "key":"MfaRule","value":"Grant"
      }
    ]
  },
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-05-12T23:53:55.327Z",
    "endDateTime":"2018-08-10T23:53:55.327Z",
    "duration":"PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
