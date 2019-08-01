---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: efb24101e86b1068d38fb9d2127e629b32a2fe9d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014596"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="b6850-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b6850-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="b6850-104">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6850-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b6850-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b6850-105">Permissions</span></span>

<span data-ttu-id="b6850-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6850-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6850-108">Permission type</span></span>      | <span data-ttu-id="b6850-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b6850-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b6850-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6850-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b6850-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6850-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b6850-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6850-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b6850-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6850-113">Not supported.</span></span>    |
|<span data-ttu-id="b6850-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6850-114">Application</span></span> | <span data-ttu-id="b6850-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6850-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b6850-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6850-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="b6850-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6850-117">Request headers</span></span>

| <span data-ttu-id="b6850-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b6850-118">Name</span></span> | <span data-ttu-id="b6850-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6850-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b6850-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6850-120">Authorization</span></span> | <span data-ttu-id="b6850-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6850-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b6850-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b6850-123">Content-Type</span></span>  | <span data-ttu-id="b6850-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b6850-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b6850-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6850-125">Request body</span></span>
<span data-ttu-id="b6850-126">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6850-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b6850-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6850-127">Response</span></span>

<span data-ttu-id="b6850-128">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6850-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6850-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6850-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b6850-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6850-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b6850-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="b6850-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b6850-132">C#</span><span class="sxs-lookup"><span data-stu-id="b6850-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b6850-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="b6850-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b6850-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b6850-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b6850-135">Java</span><span class="sxs-lookup"><span data-stu-id="b6850-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-grouplifecyclepolicy-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="b6850-136">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b6850-136">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b6850-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6850-137">Response</span></span>

<span data-ttu-id="b6850-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6850-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
