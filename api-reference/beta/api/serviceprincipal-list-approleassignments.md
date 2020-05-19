---
title: Listar appRoleAssignments concedidos a uma entidade de serviço
description: Recupere a lista de atribuições de função de aplicativo concedidas a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 6ca7252f8c408a8bdff89159e058488e2d56533b
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290732"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a><span data-ttu-id="b89b9-103">Listar appRoleAssignments concedidos a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="b89b9-103">List appRoleAssignments granted to a service principal</span></span>

<span data-ttu-id="b89b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b89b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b89b9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b89b9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b89b9-106">Recupere a lista de [appRoleAssignment](../resources/approleassignment.md) que foram concedidas a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="b89b9-106">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a service principal.</span></span>

<span data-ttu-id="b89b9-107">As funções de aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="b89b9-107">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="b89b9-108">As permissões de aplicativo podem ser concedidas diretamente criando atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="b89b9-108">Application permissions can be granted directly by creating app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

## <a name="permissions"></a><span data-ttu-id="b89b9-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="b89b9-109">Permissions</span></span>

<span data-ttu-id="b89b9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b89b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b89b9-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b89b9-112">Permission type</span></span>      | <span data-ttu-id="b89b9-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b89b9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b89b9-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b89b9-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b89b9-115">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="b89b9-115">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="b89b9-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b89b9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b89b9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b89b9-117">Not supported.</span></span>    |
|<span data-ttu-id="b89b9-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b89b9-118">Application</span></span> | <span data-ttu-id="b89b9-119">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b89b9-119">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b89b9-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b89b9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b89b9-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b89b9-121">Optional query parameters</span></span>

<span data-ttu-id="b89b9-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b89b9-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b89b9-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b89b9-123">Request headers</span></span>

| <span data-ttu-id="b89b9-124">Nome</span><span class="sxs-lookup"><span data-stu-id="b89b9-124">Name</span></span>           | <span data-ttu-id="b89b9-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b89b9-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b89b9-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="b89b9-126">Authorization</span></span>  | <span data-ttu-id="b89b9-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b89b9-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b89b9-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b89b9-129">Request body</span></span>

<span data-ttu-id="b89b9-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b89b9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b89b9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b89b9-131">Response</span></span>

<span data-ttu-id="b89b9-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b89b9-132">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b89b9-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b89b9-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b89b9-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b89b9-134">Request</span></span>

<span data-ttu-id="b89b9-135">Veja a seguir um exemplo de uma solicitação para recuperar as funções de aplicativo que foram atribuídas a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="b89b9-135">The following is an example of a request to retrieve the app roles that have been assigned to a service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```

### <a name="response"></a><span data-ttu-id="b89b9-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b89b9-136">Response</span></span>

<span data-ttu-id="b89b9-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b89b9-137">Here is an example of the response.</span></span> 

> <span data-ttu-id="b89b9-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b89b9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
