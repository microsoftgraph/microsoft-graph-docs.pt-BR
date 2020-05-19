---
title: Conceder um appRoleAssignment a uma entidade de serviço
description: Conceda uma atribuição de função de aplicativo a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 557c7673f299cb37a90bf20357e093b80ca3a264
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290016"
---
# <a name="grant-an-approleassignment-to-a-service-principal"></a><span data-ttu-id="a4c83-103">Conceder um appRoleAssignment a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="a4c83-103">Grant an appRoleAssignment to a service principal</span></span>

<span data-ttu-id="a4c83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4c83-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4c83-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4c83-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4c83-106">Atribuir uma função de aplicativo a uma entidade de serviço de cliente.</span><span class="sxs-lookup"><span data-stu-id="a4c83-106">Assign an app role to a client service principal.</span></span>

<span data-ttu-id="a4c83-107">As funções de aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="a4c83-107">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="a4c83-108">As permissões de aplicativo podem ser concedidas diretamente com as atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="a4c83-108">Application permissions can be granted directly with app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="a4c83-109">Para conceder a uma atribuição de função de aplicativo a uma entidade de serviço de cliente, você precisa de três identificadores:</span><span class="sxs-lookup"><span data-stu-id="a4c83-109">To grant an app role assignment to a client service principal, you need three identifiers:</span></span>

- <span data-ttu-id="a4c83-110">`principalId`: O `id` da entidade de serviço do cliente para a qual você está atribuindo a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a4c83-110">`principalId`: The `id` of the client service principal to which you are assigning the app role.</span></span>
- <span data-ttu-id="a4c83-111">`resourceId`: O `id` do recurso `servicePrincipal` (a API) que definiu a função de aplicativo (a permissão de aplicativo).</span><span class="sxs-lookup"><span data-stu-id="a4c83-111">`resourceId`: The `id` of the resource `servicePrincipal` (the API) which has defined the app role (the application permission).</span></span>
- <span data-ttu-id="a4c83-112">`appRoleId`: O `id` `appRole` (definido na entidade de segurança do serviço de recurso) a ser atribuído à entidade de serviço do cliente.</span><span class="sxs-lookup"><span data-stu-id="a4c83-112">`appRoleId`: The `id` of the `appRole` (defined on the resource service principal) to assign to the client service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4c83-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4c83-113">Permissions</span></span>

<span data-ttu-id="a4c83-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4c83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4c83-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4c83-116">Permission type</span></span>      | <span data-ttu-id="a4c83-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4c83-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4c83-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4c83-118">Delegated (work or school account)</span></span> | <span data-ttu-id="a4c83-119">AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="a4c83-119">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4c83-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4c83-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4c83-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4c83-121">Not supported.</span></span>    |
|<span data-ttu-id="a4c83-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4c83-122">Application</span></span> | <span data-ttu-id="a4c83-123">AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a4c83-123">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4c83-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4c83-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments
```

> [!NOTE]
> <span data-ttu-id="a4c83-125">Como prática recomendada, recomendamos a criação de atribuições de função de aplicativo através da [ `appRoleAssignedTo` relação da entidade de serviço de _recurso_ ](serviceprincipal-post-approleassignedto.md), em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="a4c83-125">As a best practice, we recommend creating app role assignments through the [`appRoleAssignedTo` relationship of the _resource_ service principal](serviceprincipal-post-approleassignedto.md), instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4c83-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c83-126">Request headers</span></span>

| <span data-ttu-id="a4c83-127">Nome</span><span class="sxs-lookup"><span data-stu-id="a4c83-127">Name</span></span>       | <span data-ttu-id="a4c83-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4c83-128">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="a4c83-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4c83-129">Authorization</span></span> | <span data-ttu-id="a4c83-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4c83-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a4c83-132">Content-type</span><span class="sxs-lookup"><span data-stu-id="a4c83-132">Content-type</span></span> | <span data-ttu-id="a4c83-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4c83-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4c83-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c83-135">Request body</span></span>

<span data-ttu-id="a4c83-136">No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a4c83-136">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a4c83-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c83-137">Response</span></span>

<span data-ttu-id="a4c83-138">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c83-138">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4c83-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a4c83-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4c83-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4c83-140">Request</span></span>

<span data-ttu-id="a4c83-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4c83-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_create_approleassignment"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```

<span data-ttu-id="a4c83-142">Neste exemplo, `{id}` e `{principalId-value}` seria o `id` da entidade de serviço de cliente atribuída, e `{resoruceId}` seria o `id` da entidade de serviço de recurso (a API).</span><span class="sxs-lookup"><span data-stu-id="a4c83-142">In this example, `{id}` and `{principalId-value}` would both be the `id` of the assigned client service principal, and `{resoruceId}` would be the `id` of the resource service principal (the API).</span></span>

### <a name="response"></a><span data-ttu-id="a4c83-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4c83-143">Response</span></span>

<span data-ttu-id="a4c83-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4c83-144">Here is an example of the response.</span></span> 

> <span data-ttu-id="a4c83-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4c83-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
