---
title: Listar os memberOf transitivos de servicePrincipalName
description: Obtenha os grupos e funções de diretório dos quais essa entidade de serviço é membro.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 34c55d7a806f125fc8f4a7b060eb9315a4c384a1
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383543"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="27601-103">Listar os memberOf transitivos de servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="27601-103">List servicePrincipal transitive memberOf</span></span>

<span data-ttu-id="27601-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27601-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27601-105">Obtenha os grupos e funções de diretório dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro.</span><span class="sxs-lookup"><span data-stu-id="27601-105">Get the groups and directory roles that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span> <span data-ttu-id="27601-106">Essa operação é transitiva e inclui todos os grupos dos quais essa entidade de serviço é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="27601-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="27601-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="27601-107">Permissions</span></span>
<span data-ttu-id="27601-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27601-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27601-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27601-110">Permission type</span></span>      | <span data-ttu-id="27601-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27601-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27601-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27601-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27601-113">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="27601-113">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="27601-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27601-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27601-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27601-115">Not supported.</span></span>    |
|<span data-ttu-id="27601-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27601-116">Application</span></span> | <span data-ttu-id="27601-117">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="27601-117">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="27601-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27601-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/transitiveMemberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27601-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27601-119">Optional query parameters</span></span>
<span data-ttu-id="27601-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27601-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27601-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27601-121">Request headers</span></span>
| <span data-ttu-id="27601-122">Nome</span><span class="sxs-lookup"><span data-stu-id="27601-122">Name</span></span>           | <span data-ttu-id="27601-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="27601-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="27601-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="27601-124">Authorization</span></span>  | <span data-ttu-id="27601-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27601-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27601-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27601-127">Request body</span></span>
<span data-ttu-id="27601-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27601-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27601-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="27601-129">Response</span></span>

<span data-ttu-id="27601-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27601-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27601-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27601-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="27601-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27601-132">Request</span></span>

<span data-ttu-id="27601-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27601-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="27601-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="27601-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_tranitivememberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="27601-135">C#</span><span class="sxs-lookup"><span data-stu-id="27601-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-serviceprincipal-tranitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27601-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27601-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-serviceprincipal-tranitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27601-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27601-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-serviceprincipal-tranitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="27601-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="27601-138">Response</span></span>

<span data-ttu-id="27601-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27601-139">Here is an example of the response.</span></span> 

><span data-ttu-id="27601-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27601-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
