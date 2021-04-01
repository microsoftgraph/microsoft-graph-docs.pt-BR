---
title: Conceder um appRoleAssignment a um grupo
description: Conceder uma atribuição de função de aplicativo a um grupo.
localization_priority: Priority
doc_type: apiPageType
ms.prod: groups
author: psignoret
ms.openlocfilehash: d574b638d190b1d63cc7fd859160d6ae144c9aab
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469007"
---
# <a name="grant-an-approleassignment-to-a-group"></a><span data-ttu-id="e59b7-103">Conceder um appRoleAssignment a um grupo</span><span class="sxs-lookup"><span data-stu-id="e59b7-103">Grant an appRoleAssignment to a group</span></span>

<span data-ttu-id="e59b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e59b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e59b7-105">Use esta API para atribuir uma função de aplicativo a um grupo.</span><span class="sxs-lookup"><span data-stu-id="e59b7-105">Use this API to assign an app role to a group.</span></span> <span data-ttu-id="e59b7-106">Todos os membros diretos do grupo serão considerados atribuídos.</span><span class="sxs-lookup"><span data-stu-id="e59b7-106">All direct members of the group will be considered assigned.</span></span> <span data-ttu-id="e59b7-107">Para conceder uma atribuição de função de aplicativo a um grupo, você precisa de três identificadores:</span><span class="sxs-lookup"><span data-stu-id="e59b7-107">To grant an app role assignment to a group, you need three identifiers:</span></span>

- <span data-ttu-id="e59b7-108">`principalId`: A `id` do grupo ao qual você está atribuindo a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e59b7-108">`principalId`: The `id` of the group to which you are assigning the app role.</span></span>
- <span data-ttu-id="e59b7-109">`resourceId`: A `id` do recurso `servicePrincipal` que definiu a função do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e59b7-109">`resourceId`: The `id` of the resource `servicePrincipal` which has defined the app role.</span></span>
- <span data-ttu-id="e59b7-110">`appRoleId`: A `id` do `appRole` (definido na entidade de serviço do recurso) para atribuir ao grupo.</span><span class="sxs-lookup"><span data-stu-id="e59b7-110">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the group.</span></span>

<span data-ttu-id="e59b7-111">Licenças adicionais podem ser necessárias para [usar um grupo para gerenciar o acesso aos aplicativos](/azure/active-directory/users-groups-roles/groups-saasapps).</span><span class="sxs-lookup"><span data-stu-id="e59b7-111">Additional licenses might be required to [use a group to manage access to applications](/azure/active-directory/users-groups-roles/groups-saasapps).</span></span>

## <a name="permissions"></a><span data-ttu-id="e59b7-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="e59b7-112">Permissions</span></span>

<span data-ttu-id="e59b7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e59b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e59b7-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e59b7-115">Permission type</span></span>      | <span data-ttu-id="e59b7-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e59b7-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e59b7-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e59b7-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e59b7-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e59b7-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e59b7-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e59b7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e59b7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e59b7-120">Not supported.</span></span>    |
|<span data-ttu-id="e59b7-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e59b7-121">Application</span></span> | <span data-ttu-id="e59b7-122">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e59b7-122">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e59b7-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e59b7-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="e59b7-124">Como prática recomendada, recomendamos que você crie atribuições de função de aplicativo por meio da `appRoleAssignedTo`relação do _recurso_ da entidade de serviço, em vez da `appRoleAssignments`relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="e59b7-124">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e59b7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e59b7-125">Request headers</span></span>

| <span data-ttu-id="e59b7-126">Nome</span><span class="sxs-lookup"><span data-stu-id="e59b7-126">Name</span></span>       | <span data-ttu-id="e59b7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e59b7-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e59b7-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="e59b7-128">Authorization</span></span> | <span data-ttu-id="e59b7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e59b7-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e59b7-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="e59b7-131">Content-type</span></span> | <span data-ttu-id="e59b7-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e59b7-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e59b7-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e59b7-134">Request body</span></span>

<span data-ttu-id="e59b7-135">No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e59b7-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e59b7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e59b7-136">Response</span></span>

<span data-ttu-id="e59b7-137">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e59b7-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e59b7-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e59b7-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e59b7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e59b7-139">Request</span></span>

<span data-ttu-id="e59b7-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e59b7-140">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e59b7-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e59b7-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/7679d9a4-2323-44cd-b5c2-673ec88d8b12/appRoleAssignments
Content-Type: application/json

{
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055",
  "appRoleId": "00000000-0000-0000-0000-000000000000"
}
```
# <a name="c"></a>[<span data-ttu-id="e59b7-142">C#</span><span class="sxs-lookup"><span data-stu-id="e59b7-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-create-approleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e59b7-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e59b7-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-create-approleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e59b7-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e59b7-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-create-approleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e59b7-145">Java</span><span class="sxs-lookup"><span data-stu-id="e59b7-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-create-approleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="e59b7-146">Neste exemplo, `{id}` e `{principalId-value}` seriam os `id` do grupo atribuído.</span><span class="sxs-lookup"><span data-stu-id="e59b7-146">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned group.</span></span>

### <a name="response"></a><span data-ttu-id="e59b7-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="e59b7-147">Response</span></span>

<span data-ttu-id="e59b7-148">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e59b7-148">Here is an example of the response.</span></span> 

><span data-ttu-id="e59b7-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e59b7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('7679d9a4-2323-44cd-b5c2-673ec88d8b12')/appRoleAssignments/$entity",
  "id": "pNl5diMjzUS1wmc-yI2LEkGgWqFFrFdLhG2Ly2CysL4",
  "deletedDateTime": null,
  "appRoleId": "00000000-0000-0000-0000-000000000000",
  "createdDateTime": "2021-02-19T17:55:08.3369542Z",
  "principalDisplayName": "Young techmakers",
  "principalId": "7679d9a4-2323-44cd-b5c2-673ec88d8b12",
  "principalType": "Group",
  "resourceDisplayName": "Yammer",
  "resourceId": "076e8b57-bac8-49d7-9396-e3449b685055"
}
```

<span data-ttu-id="e59b7-151">Neste exemplo, observe que o valor usado como a **id** do usuário na URL de solicitação (`cde330e5-2150-4c11-9c5b-14bfdc948c79`) é o mesmo que a propriedade **principalId** no corpo.</span><span class="sxs-lookup"><span data-stu-id="e59b7-151">In this example, note that the value used as the user **id** in the request URL (`cde330e5-2150-4c11-9c5b-14bfdc948c79`) is the same as the **principalId** property in the body.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
