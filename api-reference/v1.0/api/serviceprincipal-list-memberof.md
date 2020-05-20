---
title: Listar o servicePrincipalName memberOf
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro direto. Essa operação não é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 9cf62c9457f75168c7ef7c78758c2096e76ad077
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291115"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="e3c3b-104">Listar o servicePrincipalName memberOf</span><span class="sxs-lookup"><span data-stu-id="e3c3b-104">List servicePrincipal memberOf</span></span>

<span data-ttu-id="e3c3b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3c3b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e3c3b-106">Obtenha os grupos e funções de diretório dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro direto.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-106">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a direct member of.</span></span> <span data-ttu-id="e3c3b-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3c3b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3c3b-108">Permissions</span></span>

<span data-ttu-id="e3c3b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3c3b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3c3b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3c3b-111">Permission type</span></span>      | <span data-ttu-id="e3c3b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3c3b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3c3b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3c3b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e3c3b-114">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="e3c3b-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3c3b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3c3b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3c3b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-116">Not supported.</span></span>    |
|<span data-ttu-id="e3c3b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3c3b-117">Application</span></span> | <span data-ttu-id="e3c3b-118">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e3c3b-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e3c3b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3c3b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3c3b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3c3b-120">Optional query parameters</span></span>

<span data-ttu-id="e3c3b-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3c3b-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c3b-122">Request headers</span></span>
| <span data-ttu-id="e3c3b-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e3c3b-123">Name</span></span>           | <span data-ttu-id="e3c3b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c3b-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e3c3b-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3c3b-125">Authorization</span></span>  | <span data-ttu-id="e3c3b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3c3b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c3b-128">Request body</span></span>
<span data-ttu-id="e3c3b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3c3b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c3b-130">Response</span></span>

<span data-ttu-id="e3c3b-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3c3b-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e3c3b-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3c3b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c3b-133">Request</span></span>

<span data-ttu-id="e3c3b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="e3c3b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c3b-135">Response</span></span>

<span data-ttu-id="e3c3b-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-136">Here is an example of the response.</span></span> 
><span data-ttu-id="e3c3b-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3c3b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
