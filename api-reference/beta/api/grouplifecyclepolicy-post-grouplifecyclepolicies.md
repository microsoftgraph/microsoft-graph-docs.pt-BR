---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 55c0022c3bfdb53c04775cbaede074ea4f7ccfe5
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262745"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="b860f-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="b860f-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b860f-104">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b860f-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b860f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b860f-105">Permissions</span></span>

<span data-ttu-id="b860f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b860f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b860f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b860f-108">Permission type</span></span>      | <span data-ttu-id="b860f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b860f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b860f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b860f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b860f-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b860f-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="b860f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b860f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b860f-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="b860f-113">Not supported</span></span> |
|<span data-ttu-id="b860f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b860f-114">Application</span></span> |  <span data-ttu-id="b860f-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b860f-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b860f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b860f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="b860f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b860f-117">Request headers</span></span>

| <span data-ttu-id="b860f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b860f-118">Name</span></span> | <span data-ttu-id="b860f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b860f-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b860f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b860f-120">Authorization</span></span> | <span data-ttu-id="b860f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b860f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b860f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b860f-123">Content-Type</span></span>  | <span data-ttu-id="b860f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b860f-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b860f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b860f-125">Request body</span></span>
<span data-ttu-id="b860f-126">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b860f-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b860f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="b860f-127">Response</span></span>

<span data-ttu-id="b860f-128">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b860f-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b860f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b860f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b860f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b860f-130">Request</span></span>

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
<span data-ttu-id="b860f-131">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="b860f-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b860f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b860f-132">Response</span></span>

<span data-ttu-id="b860f-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b860f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b860f-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="b860f-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b860f-136">C#</span><span class="sxs-lookup"><span data-stu-id="b860f-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b860f-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b860f-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b860f-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="b860f-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
