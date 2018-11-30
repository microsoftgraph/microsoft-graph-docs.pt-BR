---
title: Atualizar approleassignment
description: Atualize as propriedades do objeto approleassignment.
ms.openlocfilehash: 3c861afde396d9cab2f745c15c7de1d9a81c5dcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033708"
---
# <a name="update-approleassignment"></a><span data-ttu-id="eacae-103">Atualizar approleassignment</span><span class="sxs-lookup"><span data-stu-id="eacae-103">Update approleassignment</span></span>

> <span data-ttu-id="eacae-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eacae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eacae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eacae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eacae-106">Atualize as propriedades do objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="eacae-106">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="eacae-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="eacae-107">Permissions</span></span>
<span data-ttu-id="eacae-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eacae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eacae-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eacae-110">Permission type</span></span>      | <span data-ttu-id="eacae-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eacae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eacae-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eacae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eacae-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eacae-113">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="eacae-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eacae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eacae-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eacae-115">Not supported.</span></span>    |
|<span data-ttu-id="eacae-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eacae-116">Application</span></span> | <span data-ttu-id="eacae-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eacae-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eacae-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eacae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eacae-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eacae-119">Request headers</span></span>
| <span data-ttu-id="eacae-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eacae-120">Name</span></span>       | <span data-ttu-id="eacae-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="eacae-121">Type</span></span> | <span data-ttu-id="eacae-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="eacae-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eacae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="eacae-123">Authorization</span></span>  | <span data-ttu-id="eacae-124">string</span><span class="sxs-lookup"><span data-stu-id="eacae-124">string</span></span>  | <span data-ttu-id="eacae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eacae-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eacae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eacae-127">Request body</span></span>
<span data-ttu-id="eacae-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="eacae-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="eacae-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eacae-131">Property</span></span>     | <span data-ttu-id="eacae-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eacae-132">Type</span></span>   |<span data-ttu-id="eacae-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eacae-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eacae-134">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="eacae-134">creationTimestamp</span></span>|<span data-ttu-id="eacae-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eacae-135">DateTimeOffset</span></span>|<span data-ttu-id="eacae-136">A hora em que a concessão foi criada.</span><span class="sxs-lookup"><span data-stu-id="eacae-136">The time when the grant was created.</span></span>|
|<span data-ttu-id="eacae-137">id</span><span class="sxs-lookup"><span data-stu-id="eacae-137">id</span></span>|<span data-ttu-id="eacae-138">Guid</span><span class="sxs-lookup"><span data-stu-id="eacae-138">Guid</span></span>|<span data-ttu-id="eacae-139">A id de função que foi atribuída à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="eacae-139">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="eacae-140">Essa função deve ser declarada pelo destino recurso aplicativo **resourceId** em sua propriedade **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="eacae-140">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="eacae-141">Onde o recurso não declarar todas as permissões, uma id do padrão (zero GUID) deve ser especificada.</span><span class="sxs-lookup"><span data-stu-id="eacae-141">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="eacae-142">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="eacae-142">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="eacae-143">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="eacae-143">principalDisplayName</span></span>|<span data-ttu-id="eacae-144">String</span><span class="sxs-lookup"><span data-stu-id="eacae-144">String</span></span>|<span data-ttu-id="eacae-145">O nome de exibição da entidade que foi concedido o acesso.</span><span class="sxs-lookup"><span data-stu-id="eacae-145">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="eacae-146">principalId</span><span class="sxs-lookup"><span data-stu-id="eacae-146">principalId</span></span>|<span data-ttu-id="eacae-147">Guid</span><span class="sxs-lookup"><span data-stu-id="eacae-147">Guid</span></span>|<span data-ttu-id="eacae-148">O identificador exclusivo (**objectId**) para a entidade sendo concedida o acesso.</span><span class="sxs-lookup"><span data-stu-id="eacae-148">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="eacae-149">**Observações**: necessários.</span><span class="sxs-lookup"><span data-stu-id="eacae-149">**Notes**: required.</span></span>            |
|<span data-ttu-id="eacae-150">principalType</span><span class="sxs-lookup"><span data-stu-id="eacae-150">principalType</span></span>|<span data-ttu-id="eacae-151">String</span><span class="sxs-lookup"><span data-stu-id="eacae-151">String</span></span>|<span data-ttu-id="eacae-152">O tipo de entidade.</span><span class="sxs-lookup"><span data-stu-id="eacae-152">The type of principal.</span></span>  <span data-ttu-id="eacae-153">Isso pode ser "User", "Grupo" ou "ServicePrincipal".</span><span class="sxs-lookup"><span data-stu-id="eacae-153">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="eacae-154">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="eacae-154">resourceDisplayName</span></span>|<span data-ttu-id="eacae-155">String</span><span class="sxs-lookup"><span data-stu-id="eacae-155">String</span></span>|<span data-ttu-id="eacae-156">O nome de exibição do recurso para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="eacae-156">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="eacae-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="eacae-157">resourceId</span></span>|<span data-ttu-id="eacae-158">Guid</span><span class="sxs-lookup"><span data-stu-id="eacae-158">Guid</span></span>|<span data-ttu-id="eacae-159">O identificador exclusivo (**objectId**) para o recurso de destino (entidade de serviço) para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="eacae-159">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="eacae-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="eacae-160">Response</span></span>

<span data-ttu-id="eacae-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eacae-161">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eacae-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eacae-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eacae-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eacae-163">Request</span></span>
<span data-ttu-id="eacae-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eacae-164">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_approleassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/appRoleAssignments/{id}
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="eacae-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="eacae-165">Response</span></span>
<span data-ttu-id="eacae-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eacae-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->