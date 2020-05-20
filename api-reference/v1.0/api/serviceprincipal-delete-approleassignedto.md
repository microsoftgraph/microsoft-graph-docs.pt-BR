---
title: Excluir um appRoleAssignment concedido para uma entidade de serviço
description: Excluir um appRoleAssignment concedido para uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 7260cba9886f4366d821ae7e4ad67a8b612bc902
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290101"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="bbb8e-103">Excluir um appRoleAssignment concedido para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="bbb8e-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="bbb8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbb8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bbb8e-105">Exclui um [appRoleAssignment](../resources/approleassignment.md) que um usuário, grupo ou entidade de serviço de cliente foi concedido para uma entidade de serviço de recurso.</span><span class="sxs-lookup"><span data-stu-id="bbb8e-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbb8e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbb8e-106">Permissions</span></span>

<span data-ttu-id="bbb8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbb8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbb8e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbb8e-109">Permission type</span></span>      | <span data-ttu-id="bbb8e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbb8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbb8e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbb8e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bbb8e-112">AppRoleAssignment. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="bbb8e-112">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bbb8e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbb8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbb8e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbb8e-114">Not supported.</span></span>    |
|<span data-ttu-id="bbb8e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbb8e-115">Application</span></span> | <span data-ttu-id="bbb8e-116">AppRoleAssignment. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bbb8e-116">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbb8e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbb8e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}
```

> [!NOTE]
> <span data-ttu-id="bbb8e-118">Como prática recomendada, recomendamos a exclusão de atribuições de função de aplicativo através da `appRoleAssignedTo` relação da entidade de serviço de _recurso_ , em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="bbb8e-118">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bbb8e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb8e-119">Request headers</span></span>

| <span data-ttu-id="bbb8e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bbb8e-120">Name</span></span>       | <span data-ttu-id="bbb8e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbb8e-121">Type</span></span> | <span data-ttu-id="bbb8e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbb8e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bbb8e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbb8e-123">Authorization</span></span>  | <span data-ttu-id="bbb8e-124">string</span><span class="sxs-lookup"><span data-stu-id="bbb8e-124">string</span></span>  | <span data-ttu-id="bbb8e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbb8e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbb8e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb8e-127">Request body</span></span>

<span data-ttu-id="bbb8e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bbb8e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbb8e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbb8e-129">Response</span></span>

<span data-ttu-id="bbb8e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbb8e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bbb8e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bbb8e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bbb8e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbb8e-133">Request</span></span>

<span data-ttu-id="bbb8e-134">Veja a seguir um exemplo da solicitação para excluir uma atribuição de função de aplicativo da entidade de serviço de recurso.</span><span class="sxs-lookup"><span data-stu-id="bbb8e-134">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignedTo/{id}
```

### <a name="response"></a><span data-ttu-id="bbb8e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbb8e-135">Response</span></span>

<span data-ttu-id="bbb8e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bbb8e-136">The following is an example of the response.</span></span>

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
