---
title: Criar groupLifecyclePolicy
description: Cria um novo objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 11a4f7dcd79641fc3cf1bb5e8ca3ae7b48ecd1f8
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592331"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="ec7fe-103">Criar groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="ec7fe-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec7fe-104">Cria um novo objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ec7fe-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ec7fe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec7fe-105">Permissions</span></span>

<span data-ttu-id="ec7fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec7fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ec7fe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec7fe-108">Permission type</span></span>      | <span data-ttu-id="ec7fe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec7fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec7fe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec7fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec7fe-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec7fe-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="ec7fe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec7fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec7fe-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="ec7fe-113">Not supported</span></span> |
|<span data-ttu-id="ec7fe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec7fe-114">Application</span></span> |  <span data-ttu-id="ec7fe-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec7fe-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec7fe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec7fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="ec7fe-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec7fe-117">Request headers</span></span>

| <span data-ttu-id="ec7fe-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ec7fe-118">Name</span></span> | <span data-ttu-id="ec7fe-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec7fe-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ec7fe-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec7fe-120">Authorization</span></span> | <span data-ttu-id="ec7fe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec7fe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec7fe-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec7fe-123">Content-Type</span></span>  | <span data-ttu-id="ec7fe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ec7fe-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec7fe-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec7fe-125">Request body</span></span>
<span data-ttu-id="ec7fe-126">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ec7fe-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ec7fe-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec7fe-127">Response</span></span>

<span data-ttu-id="ec7fe-128">Quando é bem-sucedido, este método retorna o código de resposta `201 Created` e uma coleção de objetos [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec7fe-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec7fe-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec7fe-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ec7fe-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec7fe-130">Request</span></span>

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
<span data-ttu-id="ec7fe-131">No corpo da solicitação, forneça uma representação JSON do objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="ec7fe-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ec7fe-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec7fe-132">Response</span></span>

<span data-ttu-id="ec7fe-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec7fe-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ec7fe-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ec7fe-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ec7fe-136">Basic</span><span class="sxs-lookup"><span data-stu-id="ec7fe-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec7fe-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec7fe-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
