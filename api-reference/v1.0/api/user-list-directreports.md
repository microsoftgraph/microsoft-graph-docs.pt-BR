---
title: Listar directReports
description: Obtenha relatórios diretos do usuário.
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 17e2dd9396da3ae572e883250514b26fd3ba7c21
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51472076"
---
# <a name="list-directreports"></a><span data-ttu-id="9115f-103">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="9115f-103">List directReports</span></span>

<span data-ttu-id="9115f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9115f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9115f-105">Obtenha relatórios diretos do usuário.</span><span class="sxs-lookup"><span data-stu-id="9115f-105">Get a user's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="9115f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9115f-106">Permissions</span></span>
<span data-ttu-id="9115f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9115f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9115f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9115f-109">Permission type</span></span>      | <span data-ttu-id="9115f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9115f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9115f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9115f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9115f-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9115f-112">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="9115f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9115f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9115f-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9115f-114">Not supported</span></span> |
|<span data-ttu-id="9115f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9115f-115">Application</span></span> | <span data-ttu-id="9115f-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9115f-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="9115f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9115f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9115f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9115f-118">Optional query parameters</span></span>
<span data-ttu-id="9115f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9115f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9115f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9115f-120">Request headers</span></span>
| <span data-ttu-id="9115f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9115f-121">Header</span></span>       | <span data-ttu-id="9115f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9115f-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9115f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9115f-123">Authorization</span></span>  | <span data-ttu-id="9115f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9115f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9115f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9115f-126">Content-Type</span></span>   | <span data-ttu-id="9115f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9115f-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9115f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9115f-128">Request body</span></span>
<span data-ttu-id="9115f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9115f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9115f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9115f-130">Response</span></span>

<span data-ttu-id="9115f-131">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9115f-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9115f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9115f-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="9115f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9115f-133">Request</span></span>
<span data-ttu-id="9115f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9115f-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9115f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9115f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/directReports
```
# <a name="c"></a>[<span data-ttu-id="9115f-136">C#</span><span class="sxs-lookup"><span data-stu-id="9115f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9115f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9115f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9115f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9115f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9115f-139">Java</span><span class="sxs-lookup"><span data-stu-id="9115f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="9115f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9115f-140">Response</span></span>
<span data-ttu-id="9115f-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9115f-141">Here is an example of the response.</span></span> 

><span data-ttu-id="9115f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9115f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
      "id": "a97733ce-92a4-4e7e-8d45-8e1f3e6a69d8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

