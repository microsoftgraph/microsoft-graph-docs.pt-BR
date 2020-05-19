---
title: Listar appRoleAssignments concedidas a um usuário
description: Recupere a lista de atribuições de função de aplicativo concedidas a um usuário.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 803f3abc13f595ff6e0c6253009f386b3861af50
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290543"
---
# <a name="list-approleassignments-granted-to-a-user"></a><span data-ttu-id="f205c-103">Listar appRoleAssignments concedidas a um usuário</span><span class="sxs-lookup"><span data-stu-id="f205c-103">List appRoleAssignments granted to a user</span></span>

<span data-ttu-id="f205c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f205c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f205c-105">Recupere a lista de [appRoleAssignment](../resources/approleassignment.md) que um usuário recebeu.</span><span class="sxs-lookup"><span data-stu-id="f205c-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that a user has been granted.</span></span> <span data-ttu-id="f205c-106">Essa operação também retorna funções de aplicativo atribuídas a grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="f205c-106">This operation also returns app roles assigned to groups that the user is a direct member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="f205c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f205c-107">Permissions</span></span>

<span data-ttu-id="f205c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f205c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f205c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f205c-110">Permission type</span></span>      | <span data-ttu-id="f205c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f205c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f205c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f205c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f205c-113">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f205c-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="f205c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f205c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f205c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f205c-115">Not supported.</span></span>    |
|<span data-ttu-id="f205c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f205c-116">Application</span></span> | <span data-ttu-id="f205c-117">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f205c-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f205c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f205c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f205c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f205c-119">Optional query parameters</span></span>

<span data-ttu-id="f205c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f205c-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f205c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f205c-121">Request headers</span></span>

| <span data-ttu-id="f205c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f205c-122">Name</span></span>           | <span data-ttu-id="f205c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f205c-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f205c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f205c-124">Authorization</span></span>  | <span data-ttu-id="f205c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f205c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f205c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f205c-127">Request body</span></span>

<span data-ttu-id="f205c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f205c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f205c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f205c-129">Response</span></span>

<span data-ttu-id="f205c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f205c-130">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f205c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f205c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f205c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f205c-132">Request</span></span>

<span data-ttu-id="f205c-133">Aqui está um exemplo da solicitação para recuperar as funções de aplicativo que foram atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="f205c-133">Here is an example of the request to retrieve the app roles that have been assigned to a user.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments"
}-->

```http
GET https://graph.microsoft.com/beta/users/{id}/appRoleAssignments
```

### <a name="response"></a><span data-ttu-id="f205c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f205c-134">Response</span></span>

<span data-ttu-id="f205c-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f205c-135">The following is an example of the response.</span></span> 

> <span data-ttu-id="f205c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f205c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
