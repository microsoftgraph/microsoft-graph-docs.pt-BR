---
title: Listar groupLifecyclePolicies
description: Recupera uma lista de objetos groupLifecyclePolicy à qual um grupo pertence.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1ad60e5e1890e2b6c8451ac8a0e7058f0225f29d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721571"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="3619b-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="3619b-103">List groupLifecyclePolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3619b-104">Recupera uma lista de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) à qual um grupo pertence.</span><span class="sxs-lookup"><span data-stu-id="3619b-104">Retrieves a list of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects to which a group belongs.</span></span>

## <a name="permissions"></a><span data-ttu-id="3619b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3619b-105">Permissions</span></span>

<span data-ttu-id="3619b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3619b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3619b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3619b-108">Permission type</span></span>      | <span data-ttu-id="3619b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3619b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3619b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3619b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3619b-111">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3619b-111">Directory.Read.All, Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3619b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3619b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3619b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3619b-113">Not supported.</span></span>    |
|<span data-ttu-id="3619b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3619b-114">Application</span></span> | <span data-ttu-id="3619b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3619b-115">Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3619b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3619b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3619b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3619b-117">Optional query parameters</span></span>
<span data-ttu-id="3619b-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3619b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3619b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3619b-119">Request headers</span></span>
| <span data-ttu-id="3619b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3619b-120">Name</span></span> | <span data-ttu-id="3619b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3619b-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="3619b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3619b-122">Authorization</span></span> | <span data-ttu-id="3619b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3619b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3619b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3619b-125">Request body</span></span>
<span data-ttu-id="3619b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3619b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3619b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3619b-127">Response</span></span>
<span data-ttu-id="3619b-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3619b-128">If successful, this method returns a `200 OK` response code and collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3619b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3619b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3619b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3619b-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3619b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3619b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/groupLifecyclePolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3619b-132">C#</span><span class="sxs-lookup"><span data-stu-id="3619b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3619b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3619b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3619b-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3619b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3619b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3619b-135">Response</span></span>

<span data-ttu-id="3619b-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3619b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 227

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 90,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
