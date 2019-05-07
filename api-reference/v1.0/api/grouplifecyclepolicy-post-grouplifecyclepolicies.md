---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7fe5f1dd57039611d4c0378a1ce568b71a22ca28
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613368"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="b3802-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b3802-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="b3802-104">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b3802-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3802-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3802-105">Permissions</span></span>

<span data-ttu-id="b3802-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3802-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3802-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3802-108">Permission type</span></span>      | <span data-ttu-id="b3802-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3802-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3802-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3802-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b3802-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3802-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b3802-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3802-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3802-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3802-113">Not supported.</span></span>    |
|<span data-ttu-id="b3802-114">Application</span><span class="sxs-lookup"><span data-stu-id="b3802-114">Application</span></span> | <span data-ttu-id="b3802-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3802-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3802-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3802-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="b3802-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3802-117">Request headers</span></span>

| <span data-ttu-id="b3802-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b3802-118">Name</span></span> | <span data-ttu-id="b3802-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3802-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b3802-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3802-120">Authorization</span></span> | <span data-ttu-id="b3802-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3802-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3802-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3802-123">Content-Type</span></span>  | <span data-ttu-id="b3802-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b3802-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3802-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3802-125">Request body</span></span>
<span data-ttu-id="b3802-126">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b3802-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b3802-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3802-127">Response</span></span>

<span data-ttu-id="b3802-128">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3802-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3802-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3802-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3802-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3802-130">Request</span></span>

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
<span data-ttu-id="b3802-131">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b3802-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b3802-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3802-132">Response</span></span>

<span data-ttu-id="b3802-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3802-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b3802-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b3802-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b3802-136">Basic</span><span class="sxs-lookup"><span data-stu-id="b3802-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3802-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3802-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
