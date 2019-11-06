---
title: List extensionproperties
description: Recupere uma lista de objetos extensionproperty.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ff2f9d1c47d00d03ebafb7b777269b30f017f496
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006421"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="bfbbd-103">List extensionproperties</span><span class="sxs-lookup"><span data-stu-id="bfbbd-103">List extensionProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfbbd-104">Recupere a lista de objetos [extensionproperty](../resources/extensionproperty.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfbbd-104">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfbbd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bfbbd-105">Permissions</span></span>

<span data-ttu-id="bfbbd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfbbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfbbd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfbbd-108">Permission type</span></span>      | <span data-ttu-id="bfbbd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfbbd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfbbd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfbbd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bfbbd-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bfbbd-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bfbbd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfbbd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfbbd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfbbd-113">Not supported.</span></span>    |
|<span data-ttu-id="bfbbd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfbbd-114">Application</span></span> | <span data-ttu-id="bfbbd-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="bfbbd-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfbbd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfbbd-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bfbbd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="bfbbd-117">Optional query parameters</span></span>

<span data-ttu-id="bfbbd-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="bfbbd-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bfbbd-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bfbbd-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfbbd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbbd-120">Request headers</span></span>

| <span data-ttu-id="bfbbd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="bfbbd-121">Name</span></span>       | <span data-ttu-id="bfbbd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfbbd-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="bfbbd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfbbd-123">Authorization</span></span>  | <span data-ttu-id="bfbbd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfbbd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bfbbd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbbd-126">Request body</span></span>

<span data-ttu-id="bfbbd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bfbbd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfbbd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfbbd-128">Response</span></span>

<span data-ttu-id="bfbbd-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [extensionproperty](../resources/extensionproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfbbd-129">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bfbbd-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bfbbd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bfbbd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfbbd-131">Request</span></span>

<span data-ttu-id="bfbbd-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfbbd-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bfbbd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfbbd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/extensionProperties
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bfbbd-134">C#</span><span class="sxs-lookup"><span data-stu-id="bfbbd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bfbbd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfbbd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bfbbd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfbbd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bfbbd-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfbbd-137">Response</span></span>

<span data-ttu-id="bfbbd-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bfbbd-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
            "deletedDateTime": null,
            "appDisplayName": "Display name",
            "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
            "dataType": "String",
            "isSyncedFromOnPremises": false,
            "targetObjects": [
                "Application"
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List extensionProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->