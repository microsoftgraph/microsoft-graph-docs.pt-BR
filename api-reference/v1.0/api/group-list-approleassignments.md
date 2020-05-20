---
title: Listar appRoleAssignments concedidos a um grupo
description: Recupere a lista de appRoleAssignments que foram concedidas a um grupo.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 310629a06e911f408b780bdcbfa19c61bc7997e9
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288631"
---
# <a name="list-approleassignments-granted-to-a-group"></a><span data-ttu-id="54d60-103">Listar appRoleAssignments concedidos a um grupo</span><span class="sxs-lookup"><span data-stu-id="54d60-103">List appRoleAssignments granted to a group</span></span>

<span data-ttu-id="54d60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54d60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54d60-105">Recupere a lista de [appRoleAssignment](../resources/approleassignment.md) que foram concedidas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="54d60-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="54d60-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54d60-106">Permissions</span></span>

<span data-ttu-id="54d60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54d60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54d60-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54d60-109">Permission type</span></span>      | <span data-ttu-id="54d60-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54d60-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54d60-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54d60-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54d60-112">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="54d60-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="54d60-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54d60-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54d60-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54d60-114">Not supported.</span></span>    |
|<span data-ttu-id="54d60-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54d60-115">Application</span></span> | <span data-ttu-id="54d60-116">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="54d60-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54d60-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54d60-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54d60-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54d60-118">Optional query parameters</span></span>

<span data-ttu-id="54d60-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="54d60-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54d60-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54d60-120">Request headers</span></span>

| <span data-ttu-id="54d60-121">Nome</span><span class="sxs-lookup"><span data-stu-id="54d60-121">Name</span></span>           | <span data-ttu-id="54d60-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="54d60-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="54d60-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54d60-123">Authorization</span></span>  | <span data-ttu-id="54d60-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54d60-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54d60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54d60-126">Request body</span></span>

<span data-ttu-id="54d60-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54d60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54d60-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="54d60-128">Response</span></span>

<span data-ttu-id="54d60-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54d60-129">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54d60-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54d60-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="54d60-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54d60-131">Request</span></span>

<span data-ttu-id="54d60-132">O exemplo a seguir mostra uma solicitação para recuperar as funções de aplicativo que foram atribuídas a um grupo.</span><span class="sxs-lookup"><span data-stu-id="54d60-132">The following example shows a request to retrieve the app roles that have been assigned to a group.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_get_approleassignments"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments
```

### <a name="response"></a><span data-ttu-id="54d60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="54d60-133">Response</span></span>

<span data-ttu-id="54d60-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54d60-134">The following is an example of the response.</span></span>

> <span data-ttu-id="54d60-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54d60-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
