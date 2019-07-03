---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f022be2e393f10805e9d62c49a6dbfd8333d93e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442605"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="7bf10-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="7bf10-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bf10-104">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bf10-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7bf10-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7bf10-105">Permissions</span></span>

<span data-ttu-id="7bf10-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bf10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7bf10-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7bf10-108">Permission type</span></span>      | <span data-ttu-id="7bf10-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7bf10-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bf10-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7bf10-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7bf10-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf10-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="7bf10-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7bf10-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7bf10-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7bf10-113">Not supported</span></span> |
|<span data-ttu-id="7bf10-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7bf10-114">Application</span></span> |  <span data-ttu-id="7bf10-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bf10-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bf10-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf10-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="7bf10-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf10-117">Request headers</span></span>

| <span data-ttu-id="7bf10-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7bf10-118">Name</span></span> | <span data-ttu-id="7bf10-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bf10-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7bf10-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="7bf10-120">Authorization</span></span> | <span data-ttu-id="7bf10-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7bf10-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7bf10-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7bf10-123">Content-Type</span></span>  | <span data-ttu-id="7bf10-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7bf10-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7bf10-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf10-125">Request body</span></span>
<span data-ttu-id="7bf10-126">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bf10-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7bf10-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf10-127">Response</span></span>

<span data-ttu-id="7bf10-128">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7bf10-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bf10-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7bf10-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7bf10-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7bf10-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7bf10-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bf10-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bf10-132">C#</span><span class="sxs-lookup"><span data-stu-id="7bf10-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bf10-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="7bf10-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bf10-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="7bf10-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="7bf10-135">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="7bf10-135">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7bf10-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7bf10-136">Response</span></span>

<span data-ttu-id="7bf10-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7bf10-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
