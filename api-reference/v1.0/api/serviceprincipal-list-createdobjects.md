---
title: 'servicePrincipalName: listar createdObjects'
description: Recupere uma lista de objetos directoryobject.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: b3267b4234b6bf759458474e73bfc93027245b69
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383978"
---
# <a name="serviceprincipal-list-createdobjects"></a><span data-ttu-id="b93ae-103">servicePrincipalName: listar createdObjects</span><span class="sxs-lookup"><span data-stu-id="b93ae-103">servicePrincipal: List createdObjects</span></span>

<span data-ttu-id="b93ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b93ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b93ae-105">Recupere uma lista de objetos directoryobject.</span><span class="sxs-lookup"><span data-stu-id="b93ae-105">Retrieve a list of directoryobject objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b93ae-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b93ae-106">Permissions</span></span>
<span data-ttu-id="b93ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b93ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b93ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b93ae-109">Permission type</span></span>      | <span data-ttu-id="b93ae-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b93ae-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b93ae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b93ae-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b93ae-112">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="b93ae-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b93ae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b93ae-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b93ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b93ae-114">Not supported.</span></span>    |
|<span data-ttu-id="b93ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b93ae-115">Application</span></span> | <span data-ttu-id="b93ae-116">Application. Read. All, Application. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="b93ae-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="b93ae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b93ae-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b93ae-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b93ae-118">Optional query parameters</span></span>
<span data-ttu-id="b93ae-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b93ae-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b93ae-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b93ae-120">Request headers</span></span>
| <span data-ttu-id="b93ae-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b93ae-121">Name</span></span>           | <span data-ttu-id="b93ae-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b93ae-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b93ae-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b93ae-123">Authorization</span></span>  | <span data-ttu-id="b93ae-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b93ae-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b93ae-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b93ae-126">Request body</span></span>
<span data-ttu-id="b93ae-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b93ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b93ae-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b93ae-128">Response</span></span>

<span data-ttu-id="b93ae-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b93ae-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="b93ae-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b93ae-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="b93ae-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b93ae-131">Request</span></span>
<span data-ttu-id="b93ae-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b93ae-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b93ae-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b93ae-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipals_get_createdobjects"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/createdObjects
```
# <a name="c"></a>[<span data-ttu-id="b93ae-134">C#</span><span class="sxs-lookup"><span data-stu-id="b93ae-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-get-createdobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b93ae-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b93ae-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-get-createdobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b93ae-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b93ae-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-get-createdobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b93ae-137">Java</span><span class="sxs-lookup"><span data-stu-id="b93ae-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipals-get-createdobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b93ae-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b93ae-138">Response</span></span>
<span data-ttu-id="b93ae-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b93ae-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
