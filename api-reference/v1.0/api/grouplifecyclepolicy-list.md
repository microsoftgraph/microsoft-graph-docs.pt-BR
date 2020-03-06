---
title: Listar groupLifecyclePolicies
description: Listar todos os objetos groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b5c4159e3ace8d85fc55a26e4313a74878e5de07
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516869"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="22791-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="22791-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="22791-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22791-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22791-105">Listar todos os objetos [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="22791-105">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="22791-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="22791-106">Permissions</span></span>

<span data-ttu-id="22791-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22791-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="22791-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22791-109">Permission type</span></span>      | <span data-ttu-id="22791-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22791-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22791-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22791-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22791-112">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22791-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="22791-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22791-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22791-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22791-114">Not supported.</span></span>    |
|<span data-ttu-id="22791-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22791-115">Application</span></span> | <span data-ttu-id="22791-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22791-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="22791-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22791-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="22791-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22791-118">Optional query parameters</span></span>
<span data-ttu-id="22791-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22791-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="22791-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22791-120">Request headers</span></span>
| <span data-ttu-id="22791-121">Nome</span><span class="sxs-lookup"><span data-stu-id="22791-121">Name</span></span> | <span data-ttu-id="22791-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="22791-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="22791-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22791-123">Authorization</span></span> | <span data-ttu-id="22791-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22791-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22791-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22791-126">Request body</span></span>
<span data-ttu-id="22791-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22791-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22791-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="22791-128">Response</span></span>

<span data-ttu-id="22791-129">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22791-129">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22791-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22791-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="22791-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22791-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="22791-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="22791-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="22791-133">C#</span><span class="sxs-lookup"><span data-stu-id="22791-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22791-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22791-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22791-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22791-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22791-136">Java</span><span class="sxs-lookup"><span data-stu-id="22791-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="22791-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="22791-137">Response</span></span>

<span data-ttu-id="22791-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22791-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 223

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
