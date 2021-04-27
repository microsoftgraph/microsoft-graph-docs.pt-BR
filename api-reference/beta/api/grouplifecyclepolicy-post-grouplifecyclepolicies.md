---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b20b5ead43a9b8acea6751ddc09d8ffc81ab94ff
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041082"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="a0bad-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="a0bad-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="a0bad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0bad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0bad-105">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0bad-105">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a0bad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a0bad-106">Permissions</span></span>

<span data-ttu-id="a0bad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0bad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a0bad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0bad-109">Permission type</span></span>      | <span data-ttu-id="a0bad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a0bad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0bad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0bad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a0bad-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0bad-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0bad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0bad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0bad-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a0bad-114">Not supported</span></span> |
|<span data-ttu-id="a0bad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0bad-115">Application</span></span> |  <span data-ttu-id="a0bad-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0bad-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0bad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0bad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="a0bad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bad-118">Request headers</span></span>

| <span data-ttu-id="a0bad-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a0bad-119">Name</span></span> | <span data-ttu-id="a0bad-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0bad-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="a0bad-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0bad-121">Authorization</span></span> | <span data-ttu-id="a0bad-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0bad-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a0bad-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0bad-124">Content-Type</span></span>  | <span data-ttu-id="a0bad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0bad-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0bad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bad-126">Request body</span></span>
<span data-ttu-id="a0bad-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0bad-127">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0bad-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bad-128">Response</span></span>

<span data-ttu-id="a0bad-129">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0bad-129">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0bad-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0bad-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a0bad-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0bad-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a0bad-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0bad-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="a0bad-133">C#</span><span class="sxs-lookup"><span data-stu-id="a0bad-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0bad-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0bad-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0bad-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0bad-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a0bad-136">Java</span><span class="sxs-lookup"><span data-stu-id="a0bad-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-grouplifecyclepolicy-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="a0bad-137">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a0bad-137">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a0bad-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0bad-138">Response</span></span>

<span data-ttu-id="a0bad-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a0bad-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


