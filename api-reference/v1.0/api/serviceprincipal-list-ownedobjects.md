---
title: 'servicePrincipals: Lista ownedObjects'
description: Recupere uma lista de objetos pertencentes ao servicePrincipal.  Isto poderia incluir aplicativos ou grupos.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d9788a22e1d72bd98503da742a0295e7ed404e3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972767"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="1919a-104">servicePrincipals: Lista ownedObjects</span><span class="sxs-lookup"><span data-stu-id="1919a-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="1919a-105">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1919a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1919a-106">Recupere uma lista de objetos pertencentes ao [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="1919a-106">Retrieve a list of objects owned by the [servicePrincipal](../resources/serviceprincipal.md).</span></span>  <span data-ttu-id="1919a-107">Isto poderia incluir aplicativos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="1919a-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="1919a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1919a-108">Permissions</span></span>
<span data-ttu-id="1919a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1919a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1919a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1919a-111">Permission type</span></span>      | <span data-ttu-id="1919a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1919a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1919a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1919a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1919a-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1919a-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1919a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1919a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1919a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1919a-116">Not supported.</span></span>    |
|<span data-ttu-id="1919a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1919a-117">Application</span></span> | <span data-ttu-id="1919a-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1919a-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1919a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1919a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1919a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1919a-120">Optional query parameters</span></span>
<span data-ttu-id="1919a-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1919a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1919a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1919a-122">Request headers</span></span>
| <span data-ttu-id="1919a-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1919a-123">Name</span></span>           | <span data-ttu-id="1919a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1919a-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="1919a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1919a-125">Authorization</span></span>  | <span data-ttu-id="1919a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1919a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1919a-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1919a-128">Request body</span></span>
<span data-ttu-id="1919a-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1919a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1919a-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1919a-130">Response</span></span>

<span data-ttu-id="1919a-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1919a-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="1919a-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1919a-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="1919a-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1919a-133">Request</span></span>
<span data-ttu-id="1919a-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1919a-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1919a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1919a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="1919a-136">C#</span><span class="sxs-lookup"><span data-stu-id="1919a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1919a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1919a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1919a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1919a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1919a-139">Java</span><span class="sxs-lookup"><span data-stu-id="1919a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1919a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="1919a-140">Response</span></span>
<span data-ttu-id="1919a-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1919a-141">Here is an example of the response.</span></span> 
><span data-ttu-id="1919a-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1919a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

