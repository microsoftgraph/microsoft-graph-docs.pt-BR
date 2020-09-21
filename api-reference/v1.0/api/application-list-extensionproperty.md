---
title: List extensionproperties
description: Recupere uma lista de objetos extensionproperty.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c6b8445f0cbcc36046bb71572014756c992c3fe6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966490"
---
# <a name="list-extensionproperties"></a><span data-ttu-id="60f3a-103">List extensionproperties</span><span class="sxs-lookup"><span data-stu-id="60f3a-103">List extensionProperties</span></span>

<span data-ttu-id="60f3a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60f3a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60f3a-105">Recupere a lista de objetos [extensionproperty](../resources/extensionproperty.md) em um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="60f3a-105">Retrieve the list of [extensionProperty](../resources/extensionproperty.md) objects on an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="60f3a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="60f3a-106">Permissions</span></span>

<span data-ttu-id="60f3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60f3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60f3a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60f3a-109">Permission type</span></span>      | <span data-ttu-id="60f3a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60f3a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60f3a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60f3a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="60f3a-112">Application. Read. All, Application. ReadWrite. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="60f3a-112">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |
|<span data-ttu-id="60f3a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60f3a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60f3a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60f3a-114">Not supported.</span></span>    |
|<span data-ttu-id="60f3a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60f3a-115">Application</span></span> | <span data-ttu-id="60f3a-116">Application. Read. All, Application. ReadWrite. All, Directory. Read. All</span><span class="sxs-lookup"><span data-stu-id="60f3a-116">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60f3a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60f3a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/extensionProperties
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60f3a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="60f3a-118">Optional query parameters</span></span>

<span data-ttu-id="60f3a-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="60f3a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="60f3a-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="60f3a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="60f3a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60f3a-121">Request headers</span></span>

| <span data-ttu-id="60f3a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="60f3a-122">Name</span></span>       | <span data-ttu-id="60f3a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="60f3a-123">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="60f3a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="60f3a-124">Authorization</span></span>  | <span data-ttu-id="60f3a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60f3a-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="60f3a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60f3a-127">Request body</span></span>

<span data-ttu-id="60f3a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60f3a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60f3a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f3a-129">Response</span></span>

<span data-ttu-id="60f3a-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [extensionproperty](../resources/extensionproperty.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="60f3a-130">If successful, this method returns a `200 OK` response code and a collection of [extensionProperty](../resources/extensionproperty.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="60f3a-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="60f3a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="60f3a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60f3a-132">Request</span></span>

<span data-ttu-id="60f3a-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60f3a-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60f3a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="60f3a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_extensionproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
```
# <a name="c"></a>[<span data-ttu-id="60f3a-135">C#</span><span class="sxs-lookup"><span data-stu-id="60f3a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-extensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60f3a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60f3a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-extensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60f3a-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60f3a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-extensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60f3a-138">Java</span><span class="sxs-lookup"><span data-stu-id="60f3a-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-extensionproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="60f3a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="60f3a-139">Response</span></span>

<span data-ttu-id="60f3a-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60f3a-140">The following is an example of the response.</span></span>

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

