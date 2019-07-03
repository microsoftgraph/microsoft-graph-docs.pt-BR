---
title: Listar groupLifecyclePolicies
description: Listar todos os objetos groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c189ea32cd67b025c0182e6e25a853637f0320aa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445692"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="607bd-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="607bd-103">List groupLifecyclePolicies</span></span>

<span data-ttu-id="607bd-104">Listar todos os objetos [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="607bd-104">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="607bd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="607bd-105">Permissions</span></span>

<span data-ttu-id="607bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="607bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="607bd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="607bd-108">Permission type</span></span>      | <span data-ttu-id="607bd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="607bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="607bd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="607bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="607bd-111">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607bd-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="607bd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="607bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="607bd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="607bd-113">Not supported.</span></span>    |
|<span data-ttu-id="607bd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="607bd-114">Application</span></span> | <span data-ttu-id="607bd-115">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607bd-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="607bd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="607bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="607bd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="607bd-117">Optional query parameters</span></span>
<span data-ttu-id="607bd-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="607bd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="607bd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="607bd-119">Request headers</span></span>
| <span data-ttu-id="607bd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="607bd-120">Name</span></span> | <span data-ttu-id="607bd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="607bd-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="607bd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="607bd-122">Authorization</span></span> | <span data-ttu-id="607bd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="607bd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="607bd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="607bd-125">Request body</span></span>
<span data-ttu-id="607bd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="607bd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="607bd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="607bd-127">Response</span></span>

<span data-ttu-id="607bd-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="607bd-128">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="607bd-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="607bd-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="607bd-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="607bd-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="607bd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="607bd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="607bd-132">C#</span><span class="sxs-lookup"><span data-stu-id="607bd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="607bd-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="607bd-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="607bd-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="607bd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="607bd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="607bd-135">Response</span></span>

<span data-ttu-id="607bd-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="607bd-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
