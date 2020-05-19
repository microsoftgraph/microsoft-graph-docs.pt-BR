---
title: Conceder um appRoleAssignment a uma entidade de serviço
description: Conceda uma atribuição de função de aplicativo a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 6ecfbd4f85fb1c991a9097688daa40634a630c3a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290023"
---
# <a name="grant-an-approleassignment-for-a-service-principal"></a><span data-ttu-id="171af-103">Conceder um appRoleAssignment para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="171af-103">Grant an appRoleAssignment for a service principal</span></span>

<span data-ttu-id="171af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="171af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="171af-105">Atribuir uma função de aplicativo para uma entidade de serviço de recurso, a um usuário, grupo ou entidade de serviço de cliente.</span><span class="sxs-lookup"><span data-stu-id="171af-105">Assign an app role for a resource service principal, to a user, group, or client service principal.</span></span>

<span data-ttu-id="171af-106">As funções de aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="171af-106">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="171af-107">As permissões de aplicativo podem ser concedidas diretamente com as atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="171af-107">Application permissions can be granted directly with app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

<span data-ttu-id="171af-108">Para conceder uma atribuição de função de aplicativo, você precisa de três identificadores:</span><span class="sxs-lookup"><span data-stu-id="171af-108">To grant an app role assignment, you need three identifiers:</span></span>

- <span data-ttu-id="171af-109">`principalId`: O `id` do **usuário**, **grupo** ou **userdirigente** do cliente ao qual você está atribuindo a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="171af-109">`principalId`: The `id` of the **user**, **group** or client **servicePrincipal** to which you are assigning the app role.</span></span>
- <span data-ttu-id="171af-110">`resourceId`: O `id` do Resource **servicePrincipalName** que definiu a função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="171af-110">`resourceId`: The `id` of the resource **servicePrincipal** which has defined the app role.</span></span>
- <span data-ttu-id="171af-111">`appRoleId`: O `id` do **appRole** (definido na entidade de segurança do serviço de recurso) a ser atribuído a um usuário, grupo ou entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="171af-111">`appRoleId`: The `id` of the **appRole** (defined on the resource service principal) to assign to a user, group, or service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="171af-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="171af-112">Permissions</span></span>

<span data-ttu-id="171af-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="171af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="171af-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="171af-115">Permission type</span></span>      | <span data-ttu-id="171af-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="171af-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="171af-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="171af-117">Delegated (work or school account)</span></span> | <span data-ttu-id="171af-118">AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="171af-118">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="171af-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="171af-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="171af-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="171af-120">Not supported.</span></span>    |
|<span data-ttu-id="171af-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="171af-121">Application</span></span> | <span data-ttu-id="171af-122">AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="171af-122">AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="171af-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="171af-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="request-headers"></a><span data-ttu-id="171af-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="171af-124">Request headers</span></span>

| <span data-ttu-id="171af-125">Nome</span><span class="sxs-lookup"><span data-stu-id="171af-125">Name</span></span>       | <span data-ttu-id="171af-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="171af-126">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="171af-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="171af-127">Authorization</span></span> | <span data-ttu-id="171af-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="171af-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="171af-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="171af-130">Content-type</span></span> | <span data-ttu-id="171af-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="171af-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="171af-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="171af-133">Request body</span></span>

<span data-ttu-id="171af-134">No corpo da solicitação, forneça uma representação JSON de um objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="171af-134">In the request body, supply a JSON representation of an [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="171af-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="171af-135">Response</span></span>

<span data-ttu-id="171af-136">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="171af-136">If successful, this method returns a `201 Created` response code and an [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="171af-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="171af-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="171af-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="171af-138">Request</span></span>

<span data-ttu-id="171af-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="171af-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_create_approleassignedto"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo
Content-Type: application/json
Content-Length: 110

{
  "principalId": "principalId-value",
  "resourceId": "resourceId-value",
  "appRoleId": "appRoleId-value"
}
```

<span data-ttu-id="171af-140">Neste exemplo, `{id}` e `{resourceId-value}` seria o `id` da entidade de serviço de recurso e `{principalId}` seria o `id` usuário, grupo ou entidade de serviço de cliente atribuído.</span><span class="sxs-lookup"><span data-stu-id="171af-140">In this example, `{id}` and `{resourceId-value}` would both be the `id` of the resource service principal, and `{principalId}` would be the `id` of the assigned user, group, or client service principal.</span></span>

### <a name="response"></a><span data-ttu-id="171af-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="171af-141">Response</span></span>

<span data-ttu-id="171af-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="171af-142">Here is an example of the response.</span></span> 

> <span data-ttu-id="171af-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="171af-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
