---
title: Obter groupLifecyclePolicy
description: Recupera as propriedades e os relacionamentos de um objeto groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: fa1d49cf580cfcd8f1ddbf4de82a9dd3520ef552
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888465"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="64fb7-103">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="64fb7-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="64fb7-104">Recupera as propriedades e os relacionamentos de um objeto [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="64fb7-104">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="64fb7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="64fb7-105">Permissions</span></span>

<span data-ttu-id="64fb7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64fb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64fb7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64fb7-108">Permission type</span></span>      | <span data-ttu-id="64fb7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64fb7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64fb7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64fb7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64fb7-111">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64fb7-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="64fb7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64fb7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64fb7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64fb7-113">Not supported.</span></span>    |
|<span data-ttu-id="64fb7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64fb7-114">Application</span></span> | <span data-ttu-id="64fb7-115">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64fb7-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64fb7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64fb7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64fb7-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="64fb7-117">Optional query parameters</span></span>
<span data-ttu-id="64fb7-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="64fb7-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64fb7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb7-119">Request headers</span></span>
| <span data-ttu-id="64fb7-120">Nome</span><span class="sxs-lookup"><span data-stu-id="64fb7-120">Name</span></span> | <span data-ttu-id="64fb7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="64fb7-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="64fb7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="64fb7-122">Authorization</span></span> | <span data-ttu-id="64fb7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64fb7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64fb7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb7-125">Request body</span></span>
<span data-ttu-id="64fb7-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64fb7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="64fb7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="64fb7-127">Response</span></span>
<span data-ttu-id="64fb7-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64fb7-128">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64fb7-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64fb7-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64fb7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64fb7-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="64fb7-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="64fb7-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64fb7-132">C#</span><span class="sxs-lookup"><span data-stu-id="64fb7-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64fb7-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="64fb7-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64fb7-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="64fb7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="64fb7-135">Java</span><span class="sxs-lookup"><span data-stu-id="64fb7-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64fb7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="64fb7-136">Response</span></span>

<span data-ttu-id="64fb7-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64fb7-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
