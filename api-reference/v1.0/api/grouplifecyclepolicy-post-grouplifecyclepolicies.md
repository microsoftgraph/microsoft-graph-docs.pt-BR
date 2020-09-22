---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: aaddcd0edbc1e00e21e2f53fa96580c73a24256b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041852"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="f0686-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="f0686-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="f0686-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0686-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0686-105">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0686-105">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f0686-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0686-106">Permissions</span></span>

<span data-ttu-id="f0686-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0686-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0686-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0686-109">Permission type</span></span>      | <span data-ttu-id="f0686-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0686-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0686-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0686-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0686-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0686-112">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f0686-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0686-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0686-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0686-114">Not supported.</span></span>    |
|<span data-ttu-id="f0686-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0686-115">Application</span></span> | <span data-ttu-id="f0686-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0686-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0686-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0686-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="f0686-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0686-118">Request headers</span></span>

| <span data-ttu-id="f0686-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f0686-119">Name</span></span> | <span data-ttu-id="f0686-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0686-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="f0686-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0686-121">Authorization</span></span> | <span data-ttu-id="f0686-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0686-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f0686-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0686-124">Content-Type</span></span>  | <span data-ttu-id="f0686-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0686-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0686-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0686-126">Request body</span></span>
<span data-ttu-id="f0686-127">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0686-127">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f0686-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0686-128">Response</span></span>

<span data-ttu-id="f0686-129">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0686-129">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0686-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0686-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f0686-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0686-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f0686-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0686-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f0686-133">C#</span><span class="sxs-lookup"><span data-stu-id="f0686-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0686-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0686-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0686-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0686-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0686-136">Java</span><span class="sxs-lookup"><span data-stu-id="f0686-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-grouplifecyclepolicy-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f0686-137">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f0686-137">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f0686-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0686-138">Response</span></span>

<span data-ttu-id="f0686-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0686-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

