---
title: 'servicePrincipals: Lista ownedObjects'
description: Recupere uma lista de objetos pertencentes ao servicePrincipal.  Isto poderia incluir aplicativos ou grupos.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 614d91b837bf5a275d19171271336ab5fa3faec0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134313"
---
# <a name="serviceprincipals-list-ownedobjects"></a><span data-ttu-id="e05cf-104">servicePrincipals: Lista ownedObjects</span><span class="sxs-lookup"><span data-stu-id="e05cf-104">servicePrincipals: List ownedObjects</span></span>

<span data-ttu-id="e05cf-105">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e05cf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e05cf-106">Recupere uma lista de objetos pertencentes ao [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="e05cf-106">Retrieve a list of objects owned by the [servicePrincipal](../resources/serviceprincipal.md).</span></span>  <span data-ttu-id="e05cf-107">Isto poderia incluir aplicativos ou grupos.</span><span class="sxs-lookup"><span data-stu-id="e05cf-107">This could include applications or groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="e05cf-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e05cf-108">Permissions</span></span>
<span data-ttu-id="e05cf-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e05cf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e05cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e05cf-111">Permission type</span></span>      | <span data-ttu-id="e05cf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e05cf-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e05cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e05cf-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e05cf-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e05cf-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e05cf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e05cf-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e05cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e05cf-116">Not supported.</span></span>    |
|<span data-ttu-id="e05cf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e05cf-117">Application</span></span> | <span data-ttu-id="e05cf-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e05cf-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e05cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e05cf-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e05cf-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e05cf-120">Optional query parameters</span></span>
<span data-ttu-id="e05cf-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e05cf-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e05cf-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e05cf-122">Request headers</span></span>
| <span data-ttu-id="e05cf-123">Nome</span><span class="sxs-lookup"><span data-stu-id="e05cf-123">Name</span></span>           | <span data-ttu-id="e05cf-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e05cf-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="e05cf-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e05cf-125">Authorization</span></span>  | <span data-ttu-id="e05cf-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e05cf-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e05cf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e05cf-128">Request body</span></span>
<span data-ttu-id="e05cf-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e05cf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e05cf-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e05cf-130">Response</span></span>

<span data-ttu-id="e05cf-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e05cf-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="e05cf-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e05cf-132">Examples</span></span>
### <a name="request"></a><span data-ttu-id="e05cf-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e05cf-133">Request</span></span>
<span data-ttu-id="e05cf-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e05cf-134">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e05cf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e05cf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/ownedObjects
```
# <a name="c"></a>[<span data-ttu-id="e05cf-136">C#</span><span class="sxs-lookup"><span data-stu-id="e05cf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-ownedobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e05cf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e05cf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-ownedobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e05cf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e05cf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-ownedobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e05cf-139">Java</span><span class="sxs-lookup"><span data-stu-id="e05cf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-ownedobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e05cf-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e05cf-140">Response</span></span>
<span data-ttu-id="e05cf-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e05cf-141">Here is an example of the response.</span></span> 
><span data-ttu-id="e05cf-p105">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e05cf-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

