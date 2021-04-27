---
title: Criar securityAction
description: Crie um novo objeto securityAction."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: f1d513ca1a24a1314be48f550be1ceae81282609
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049734"
---
# <a name="create-securityaction"></a><span data-ttu-id="54940-103">Criar securityAction</span><span class="sxs-lookup"><span data-stu-id="54940-103">Create securityAction</span></span>

<span data-ttu-id="54940-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54940-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54940-105">Crie um novo [objeto securityAction.](../resources/securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="54940-105">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54940-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54940-106">Permissions</span></span>

<span data-ttu-id="54940-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54940-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54940-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54940-109">Permission type</span></span>                        | <span data-ttu-id="54940-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54940-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54940-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54940-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54940-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54940-112">Not supported.</span></span> |
| <span data-ttu-id="54940-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54940-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54940-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54940-114">Not supported.</span></span> |
| <span data-ttu-id="54940-115">Application</span><span class="sxs-lookup"><span data-stu-id="54940-115">Application</span></span>                            | <span data-ttu-id="54940-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54940-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54940-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54940-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="54940-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54940-118">Request headers</span></span>

| <span data-ttu-id="54940-119">Nome</span><span class="sxs-lookup"><span data-stu-id="54940-119">Name</span></span>          | <span data-ttu-id="54940-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="54940-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="54940-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="54940-121">Authorization</span></span> | <span data-ttu-id="54940-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="54940-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="54940-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54940-123">Request body</span></span>

<span data-ttu-id="54940-124">No corpo da solicitação, fornece uma representação JSON de um [objeto securityAction.](../resources/securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="54940-124">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="54940-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="54940-125">Response</span></span>

<span data-ttu-id="54940-126">Se tiver êxito, este método retornará `201 Created` o código de resposta e um objeto [securityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54940-126">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54940-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="54940-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54940-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54940-128">Request</span></span>

<span data-ttu-id="54940-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54940-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54940-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="54940-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="54940-131">C#</span><span class="sxs-lookup"><span data-stu-id="54940-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54940-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54940-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54940-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54940-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54940-134">Java</span><span class="sxs-lookup"><span data-stu-id="54940-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-securityaction-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54940-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="54940-135">Response</span></span>

<span data-ttu-id="54940-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54940-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="54940-137">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="54940-137">The response object shown here might be shortened for readability.</span></span>

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


