---
title: Excluir um appRoleAssignment concedido a um usuário
description: Excluir um appRoleAssignment que tenha sido concedido a um usuário.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 447d635a6822fb62d9be128b46c357ac6efa06df
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290065"
---
# <a name="delete-an-approleassignment-granted-to-a-user"></a><span data-ttu-id="71dcc-103">Excluir um appRoleAssignment concedido a um usuário</span><span class="sxs-lookup"><span data-stu-id="71dcc-103">Delete an appRoleAssignment granted to a user</span></span>

<span data-ttu-id="71dcc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71dcc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71dcc-105">Excluir um [appRoleAssignment](../resources/approleassignment.md) que tenha sido concedido a um usuário.</span><span class="sxs-lookup"><span data-stu-id="71dcc-105">Delete an [appRoleAssignment](../resources/approleassignment.md) that has been granted to a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="71dcc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="71dcc-106">Permissions</span></span>

<span data-ttu-id="71dcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71dcc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71dcc-109">Permission type</span></span>      | <span data-ttu-id="71dcc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71dcc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71dcc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71dcc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="71dcc-112">AppRoleAssignment. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="71dcc-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71dcc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71dcc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71dcc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71dcc-114">Not supported.</span></span>    |
|<span data-ttu-id="71dcc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71dcc-115">Application</span></span> | <span data-ttu-id="71dcc-116">AppRoleAssignment. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="71dcc-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71dcc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71dcc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /users/{id}/appRoleAssignments/{id}
```

> [!NOTE]
> <span data-ttu-id="71dcc-118">Como prática recomendada, recomendamos a exclusão de atribuições de função de aplicativo através da `appRoleAssignedTo` relação da entidade de serviço de _recurso_ , em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="71dcc-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71dcc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71dcc-119">Request headers</span></span>

| <span data-ttu-id="71dcc-120">Nome</span><span class="sxs-lookup"><span data-stu-id="71dcc-120">Name</span></span>       | <span data-ttu-id="71dcc-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="71dcc-121">Type</span></span> | <span data-ttu-id="71dcc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="71dcc-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71dcc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71dcc-123">Authorization</span></span>  | <span data-ttu-id="71dcc-124">string</span><span class="sxs-lookup"><span data-stu-id="71dcc-124">string</span></span>  | <span data-ttu-id="71dcc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71dcc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71dcc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71dcc-127">Request body</span></span>

<span data-ttu-id="71dcc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71dcc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71dcc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="71dcc-129">Response</span></span>

<span data-ttu-id="71dcc-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71dcc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71dcc-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="71dcc-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71dcc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71dcc-133">Request</span></span>

<span data-ttu-id="71dcc-134">Veja a seguir um exemplo da solicitação para excluir uma atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="71dcc-134">Here is an example of the request to delete an app role assignment.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/{id}/appRoleAssignments/{id}
```

### <a name="response"></a><span data-ttu-id="71dcc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="71dcc-135">Response</span></span>

<span data-ttu-id="71dcc-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71dcc-136">Here is an example of the response.</span></span>

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
