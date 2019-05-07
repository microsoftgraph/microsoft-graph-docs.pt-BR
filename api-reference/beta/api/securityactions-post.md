---
title: Criar securityAction
description: Criar um novo objeto SecurityAction. "
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: aa105383597c6d97e1a61d95dc9593b21547a0ee
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638757"
---
# <a name="create-securityaction"></a><span data-ttu-id="a91a4-103">Criar securityAction</span><span class="sxs-lookup"><span data-stu-id="a91a4-103">Create securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a91a4-104">Criar um novo [](../resources/securityaction.md) objeto SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="a91a4-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a91a4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a91a4-105">Permissions</span></span>

<span data-ttu-id="a91a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a91a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a91a4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a91a4-108">Permission type</span></span>                        | <span data-ttu-id="a91a4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a91a4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a91a4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a91a4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a91a4-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a91a4-111">Not supported.</span></span> |
| <span data-ttu-id="a91a4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a91a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a91a4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a91a4-113">Not supported.</span></span> |
| <span data-ttu-id="a91a4-114">Application</span><span class="sxs-lookup"><span data-stu-id="a91a4-114">Application</span></span>                            | <span data-ttu-id="a91a4-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a91a4-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a91a4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a91a4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="a91a4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a91a4-117">Request headers</span></span>

| <span data-ttu-id="a91a4-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a91a4-118">Name</span></span>          | <span data-ttu-id="a91a4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a91a4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a91a4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a91a4-120">Authorization</span></span> | <span data-ttu-id="a91a4-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a91a4-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a91a4-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a91a4-122">Request body</span></span>

<span data-ttu-id="a91a4-123">No corpo da solicitação, forneça uma representação JSON de um [](../resources/securityaction.md) objeto SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="a91a4-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a91a4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="a91a4-124">Response</span></span>

<span data-ttu-id="a91a4-125">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a91a4-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a91a4-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a91a4-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a91a4-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a91a4-127">Request</span></span>

<span data-ttu-id="a91a4-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a91a4-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions
Content-type: application/json

{
  "name": "BlockIp",
  "actionReason": "Test",
  "parameters": [
    {
      "name": "IP",
      "value": "1.2.3.4"
    }
  ],
  "vendorInformation": {
    "provider": "Windows Defender ATP",
    "vendor": "Microsoft"
  }
}
```

### <a name="response"></a><span data-ttu-id="a91a4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a91a4-129">Response</span></span>

<span data-ttu-id="a91a4-130">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a91a4-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a91a4-131">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a91a4-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a91a4-132">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a91a4-132">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id" : "1234567890",
    "status" : "notStarted",
    "createdDateTime": "2019-01-10 12:23:23.33333",
    "lastActionDateTime": "2019-01-10 12:23:23.33333",
    "name": "blockIp",
    "actionReason": "Test",
    "errorInfo": null,
    "vendorInformation": {
        "provider": "Windows Defender ATP",
        "providerVersion": null,
        "subProvider": null,
        "vendor": "Microsoft"
    },
    "parameters": [
        {
            "name": "IP",
            "value": "1.2.3.4"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a91a4-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a91a4-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a91a4-134">Basic</span><span class="sxs-lookup"><span data-stu-id="a91a4-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_securityaction_from_security-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a91a4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a91a4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_securityaction_from_security-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securityactions-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securityactions-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
