---
title: Conceder um appRoleAssignment a um grupo
description: Conceder uma atribuição de função de aplicativo a um grupo.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 831d141bbd7515ff23992b6ea56043a6472b16dd
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289592"
---
# <a name="grant-an-approleassignment-to-a-group"></a><span data-ttu-id="15140-103">Conceder um appRoleAssignment a um grupo</span><span class="sxs-lookup"><span data-stu-id="15140-103">Grant an appRoleAssignment to a group</span></span>

<span data-ttu-id="15140-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15140-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15140-105">Use essa API para atribuir uma função de aplicativo a um grupo.</span><span class="sxs-lookup"><span data-stu-id="15140-105">Use this API to assign an app role to a group.</span></span> <span data-ttu-id="15140-106">Todos os membros diretos do grupo serão considerados atribuídos.</span><span class="sxs-lookup"><span data-stu-id="15140-106">All direct members of the group will be considered assigned.</span></span> <span data-ttu-id="15140-107">Para conceder a um grupo uma atribuição de função de aplicativo, você precisa de três identificadores:</span><span class="sxs-lookup"><span data-stu-id="15140-107">To grant an app role assignment to a group, you need three identifiers:</span></span>

- <span data-ttu-id="15140-108">`principalId`: O `id` do grupo ao qual você está atribuindo a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15140-108">`principalId`: The `id` of the group to which you are assigning the app role.</span></span>
- <span data-ttu-id="15140-109">`resourceId`: O `id` do recurso `servicePrincipal` que definiu a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="15140-109">`resourceId`: The `id` of the resource `servicePrincipal` which has defined the app role.</span></span>
- <span data-ttu-id="15140-110">`appRoleId`: O `id` `appRole` (definido na entidade de segurança do serviço de recursos) a ser atribuído ao grupo.</span><span class="sxs-lookup"><span data-stu-id="15140-110">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the group.</span></span>

<span data-ttu-id="15140-111">Licenças adicionais podem ser necessárias para [usar um grupo para gerenciar o acesso a aplicativos](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-saasapps).</span><span class="sxs-lookup"><span data-stu-id="15140-111">Additional licenses might be required to [use a group to manage access to applications](https://docs.microsoft.com/azure/active-directory/users-groups-roles/groups-saasapps).</span></span>

## <a name="permissions"></a><span data-ttu-id="15140-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="15140-112">Permissions</span></span>

<span data-ttu-id="15140-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15140-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15140-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="15140-115">Permission type</span></span>      | <span data-ttu-id="15140-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="15140-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15140-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="15140-117">Delegated (work or school account)</span></span> | <span data-ttu-id="15140-118">AppRoleAssignment. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="15140-118">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="15140-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="15140-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15140-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="15140-120">Not supported.</span></span>    |
|<span data-ttu-id="15140-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15140-121">Application</span></span> | <span data-ttu-id="15140-122">AppRoleAssignment. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="15140-122">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15140-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="15140-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="15140-124">Como prática recomendada, recomendamos a criação de atribuições de função de aplicativo através da `appRoleAssignedTo` relação da entidade de serviço de _recurso_ , em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="15140-124">As a best practice, we recommend creating app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15140-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="15140-125">Request headers</span></span>

| <span data-ttu-id="15140-126">Nome</span><span class="sxs-lookup"><span data-stu-id="15140-126">Name</span></span>       | <span data-ttu-id="15140-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="15140-127">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="15140-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="15140-128">Authorization</span></span> | <span data-ttu-id="15140-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15140-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="15140-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="15140-131">Content-type</span></span> | <span data-ttu-id="15140-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="15140-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15140-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="15140-134">Request body</span></span>

<span data-ttu-id="15140-135">No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="15140-135">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="15140-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="15140-136">Response</span></span>

<span data-ttu-id="15140-137">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15140-137">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15140-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="15140-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15140-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="15140-139">Request</span></span>

<span data-ttu-id="15140-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="15140-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```

<span data-ttu-id="15140-141">Neste exemplo, `{id}` e `{principalId-value}` seria o `id` do grupo atribuído.</span><span class="sxs-lookup"><span data-stu-id="15140-141">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned group.</span></span>

### <a name="response"></a><span data-ttu-id="15140-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="15140-142">Response</span></span>

<span data-ttu-id="15140-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="15140-143">Here is an example of the response.</span></span> 

><span data-ttu-id="15140-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="15140-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "id": "id-value",
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalType": "principalType-value",
  "principalId": "principalId-value",
  "principalDisplayName": "principalDisplayName-value",
  "resourceId": "resourceId-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

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
