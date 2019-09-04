---
title: Listar groupLifecyclePolicies
description: Listar todos os objetos groupLifecyclePolicies.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b73cb4630a4335b236b0b5fc0bb1150fb3c7bce4
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721534"
---
# <a name="list-grouplifecyclepolicies"></a><span data-ttu-id="2bff2-103">Listar groupLifecyclePolicies</span><span class="sxs-lookup"><span data-stu-id="2bff2-103">List groupLifecyclePolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bff2-104">Listar todos os objetos [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="2bff2-104">List all the [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2bff2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2bff2-105">Permissions</span></span>

<span data-ttu-id="2bff2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bff2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2bff2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bff2-108">Permission type</span></span>      | <span data-ttu-id="2bff2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2bff2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bff2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bff2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2bff2-111">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bff2-111">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="2bff2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bff2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bff2-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2bff2-113">Not supported</span></span> |
|<span data-ttu-id="2bff2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bff2-114">Application</span></span> | <span data-ttu-id="2bff2-115">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bff2-115">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bff2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bff2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2bff2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2bff2-117">Optional query parameters</span></span>
<span data-ttu-id="2bff2-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2bff2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bff2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bff2-119">Request headers</span></span>
| <span data-ttu-id="2bff2-120">Nome</span><span class="sxs-lookup"><span data-stu-id="2bff2-120">Name</span></span> | <span data-ttu-id="2bff2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bff2-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="2bff2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bff2-122">Authorization</span></span> | <span data-ttu-id="2bff2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bff2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2bff2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bff2-125">Request body</span></span>
<span data-ttu-id="2bff2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bff2-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bff2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bff2-127">Response</span></span>

<span data-ttu-id="2bff2-128">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bff2-128">If successful, this method returns a `200 OK` response code and a collection of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bff2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bff2-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2bff2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bff2-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2bff2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bff2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groupLifecyclePolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2bff2-132">C#</span><span class="sxs-lookup"><span data-stu-id="2bff2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2bff2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bff2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2bff2-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="2bff2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2bff2-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bff2-135">Response</span></span>

<span data-ttu-id="2bff2-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bff2-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
