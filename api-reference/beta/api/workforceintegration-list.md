---
title: Listar workforceIntegrations
description: Recupere uma lista de objetos workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aea3aea8181d83e1cb04be3578ef0b88d8829c15
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870570"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="3e0dc-103">Listar workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="3e0dc-103">List workforceIntegrations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e0dc-104">Recupere uma lista de objetos [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="3e0dc-104">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e0dc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3e0dc-105">Permissions</span></span>

<span data-ttu-id="3e0dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e0dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e0dc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3e0dc-108">Permission type</span></span>                        | <span data-ttu-id="3e0dc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3e0dc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e0dc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3e0dc-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="3e0dc-111">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3e0dc-111">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="3e0dc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3e0dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e0dc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-113">Not supported.</span></span> |
| <span data-ttu-id="3e0dc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3e0dc-114">Application</span></span>                            | <span data-ttu-id="3e0dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e0dc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e0dc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e0dc-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3e0dc-117">Optional query parameters</span></span>

<span data-ttu-id="3e0dc-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3e0dc-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3e0dc-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e0dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0dc-120">Request headers</span></span>

| <span data-ttu-id="3e0dc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3e0dc-121">Name</span></span>      |<span data-ttu-id="3e0dc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e0dc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e0dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e0dc-123">Authorization</span></span> | <span data-ttu-id="3e0dc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e0dc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0dc-126">Request body</span></span>

<span data-ttu-id="3e0dc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e0dc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e0dc-128">Response</span></span>

<span data-ttu-id="3e0dc-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-129">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e0dc-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3e0dc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e0dc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e0dc-131">Request</span></span>

<span data-ttu-id="3e0dc-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3e0dc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e0dc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3e0dc-134">C#</span><span class="sxs-lookup"><span data-stu-id="3e0dc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e0dc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e0dc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3e0dc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e0dc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e0dc-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e0dc-137">Response</span></span>

<span data-ttu-id="3e0dc-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-138">The following is an example of the response.</span></span>

> <span data-ttu-id="3e0dc-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e0dc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
