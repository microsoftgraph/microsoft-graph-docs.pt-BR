---
title: Criar securityAction
description: Criar um novo objeto SecurityAction. "
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 97eb08d27388d1396c203bd0309f80d5f3e941ff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364121"
---
# <a name="create-securityaction"></a><span data-ttu-id="4cfeb-103">Criar securityAction</span><span class="sxs-lookup"><span data-stu-id="4cfeb-103">Create securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cfeb-104">Criar um novo [](../resources/securityaction.md) objeto SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cfeb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4cfeb-105">Permissions</span></span>

<span data-ttu-id="4cfeb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cfeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4cfeb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cfeb-108">Permission type</span></span>                        | <span data-ttu-id="4cfeb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4cfeb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4cfeb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cfeb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4cfeb-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-111">Not supported.</span></span> |
| <span data-ttu-id="4cfeb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cfeb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cfeb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-113">Not supported.</span></span> |
| <span data-ttu-id="4cfeb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cfeb-114">Application</span></span>                            | <span data-ttu-id="4cfeb-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfeb-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cfeb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cfeb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="4cfeb-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfeb-117">Request headers</span></span>

| <span data-ttu-id="4cfeb-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4cfeb-118">Name</span></span>          | <span data-ttu-id="4cfeb-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cfeb-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4cfeb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cfeb-120">Authorization</span></span> | <span data-ttu-id="4cfeb-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4cfeb-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cfeb-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfeb-122">Request body</span></span>

<span data-ttu-id="4cfeb-123">No corpo da solicitação, forneça uma representação JSON de um [](../resources/securityaction.md) objeto SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4cfeb-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cfeb-124">Response</span></span>

<span data-ttu-id="4cfeb-125">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4cfeb-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4cfeb-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4cfeb-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfeb-127">Request</span></span>

<span data-ttu-id="4cfeb-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4cfeb-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cfeb-129">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4cfeb-130">C#</span><span class="sxs-lookup"><span data-stu-id="4cfeb-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4cfeb-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cfeb-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4cfeb-132">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4cfeb-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4cfeb-133">Java</span><span class="sxs-lookup"><span data-stu-id="4cfeb-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-securityaction-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4cfeb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cfeb-134">Response</span></span>

<span data-ttu-id="4cfeb-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="4cfeb-136">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4cfeb-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cfeb-137">All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
