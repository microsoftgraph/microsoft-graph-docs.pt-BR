---
title: Excluir um appRoleAssignment de uma entidade de serviço
description: Excluir um appRoleAssignment de uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: b81921d9ede08d247810faa5aa4c9e4d3aab3d15
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291171"
---
# <a name="delete-an-approleassignment-granted-to-a-service-principal"></a><span data-ttu-id="13bd1-103">Excluir um appRoleAssignment concedido a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="13bd1-103">Delete an appRoleAssignment granted to a service principal</span></span>

<span data-ttu-id="13bd1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13bd1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="13bd1-105">Exclui um [appRoleAssignment](../resources/approleassignment.md) que recebeu uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="13bd1-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a service principal has been granted.</span></span>

<span data-ttu-id="13bd1-106">As funções de aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="13bd1-106">App roles which are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="13bd1-107">A exclusão de uma atribuição de função de aplicativo para uma entidade de serviço é equivalente a revogar a concessão de permissão somente de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13bd1-107">Deleting an app role assignment for a service principal is equivalent to revoking the app-only permission grant.</span></span>

## <a name="permissions"></a><span data-ttu-id="13bd1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="13bd1-108">Permissions</span></span>

<span data-ttu-id="13bd1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13bd1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13bd1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13bd1-111">Permission type</span></span>      | <span data-ttu-id="13bd1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13bd1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13bd1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13bd1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="13bd1-114">AppRoleAssignment. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="13bd1-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="13bd1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13bd1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13bd1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13bd1-116">Not supported.</span></span>    |
|<span data-ttu-id="13bd1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13bd1-117">Application</span></span> | <span data-ttu-id="13bd1-118">AppRoleAssignment. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="13bd1-118">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13bd1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13bd1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="13bd1-120">Como prática recomendada, recomendamos a exclusão de atribuições de função de aplicativo através da `appRoleAssignedTo` relação da entidade de serviço de _recurso_ , em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="13bd1-120">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13bd1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13bd1-121">Request headers</span></span>

| <span data-ttu-id="13bd1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="13bd1-122">Name</span></span>       | <span data-ttu-id="13bd1-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="13bd1-123">Type</span></span> | <span data-ttu-id="13bd1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="13bd1-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="13bd1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="13bd1-125">Authorization</span></span>  | <span data-ttu-id="13bd1-126">string</span><span class="sxs-lookup"><span data-stu-id="13bd1-126">string</span></span>  | <span data-ttu-id="13bd1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="13bd1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="13bd1-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13bd1-129">Request body</span></span>

<span data-ttu-id="13bd1-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13bd1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13bd1-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="13bd1-131">Response</span></span>

<span data-ttu-id="13bd1-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13bd1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13bd1-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13bd1-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13bd1-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13bd1-135">Request</span></span>

<span data-ttu-id="13bd1-136">Veja a seguir um exemplo da solicitação para excluir uma atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="13bd1-136">Here is an example of the request to delete an app role assignment.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignments/{id}
```

### <a name="response"></a><span data-ttu-id="13bd1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="13bd1-137">Response</span></span>

<span data-ttu-id="13bd1-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13bd1-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
