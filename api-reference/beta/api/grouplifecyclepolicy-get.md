---
title: Obter groupLifecyclePolicy
description: Recupera as propriedades e os relacionamentos de um objeto groupLifecyclePolicies.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 43d4f6b11df2ca40af24b808b584802489963089
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459656"
---
# <a name="get-grouplifecyclepolicy"></a><span data-ttu-id="9e970-103">Obter groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="9e970-103">Get groupLifecyclePolicy</span></span>

<span data-ttu-id="9e970-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e970-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e970-105">Recupera as propriedades e os relacionamentos de um objeto [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="9e970-105">Retrieve the properties and relationships of a [groupLifecyclePolicies](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e970-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e970-106">Permissions</span></span>

<span data-ttu-id="9e970-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9e970-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e970-109">Permission type</span></span>      | <span data-ttu-id="9e970-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e970-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e970-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e970-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9e970-112">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e970-112">Directory.Read.All or Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="9e970-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e970-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e970-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9e970-114">Not supported</span></span> |
|<span data-ttu-id="9e970-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e970-115">Application</span></span> | <span data-ttu-id="9e970-116">Directory.Read.All ou Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e970-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e970-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e970-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupLifecyclePolicies/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9e970-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9e970-118">Optional query parameters</span></span>
<span data-ttu-id="9e970-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e970-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e970-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e970-120">Request headers</span></span>
| <span data-ttu-id="9e970-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9e970-121">Name</span></span> | <span data-ttu-id="9e970-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e970-122">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="9e970-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e970-123">Authorization</span></span> | <span data-ttu-id="9e970-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e970-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e970-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e970-126">Request body</span></span>
<span data-ttu-id="9e970-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e970-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9e970-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e970-128">Response</span></span>
<span data-ttu-id="9e970-129">Quando é bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e970-129">If successful, this method returns a `200 OK` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e970-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e970-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9e970-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e970-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9e970-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e970-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="9e970-133">C#</span><span class="sxs-lookup"><span data-stu-id="9e970-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e970-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e970-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e970-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e970-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9e970-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e970-136">Response</span></span>

<span data-ttu-id="9e970-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e970-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
