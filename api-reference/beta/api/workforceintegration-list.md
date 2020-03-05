---
title: Listar workforceIntegrations
description: Recupere uma lista de objetos workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7854a2bded54d8480e9423fb8e7e6d6548455430
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451277"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="6ff70-103">Listar workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="6ff70-103">List workforceIntegrations</span></span>

<span data-ttu-id="6ff70-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6ff70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ff70-105">Recupere uma lista de objetos [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="6ff70-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ff70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6ff70-106">Permissions</span></span>

<span data-ttu-id="6ff70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ff70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ff70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ff70-109">Permission type</span></span>                        | <span data-ttu-id="6ff70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6ff70-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6ff70-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ff70-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="6ff70-112">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6ff70-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="6ff70-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ff70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ff70-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ff70-114">Not supported.</span></span> |
| <span data-ttu-id="6ff70-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ff70-115">Application</span></span>                            | <span data-ttu-id="6ff70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ff70-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ff70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ff70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ff70-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6ff70-118">Optional query parameters</span></span>

<span data-ttu-id="6ff70-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6ff70-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6ff70-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6ff70-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ff70-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ff70-121">Request headers</span></span>

| <span data-ttu-id="6ff70-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6ff70-122">Name</span></span>      |<span data-ttu-id="6ff70-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff70-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ff70-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ff70-124">Authorization</span></span> | <span data-ttu-id="6ff70-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ff70-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ff70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ff70-127">Request body</span></span>

<span data-ttu-id="6ff70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ff70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ff70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ff70-129">Response</span></span>

<span data-ttu-id="6ff70-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ff70-130">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6ff70-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6ff70-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6ff70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ff70-132">Request</span></span>

<span data-ttu-id="6ff70-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ff70-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ff70-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ff70-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="6ff70-135">C#</span><span class="sxs-lookup"><span data-stu-id="6ff70-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ff70-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ff70-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ff70-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ff70-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ff70-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ff70-138">Response</span></span>

<span data-ttu-id="6ff70-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6ff70-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6ff70-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ff70-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "apiVersion": 99,
      "encryption": {
        "protocol": "protocol-value",
        "secret": "secret-value"
      },
      "isActive": true,
      "url": "url-value",
      "supports": "supports-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
