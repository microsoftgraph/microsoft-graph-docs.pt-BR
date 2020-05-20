---
title: Listar os memberOf transitivos de servicePrincipalName
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 95a9bc73a3cca5956181123eba5bc4fa3c1bfb56
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290304"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="f7786-103">Listar os memberOf transitivos de servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f7786-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="f7786-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7786-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7786-105">Obtenha os grupos e funções de diretório dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro.</span><span class="sxs-lookup"><span data-stu-id="f7786-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="f7786-106">Essa operação é transitiva e inclui todos os grupos dos quais essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="f7786-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7786-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7786-107">Permissions</span></span>
<span data-ttu-id="f7786-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7786-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7786-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7786-110">Permission type</span></span>      | <span data-ttu-id="f7786-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7786-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7786-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7786-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7786-113">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="f7786-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f7786-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7786-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7786-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7786-115">Not supported.</span></span>    |
|<span data-ttu-id="f7786-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7786-116">Application</span></span> | <span data-ttu-id="f7786-117">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="f7786-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f7786-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7786-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7786-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7786-119">Optional query parameters</span></span>
<span data-ttu-id="f7786-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7786-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7786-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7786-121">Request headers</span></span>
| <span data-ttu-id="f7786-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f7786-122">Name</span></span>           | <span data-ttu-id="f7786-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7786-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f7786-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7786-124">Authorization</span></span>  | <span data-ttu-id="f7786-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7786-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7786-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7786-127">Request body</span></span>
<span data-ttu-id="f7786-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7786-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7786-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7786-129">Response</span></span>

<span data-ttu-id="f7786-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7786-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7786-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7786-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7786-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7786-132">Request</span></span>

<span data-ttu-id="f7786-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7786-133">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="f7786-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7786-134">Response</span></span>

<span data-ttu-id="f7786-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7786-135">Here is an example of the response.</span></span> 

><span data-ttu-id="f7786-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7786-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
