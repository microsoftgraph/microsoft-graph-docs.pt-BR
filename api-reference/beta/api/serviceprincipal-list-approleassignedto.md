---
title: Listar appRoleAssignments concedidas para uma entidade de serviço
description: Recupere uma lista de atribuições de função de aplicativo concedidas para uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: a30c80bd2dff43db3a505f593c0b30780565eef1
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291234"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a><span data-ttu-id="758d4-103">Listar appRoleAssignments concedidas para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="758d4-103">List appRoleAssignments granted for a service principal</span></span>

<span data-ttu-id="758d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="758d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="758d4-105">Recupere uma lista de [appRoleAssignment](../resources/approleassignment.md) que os usuários, grupos ou entidades de serviço de cliente foram concedidos para a entidade de serviço de recurso determinada.</span><span class="sxs-lookup"><span data-stu-id="758d4-105">Retrieve a list of [appRoleAssignment](../resources/approleassignment.md) that users, groups, or client service principals have been granted for the given resource service principal.</span></span>

<span data-ttu-id="758d4-106">Por exemplo, se a entidade de serviço de recurso é a entidade de serviço para a API do Microsoft Graph, isso retornará todas as entidades de serviço que receberam qualquer permissão somente de aplicativo para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="758d4-106">For example, if the resource service principal is the service principal for the Microsoft Graph API, this will return all service principals that have been granted any app-only permissions to Microsoft Graph.</span></span>

<span data-ttu-id="758d4-107">Se a entidade de serviço de recurso for um aplicativo que tem funções de aplicativo concedidas a usuários e grupos, isso retornará todas as funções de aplicativo atribuídas a usuários e grupos para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="758d4-107">If the resource service principal is an application that has app roles granted to users and groups, this will return all the users and groups assigned app roles for this application.</span></span>

## <a name="permissions"></a><span data-ttu-id="758d4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="758d4-108">Permissions</span></span>

<span data-ttu-id="758d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="758d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="758d4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="758d4-111">Permission type</span></span>      | <span data-ttu-id="758d4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="758d4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="758d4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="758d4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="758d4-114">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="758d4-114">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="758d4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="758d4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="758d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="758d4-116">Not supported.</span></span>    |
|<span data-ttu-id="758d4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="758d4-117">Application</span></span> | <span data-ttu-id="758d4-118">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="758d4-118">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="758d4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="758d4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="758d4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="758d4-120">Optional query parameters</span></span>

<span data-ttu-id="758d4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="758d4-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="758d4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="758d4-122">Request headers</span></span>

| <span data-ttu-id="758d4-123">Nome</span><span class="sxs-lookup"><span data-stu-id="758d4-123">Name</span></span>           | <span data-ttu-id="758d4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="758d4-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="758d4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="758d4-125">Authorization</span></span>  | <span data-ttu-id="758d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="758d4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="758d4-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="758d4-128">Request body</span></span>

<span data-ttu-id="758d4-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="758d4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="758d4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="758d4-130">Response</span></span>

<span data-ttu-id="758d4-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="758d4-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="758d4-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="758d4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="758d4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="758d4-133">Request</span></span>

<span data-ttu-id="758d4-134">Veja a seguir um exemplo da solicitação para recuperar as atribuições de funções de aplicativo que foram concedidas para uma entidade de serviço de recurso específica.</span><span class="sxs-lookup"><span data-stu-id="758d4-134">The following is an example of the request to retrieve the app roles assignments that have been granted for a given resource service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo
```

### <a name="response"></a><span data-ttu-id="758d4-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="758d4-135">Response</span></span>

<span data-ttu-id="758d4-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="758d4-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="758d4-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="758d4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
