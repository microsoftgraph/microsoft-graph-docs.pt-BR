---
title: Listar appRoleAssignments concedidos a uma entidade de serviço
description: Recupere a lista de atribuições de função de aplicativo concedidas a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 12321fefbc8d14bf697c149ecbdeb4a4666b13d8
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291129"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a><span data-ttu-id="46ee7-103">Listar appRoleAssignments concedidos a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="46ee7-103">List appRoleAssignments granted to a service principal</span></span>

<span data-ttu-id="46ee7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46ee7-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="46ee7-105">Recupere a lista de [appRoleAssignment](../resources/approleassignment.md) que foram concedidas a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="46ee7-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a service principal.</span></span>

<span data-ttu-id="46ee7-106">As funções de aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="46ee7-106">App roles that are assigned to service principals are also known as [application permissions](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="46ee7-107">As permissões de aplicativo podem ser concedidas diretamente criando atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="46ee7-107">Application permissions can be granted directly by creating app role assignments, or through a [consent experience](https://docs.microsoft.com/azure/active-directory/develop/application-consent-experience).</span></span>

## <a name="permissions"></a><span data-ttu-id="46ee7-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="46ee7-108">Permissions</span></span>

<span data-ttu-id="46ee7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ee7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46ee7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46ee7-111">Permission type</span></span>      | <span data-ttu-id="46ee7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46ee7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46ee7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46ee7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="46ee7-114">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="46ee7-114">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="46ee7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46ee7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46ee7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46ee7-116">Not supported.</span></span>    |
|<span data-ttu-id="46ee7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46ee7-117">Application</span></span> | <span data-ttu-id="46ee7-118">Directory. Read. All, AppRoleAssignment. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="46ee7-118">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46ee7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46ee7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46ee7-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="46ee7-120">Optional query parameters</span></span>

<span data-ttu-id="46ee7-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="46ee7-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46ee7-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46ee7-122">Request headers</span></span>

| <span data-ttu-id="46ee7-123">Nome</span><span class="sxs-lookup"><span data-stu-id="46ee7-123">Name</span></span>           | <span data-ttu-id="46ee7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="46ee7-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="46ee7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="46ee7-125">Authorization</span></span>  | <span data-ttu-id="46ee7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46ee7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="46ee7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46ee7-128">Request body</span></span>

<span data-ttu-id="46ee7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46ee7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46ee7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="46ee7-130">Response</span></span>

<span data-ttu-id="46ee7-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46ee7-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46ee7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46ee7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="46ee7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46ee7-133">Request</span></span>

<span data-ttu-id="46ee7-134">Veja a seguir um exemplo de uma solicitação para recuperar as funções de aplicativo que foram atribuídas a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="46ee7-134">The following is an example of a request to retrieve the app roles that have been assigned to a service principal.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/appRoleAssignments
```

### <a name="response"></a><span data-ttu-id="46ee7-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="46ee7-135">Response</span></span>

<span data-ttu-id="46ee7-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46ee7-136">Here is an example of the response.</span></span> 

> <span data-ttu-id="46ee7-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46ee7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
