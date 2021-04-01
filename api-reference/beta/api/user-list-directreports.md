---
title: Listar directReports
description: Obtenha relatórios diretos do usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 130338318fc3e7e970838dbbcb8d5f70e726e857
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473518"
---
# <a name="list-directreports"></a><span data-ttu-id="4126a-103">Listar directReports</span><span class="sxs-lookup"><span data-stu-id="4126a-103">List directReports</span></span>

<span data-ttu-id="4126a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4126a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4126a-105">Obtenha relatórios diretos do usuário.</span><span class="sxs-lookup"><span data-stu-id="4126a-105">Get a user's direct reports.</span></span> <span data-ttu-id="4126a-106">Retorna os usuários e contatos para quem este usuário está atribuído como gerente.</span><span class="sxs-lookup"><span data-stu-id="4126a-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="4126a-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4126a-107">Permissions</span></span>
<span data-ttu-id="4126a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4126a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4126a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4126a-110">Permission type</span></span>      | <span data-ttu-id="4126a-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4126a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4126a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4126a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4126a-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4126a-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="4126a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4126a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4126a-115">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4126a-115">Not supported</span></span> |
|<span data-ttu-id="4126a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4126a-116">Application</span></span> | <span data-ttu-id="4126a-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4126a-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="4126a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4126a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/directReports
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4126a-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4126a-119">Optional query parameters</span></span>
<span data-ttu-id="4126a-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4126a-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4126a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4126a-121">Request headers</span></span>
| <span data-ttu-id="4126a-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4126a-122">Header</span></span>       | <span data-ttu-id="4126a-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4126a-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="4126a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4126a-124">Authorization</span></span>  | <span data-ttu-id="4126a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4126a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4126a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4126a-127">Content-Type</span></span>   | <span data-ttu-id="4126a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4126a-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4126a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4126a-129">Request body</span></span>
<span data-ttu-id="4126a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4126a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4126a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="4126a-131">Response</span></span>

<span data-ttu-id="4126a-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4126a-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4126a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4126a-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="4126a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4126a-134">Request</span></span>
<span data-ttu-id="4126a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4126a-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4126a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4126a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/directReports
```
# <a name="c"></a>[<span data-ttu-id="4126a-137">C#</span><span class="sxs-lookup"><span data-stu-id="4126a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4126a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4126a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4126a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4126a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4126a-140">Java</span><span class="sxs-lookup"><span data-stu-id="4126a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="4126a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4126a-141">Response</span></span>
<span data-ttu-id="4126a-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4126a-142">Here is an example of the response.</span></span> 

><span data-ttu-id="4126a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4126a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


