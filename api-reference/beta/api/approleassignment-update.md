---
title: Atualizar approleassignment
description: Atualize as propriedades do objeto approleassignment.
localization_priority: Normal
ms.openlocfilehash: 89147651b1a3ea182247cf3620efba9464c4b055
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572910"
---
# <a name="update-approleassignment"></a><span data-ttu-id="37270-103">Atualizar approleassignment</span><span class="sxs-lookup"><span data-stu-id="37270-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37270-104">Atualize as propriedades do objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="37270-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="37270-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="37270-105">Permissions</span></span>
<span data-ttu-id="37270-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37270-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37270-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37270-108">Permission type</span></span>      | <span data-ttu-id="37270-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37270-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37270-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37270-110">Delegated (work or school account)</span></span> | <span data-ttu-id="37270-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="37270-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="37270-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37270-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37270-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37270-113">Not supported.</span></span>    |
|<span data-ttu-id="37270-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37270-114">Application</span></span> | <span data-ttu-id="37270-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37270-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="37270-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37270-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="37270-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37270-117">Request headers</span></span>
| <span data-ttu-id="37270-118">Nome</span><span class="sxs-lookup"><span data-stu-id="37270-118">Name</span></span>       | <span data-ttu-id="37270-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="37270-119">Type</span></span> | <span data-ttu-id="37270-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="37270-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="37270-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="37270-121">Authorization</span></span>  | <span data-ttu-id="37270-122">string</span><span class="sxs-lookup"><span data-stu-id="37270-122">string</span></span>  | <span data-ttu-id="37270-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37270-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37270-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37270-125">Request body</span></span>
<span data-ttu-id="37270-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="37270-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="37270-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37270-129">Property</span></span>     | <span data-ttu-id="37270-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="37270-130">Type</span></span>   |<span data-ttu-id="37270-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="37270-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37270-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="37270-132">creationTimestamp</span></span>|<span data-ttu-id="37270-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37270-133">DateTimeOffset</span></span>|<span data-ttu-id="37270-134">A hora em que a concessão foi criada.</span><span class="sxs-lookup"><span data-stu-id="37270-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="37270-135">id</span><span class="sxs-lookup"><span data-stu-id="37270-135">id</span></span>|<span data-ttu-id="37270-136">Guid</span><span class="sxs-lookup"><span data-stu-id="37270-136">Guid</span></span>|<span data-ttu-id="37270-137">A id de função que foi atribuída à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="37270-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="37270-138">Essa função deve ser declarada pelo destino recurso aplicativo **resourceId** em sua propriedade **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="37270-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="37270-139">Onde o recurso não declarar todas as permissões, uma id do padrão (zero GUID) deve ser especificada.</span><span class="sxs-lookup"><span data-stu-id="37270-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="37270-140">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="37270-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="37270-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="37270-141">principalDisplayName</span></span>|<span data-ttu-id="37270-142">String</span><span class="sxs-lookup"><span data-stu-id="37270-142">String</span></span>|<span data-ttu-id="37270-143">O nome de exibição da entidade que foi concedido o acesso.</span><span class="sxs-lookup"><span data-stu-id="37270-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="37270-144">principalId</span><span class="sxs-lookup"><span data-stu-id="37270-144">principalId</span></span>|<span data-ttu-id="37270-145">Guid</span><span class="sxs-lookup"><span data-stu-id="37270-145">Guid</span></span>|<span data-ttu-id="37270-146">O identificador exclusivo (**objectId**) para a entidade sendo concedida o acesso.</span><span class="sxs-lookup"><span data-stu-id="37270-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="37270-147">**Observações**: necessários.</span><span class="sxs-lookup"><span data-stu-id="37270-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="37270-148">principalType</span><span class="sxs-lookup"><span data-stu-id="37270-148">principalType</span></span>|<span data-ttu-id="37270-149">String</span><span class="sxs-lookup"><span data-stu-id="37270-149">String</span></span>|<span data-ttu-id="37270-150">O tipo de entidade.</span><span class="sxs-lookup"><span data-stu-id="37270-150">The type of principal.</span></span>  <span data-ttu-id="37270-151">Isso pode ser "User", "Grupo" ou "ServicePrincipal".</span><span class="sxs-lookup"><span data-stu-id="37270-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="37270-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="37270-152">resourceDisplayName</span></span>|<span data-ttu-id="37270-153">String</span><span class="sxs-lookup"><span data-stu-id="37270-153">String</span></span>|<span data-ttu-id="37270-154">O nome de exibição do recurso para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="37270-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="37270-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="37270-155">resourceId</span></span>|<span data-ttu-id="37270-156">Guid</span><span class="sxs-lookup"><span data-stu-id="37270-156">Guid</span></span>|<span data-ttu-id="37270-157">O identificador exclusivo (**objectId**) para o recurso de destino (entidade de serviço) para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="37270-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="37270-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="37270-158">Response</span></span>

<span data-ttu-id="37270-159">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37270-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="37270-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37270-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="37270-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37270-161">Request</span></span>
<span data-ttu-id="37270-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="37270-162">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="37270-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="37270-163">Response</span></span>
<span data-ttu-id="37270-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="37270-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
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
<!--
{
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
