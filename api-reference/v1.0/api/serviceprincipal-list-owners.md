---
title: 'servicePrincipalName: Listar proprietários'
description: Recuperar uma lista de proprietários do servicePrincipal.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c7b960993e37d9a8219b5fd509249767da65756a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054424"
---
# <a name="serviceprincipals-list-owners"></a><span data-ttu-id="2a4be-103">servicePrincipalName: Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="2a4be-103">servicePrincipals: List owners</span></span>

<span data-ttu-id="2a4be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a4be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a4be-105">Recuperar uma lista de proprietários do [servicePrincipal](../resources/serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="2a4be-105">Retrieve a list of owners of the [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a4be-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a4be-106">Permissions</span></span>
<span data-ttu-id="2a4be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a4be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a4be-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a4be-109">Permission type</span></span>      | <span data-ttu-id="2a4be-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a4be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a4be-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a4be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2a4be-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a4be-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2a4be-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a4be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a4be-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a4be-114">Not supported.</span></span>    |
|<span data-ttu-id="2a4be-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a4be-115">Application</span></span> | <span data-ttu-id="2a4be-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4be-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="2a4be-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/owners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2a4be-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a4be-118">Optional query parameters</span></span>
<span data-ttu-id="2a4be-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4be-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a4be-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4be-120">Request headers</span></span>
| <span data-ttu-id="2a4be-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2a4be-121">Name</span></span>           | <span data-ttu-id="2a4be-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4be-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2a4be-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a4be-123">Authorization</span></span>  | <span data-ttu-id="2a4be-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a4be-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a4be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4be-126">Request body</span></span>
<span data-ttu-id="2a4be-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a4be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a4be-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4be-128">Response</span></span>

<span data-ttu-id="2a4be-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4be-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2a4be-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2a4be-130">Examples</span></span>
### <a name="request"></a><span data-ttu-id="2a4be-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4be-131">Request</span></span>
<span data-ttu-id="2a4be-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a4be-132">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a4be-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4be-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="2a4be-134">C#</span><span class="sxs-lookup"><span data-stu-id="2a4be-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a4be-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a4be-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a4be-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a4be-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a4be-137">Java</span><span class="sxs-lookup"><span data-stu-id="2a4be-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a4be-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4be-138">Response</span></span>
<span data-ttu-id="2a4be-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4be-139">Here is an example of the response.</span></span> 

><span data-ttu-id="2a4be-140">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a4be-140">Note: The response object shown here might be shortened for readability.</span></span>
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
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
