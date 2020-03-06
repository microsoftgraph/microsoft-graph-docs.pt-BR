---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 390e170f306cb28d0b676efe4933ba204b23e16f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516862"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="b0d4f-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b0d4f-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="b0d4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0d4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0d4f-105">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0d4f-105">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0d4f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0d4f-106">Permissions</span></span>

<span data-ttu-id="b0d4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0d4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0d4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0d4f-109">Permission type</span></span>      | <span data-ttu-id="b0d4f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0d4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0d4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0d4f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b0d4f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0d4f-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b0d4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0d4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0d4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0d4f-114">Not supported.</span></span>    |
|<span data-ttu-id="b0d4f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0d4f-115">Application</span></span> | <span data-ttu-id="b0d4f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0d4f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0d4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0d4f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="b0d4f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d4f-118">Request headers</span></span>

| <span data-ttu-id="b0d4f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b0d4f-119">Name</span></span> | <span data-ttu-id="b0d4f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0d4f-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b0d4f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0d4f-121">Authorization</span></span> | <span data-ttu-id="b0d4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0d4f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0d4f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b0d4f-124">Content-Type</span></span>  | <span data-ttu-id="b0d4f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0d4f-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0d4f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d4f-126">Request body</span></span>
<span data-ttu-id="b0d4f-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0d4f-127">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b0d4f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0d4f-128">Response</span></span>

<span data-ttu-id="b0d4f-129">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0d4f-129">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0d4f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0d4f-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b0d4f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d4f-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="b0d4f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0d4f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="b0d4f-133">C#</span><span class="sxs-lookup"><span data-stu-id="b0d4f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b0d4f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b0d4f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b0d4f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b0d4f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b0d4f-136">Java</span><span class="sxs-lookup"><span data-stu-id="b0d4f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-grouplifecyclepolicy-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b0d4f-137">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b0d4f-137">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b0d4f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0d4f-138">Response</span></span>

<span data-ttu-id="b0d4f-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0d4f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
