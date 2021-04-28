---
title: Listar groupLifecyclePolicies
description: Listar todos os objetos groupLifecyclePolicies.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 50517fa50abc229104381beac9c057ac18f8805e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048691"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="58bc6-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="58bc6-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="58bc6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58bc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58bc6-105">Listar todos os objetos [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="58bc6-105">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="58bc6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="58bc6-106">Permissions</span></span>

<span data-ttu-id="58bc6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58bc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="58bc6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58bc6-109">Permission type</span></span>      | <span data-ttu-id="58bc6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58bc6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58bc6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58bc6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="58bc6-112">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bc6-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="58bc6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58bc6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58bc6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58bc6-114">Not supported.</span></span>    |
|<span data-ttu-id="58bc6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58bc6-115">Application</span></span> | <span data-ttu-id="58bc6-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58bc6-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58bc6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58bc6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="58bc6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58bc6-118">Optional query parameters</span></span>
<span data-ttu-id="58bc6-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="58bc6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58bc6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58bc6-120">Request headers</span></span>
| <span data-ttu-id="58bc6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="58bc6-121">Name</span></span> | <span data-ttu-id="58bc6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bc6-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="58bc6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58bc6-123">Authorization</span></span> | <span data-ttu-id="58bc6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58bc6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58bc6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58bc6-126">Request body</span></span>
<span data-ttu-id="58bc6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58bc6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58bc6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bc6-128">Response</span></span>

<span data-ttu-id="58bc6-129">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58bc6-129">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58bc6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58bc6-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="58bc6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58bc6-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="58bc6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bc6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
# <a name="c"></a>[<span data-ttu-id="58bc6-133">C#</span><span class="sxs-lookup"><span data-stu-id="58bc6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58bc6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bc6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58bc6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bc6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58bc6-136">Java</span><span class="sxs-lookup"><span data-stu-id="58bc6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="58bc6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bc6-137">Response</span></span>

<span data-ttu-id="58bc6-138">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="58bc6-138">Note: The response object shown here might be shortened for readability.</span></span>
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
