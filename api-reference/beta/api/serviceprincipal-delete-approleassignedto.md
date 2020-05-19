---
title: Excluir um appRoleAssignment concedido para uma entidade de serviço
description: Excluir um appRoleAssignment concedido para uma entidade de serviço.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 98140e16403e9b32ca2638721ba89b963c2c878f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289142"
---
# <a name="delete-an-approleassignment-granted-for-a-service-principal"></a><span data-ttu-id="180a8-103">Excluir um appRoleAssignment concedido para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="180a8-103">Delete an appRoleAssignment granted for a service principal</span></span>

<span data-ttu-id="180a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="180a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="180a8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="180a8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="180a8-106">Exclui um [appRoleAssignment](../resources/approleassignment.md) que um usuário, grupo ou entidade de serviço de cliente foi concedido para uma entidade de serviço de recurso.</span><span class="sxs-lookup"><span data-stu-id="180a8-106">Deletes an [appRoleAssignment](../resources/approleassignment.md) that a user, group, or client service principal has been granted for a resource service principal.</span></span>

## <a name="permissions"></a><span data-ttu-id="180a8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="180a8-107">Permissions</span></span>

<span data-ttu-id="180a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="180a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="180a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="180a8-110">Permission type</span></span>      | <span data-ttu-id="180a8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="180a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="180a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="180a8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="180a8-113">AppRoleAssignment. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="180a8-113">AppRoleAssignment.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="180a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="180a8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="180a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="180a8-115">Not supported.</span></span>    |
|<span data-ttu-id="180a8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="180a8-116">Application</span></span> | <span data-ttu-id="180a8-117">AppRoleAssignment. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="180a8-117">AppRoleAssignment.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="180a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="180a8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/appRoleAssignedTo/{id}
```

> [!NOTE]
> <span data-ttu-id="180a8-119">Como prática recomendada, recomendamos a exclusão de atribuições de função de aplicativo através da `appRoleAssignedTo` relação da entidade de serviço de _recurso_ , em vez da `appRoleAssignments` relação do usuário, grupo ou entidade de serviço atribuída.</span><span class="sxs-lookup"><span data-stu-id="180a8-119">As a best practice, we recommend deleting app role assignments through the `appRoleAssignedTo` relationship of the _resource_ service principal, instead of the `appRoleAssignments` relationship of the assigned user, group, or service principal.</span></span>

## <a name="request-headers"></a><span data-ttu-id="180a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="180a8-120">Request headers</span></span>

| <span data-ttu-id="180a8-121">Nome</span><span class="sxs-lookup"><span data-stu-id="180a8-121">Name</span></span>       | <span data-ttu-id="180a8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="180a8-122">Type</span></span> | <span data-ttu-id="180a8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="180a8-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="180a8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="180a8-124">Authorization</span></span>  | <span data-ttu-id="180a8-125">string</span><span class="sxs-lookup"><span data-stu-id="180a8-125">string</span></span>  | <span data-ttu-id="180a8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="180a8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="180a8-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="180a8-128">Request body</span></span>

<span data-ttu-id="180a8-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="180a8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="180a8-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="180a8-130">Response</span></span>

<span data-ttu-id="180a8-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="180a8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="180a8-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="180a8-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="180a8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="180a8-134">Request</span></span>

<span data-ttu-id="180a8-135">Veja a seguir um exemplo da solicitação para excluir uma atribuição de função de aplicativo da entidade de serviço de recurso.</span><span class="sxs-lookup"><span data-stu-id="180a8-135">Here is an example of the request to delete an app role assignment from the resource service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_approleassignedto"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```

### <a name="response"></a><span data-ttu-id="180a8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="180a8-136">Response</span></span>

<span data-ttu-id="180a8-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="180a8-137">The following is an example of the response.</span></span>

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
