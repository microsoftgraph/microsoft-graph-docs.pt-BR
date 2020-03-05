---
title: Atualizar approleassignment
description: Atualize as propriedades do objeto approleassignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4f1f499cb54ac135f5393e795e24cea6c7962685
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441358"
---
# <a name="update-approleassignment"></a><span data-ttu-id="bb0c4-103">Atualizar approleassignment</span><span class="sxs-lookup"><span data-stu-id="bb0c4-103">Update approleassignment</span></span>

<span data-ttu-id="bb0c4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bb0c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb0c4-105">Atualize as propriedades do objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-105">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb0c4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bb0c4-106">Permissions</span></span>
<span data-ttu-id="bb0c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb0c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb0c4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bb0c4-109">Permission type</span></span>      | <span data-ttu-id="bb0c4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bb0c4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb0c4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bb0c4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb0c4-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb0c4-112">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="bb0c4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bb0c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb0c4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-114">Not supported.</span></span>    |
|<span data-ttu-id="bb0c4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bb0c4-115">Application</span></span> | <span data-ttu-id="bb0c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb0c4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bb0c4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bb0c4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bb0c4-118">Request headers</span></span>
| <span data-ttu-id="bb0c4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bb0c4-119">Name</span></span>       | <span data-ttu-id="bb0c4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb0c4-120">Type</span></span> | <span data-ttu-id="bb0c4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb0c4-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bb0c4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bb0c4-122">Authorization</span></span>  | <span data-ttu-id="bb0c4-123">string</span><span class="sxs-lookup"><span data-stu-id="bb0c4-123">string</span></span>  | <span data-ttu-id="bb0c4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb0c4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bb0c4-126">Request body</span></span>
<span data-ttu-id="bb0c4-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bb0c4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bb0c4-130">Property</span></span>     | <span data-ttu-id="bb0c4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bb0c4-131">Type</span></span>   |<span data-ttu-id="bb0c4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bb0c4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb0c4-133">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="bb0c4-133">creationTimestamp</span></span>|<span data-ttu-id="bb0c4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb0c4-134">DateTimeOffset</span></span>|<span data-ttu-id="bb0c4-135">A hora em que a concessão foi criada.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-135">The time when the grant was created.</span></span>|
|<span data-ttu-id="bb0c4-136">id</span><span class="sxs-lookup"><span data-stu-id="bb0c4-136">id</span></span>|<span data-ttu-id="bb0c4-137">Guid</span><span class="sxs-lookup"><span data-stu-id="bb0c4-137">Guid</span></span>|<span data-ttu-id="bb0c4-138">A ID de função que foi atribuída à entidade.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-138">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="bb0c4-139">Essa função deve ser declarada pela **resourceId** do aplicativo do recurso de destino em sua propriedade **appRoles**.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-139">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="bb0c4-140">Quando o recurso não declarar nenhuma permissão, uma ID padrão (zero GUID) deve ser especificada.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-140">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="bb0c4-141">**Anotações**: não anulável.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-141">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="bb0c4-142">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb0c4-142">principalDisplayName</span></span>|<span data-ttu-id="bb0c4-143">String</span><span class="sxs-lookup"><span data-stu-id="bb0c4-143">String</span></span>|<span data-ttu-id="bb0c4-144">O nome de exibição da entidade à qual foi concedido o acesso.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-144">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="bb0c4-145">principalId</span><span class="sxs-lookup"><span data-stu-id="bb0c4-145">principalId</span></span>|<span data-ttu-id="bb0c4-146">Guid</span><span class="sxs-lookup"><span data-stu-id="bb0c4-146">Guid</span></span>|<span data-ttu-id="bb0c4-147">O identificador exclusivo (**ObjectID**) da entidade de segurança que recebeu o acesso.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-147">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="bb0c4-148">**Observações**: obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-148">**Notes**: required.</span></span>            |
|<span data-ttu-id="bb0c4-149">principalType</span><span class="sxs-lookup"><span data-stu-id="bb0c4-149">principalType</span></span>|<span data-ttu-id="bb0c4-150">String</span><span class="sxs-lookup"><span data-stu-id="bb0c4-150">String</span></span>|<span data-ttu-id="bb0c4-151">O tipo de entidade.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-151">The type of principal.</span></span>  <span data-ttu-id="bb0c4-152">Pode ser “User”, “Group” ou “ServicePrincipal”.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-152">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="bb0c4-153">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb0c4-153">resourceDisplayName</span></span>|<span data-ttu-id="bb0c4-154">String</span><span class="sxs-lookup"><span data-stu-id="bb0c4-154">String</span></span>|<span data-ttu-id="bb0c4-155">O nome de exibição do recurso para o qual a tarefa foi feita.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-155">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="bb0c4-156">resourceId</span><span class="sxs-lookup"><span data-stu-id="bb0c4-156">resourceId</span></span>|<span data-ttu-id="bb0c4-157">Guid</span><span class="sxs-lookup"><span data-stu-id="bb0c4-157">Guid</span></span>|<span data-ttu-id="bb0c4-158">O identificador exclusivo (**ObjectID**) do recurso de destino (entidade de serviço) para o qual a atribuição foi feita.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-158">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="bb0c4-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb0c4-159">Response</span></span>

<span data-ttu-id="bb0c4-160">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [appRoleAssignment](../resources/approleassignment.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-160">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb0c4-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bb0c4-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb0c4-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bb0c4-162">Request</span></span>
<span data-ttu-id="bb0c4-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-163">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bb0c4-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb0c4-164">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="bb0c4-165">C#</span><span class="sxs-lookup"><span data-stu-id="bb0c4-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb0c4-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb0c4-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb0c4-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb0c4-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bb0c4-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="bb0c4-168">Response</span></span>
<span data-ttu-id="bb0c4-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bb0c4-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
