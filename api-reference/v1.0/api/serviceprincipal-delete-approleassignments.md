---
title: Excluir um appRoleAssignment de uma entidade de serviço
description: Exclua um appRoleAssignment de uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: b60bd4dbd64493a54e41bef86b7c311e37a30117
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703626"
---
# <a name="delete-an-approleassignment-granted-to-a-service-principal"></a><span data-ttu-id="dcd65-103">Excluir um appRoleAssignment concedido a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="dcd65-103">Delete an appRoleAssignment granted to a service principal</span></span>

<span data-ttu-id="dcd65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcd65-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dcd65-105">Exclui um [appRoleAssignment](../resources/approleassignment.md) que uma entidade de serviço recebeu.</span><span class="sxs-lookup"><span data-stu-id="dcd65-105">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a service principal has been granted.</span></span>

<span data-ttu-id="dcd65-106">Funções de aplicativo atribuídas a entidades de serviço também são conhecidas como [permissões de aplicativo.](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)</span><span class="sxs-lookup"><span data-stu-id="dcd65-106">App roles which are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="dcd65-107">Excluir uma atribuição de função de aplicativo para uma entidade de serviço equivale a revogar a concessão de permissão somente aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dcd65-107">Deleting an app role assignment for a service principal is equivalent to revoking the app-only permission grant.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcd65-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcd65-108">Permissions</span></span>

<span data-ttu-id="dcd65-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcd65-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcd65-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcd65-111">Permission type</span></span>      | <span data-ttu-id="dcd65-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcd65-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcd65-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcd65-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dcd65-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dcd65-114">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dcd65-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcd65-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcd65-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcd65-116">Not supported.</span></span>    |
|<span data-ttu-id="dcd65-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcd65-117">Application</span></span> | <span data-ttu-id="dcd65-118">AppRoleAssignment.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcd65-118">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcd65-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcd65-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}
```

> [!NOTE]
> <span data-ttu-id="dcd65-120">Como prática prática, recomendamos excluir atribuições de função de aplicativo por meio da relação da entidade de serviço de recursos, em vez da relação do usuário, grupo ou entidade de `appRoleAssignedTo` serviço  `appRoleAssignments` atribuída.</span><span class="sxs-lookup"><span data-stu-id="dcd65-120">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcd65-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd65-121">Request headers</span></span>

| <span data-ttu-id="dcd65-122">Nome</span><span class="sxs-lookup"><span data-stu-id="dcd65-122">Name</span></span>       | <span data-ttu-id="dcd65-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="dcd65-123">Type</span></span> | <span data-ttu-id="dcd65-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcd65-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dcd65-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcd65-125">Authorization</span></span>  | <span data-ttu-id="dcd65-126">string</span><span class="sxs-lookup"><span data-stu-id="dcd65-126">string</span></span>  | <span data-ttu-id="dcd65-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcd65-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcd65-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd65-129">Request body</span></span>

<span data-ttu-id="dcd65-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcd65-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcd65-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcd65-131">Response</span></span>

<span data-ttu-id="dcd65-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcd65-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcd65-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dcd65-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcd65-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcd65-135">Request</span></span>

<span data-ttu-id="dcd65-136">Aqui está um exemplo da solicitação para excluir uma atribuição de função de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dcd65-136">Here is an example of the request to delete an app role assignment.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}
```

### <a name="response"></a><span data-ttu-id="dcd65-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcd65-137">Response</span></span>

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
