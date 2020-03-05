---
title: Criar securityAction
description: Criar um novo objeto SecurityAction. "
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3ea1d95e1ff9380919d3d4afd2877cab2e370eae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453545"
---
# <a name="create-securityaction"></a><span data-ttu-id="091a8-103">Criar securityAction</span><span class="sxs-lookup"><span data-stu-id="091a8-103">Create securityAction</span></span>

<span data-ttu-id="091a8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="091a8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="091a8-105">Criar um novo objeto [SecurityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="091a8-105">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="091a8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="091a8-106">Permissions</span></span>

<span data-ttu-id="091a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="091a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="091a8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="091a8-109">Permission type</span></span>                        | <span data-ttu-id="091a8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="091a8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="091a8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="091a8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="091a8-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="091a8-112">Not supported.</span></span> |
| <span data-ttu-id="091a8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="091a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="091a8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="091a8-114">Not supported.</span></span> |
| <span data-ttu-id="091a8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="091a8-115">Application</span></span>                            | <span data-ttu-id="091a8-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="091a8-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="091a8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="091a8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="091a8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="091a8-118">Request headers</span></span>

| <span data-ttu-id="091a8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="091a8-119">Name</span></span>          | <span data-ttu-id="091a8-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="091a8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="091a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="091a8-121">Authorization</span></span> | <span data-ttu-id="091a8-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="091a8-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="091a8-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="091a8-123">Request body</span></span>

<span data-ttu-id="091a8-124">No corpo da solicitação, forneça uma representação JSON de um objeto [SecurityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="091a8-124">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="091a8-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="091a8-125">Response</span></span>

<span data-ttu-id="091a8-126">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um objeto [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="091a8-126">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="091a8-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="091a8-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="091a8-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="091a8-128">Request</span></span>

<span data-ttu-id="091a8-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="091a8-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="091a8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="091a8-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="091a8-131">C#</span><span class="sxs-lookup"><span data-stu-id="091a8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="091a8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="091a8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="091a8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="091a8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="091a8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="091a8-134">Response</span></span>

<span data-ttu-id="091a8-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="091a8-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="091a8-136">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="091a8-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="091a8-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="091a8-137">All the properties will be returned from an actual call.</span></span>

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
