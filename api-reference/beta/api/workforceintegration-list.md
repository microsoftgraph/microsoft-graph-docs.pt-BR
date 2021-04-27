---
title: Listar workforceIntegrations
description: Recuperar uma lista de objetos workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e28e40ec75833cde86d80cca26ea4d0a423ff018
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054697"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="fafe8-103">Listar workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="fafe8-103">List workforceIntegrations</span></span>

<span data-ttu-id="fafe8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fafe8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fafe8-105">Recuperar uma lista de [objetos workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="fafe8-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fafe8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fafe8-106">Permissions</span></span>

<span data-ttu-id="fafe8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fafe8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fafe8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fafe8-109">Permission type</span></span>                        | <span data-ttu-id="fafe8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fafe8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fafe8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fafe8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fafe8-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fafe8-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="fafe8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fafe8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fafe8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fafe8-114">Not supported.</span></span> |
| <span data-ttu-id="fafe8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fafe8-115">Application</span></span>                            | <span data-ttu-id="fafe8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fafe8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fafe8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fafe8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fafe8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fafe8-118">Optional query parameters</span></span>

<span data-ttu-id="fafe8-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fafe8-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fafe8-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fafe8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fafe8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fafe8-121">Request headers</span></span>

| <span data-ttu-id="fafe8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fafe8-122">Name</span></span>      |<span data-ttu-id="fafe8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fafe8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fafe8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="fafe8-124">Authorization</span></span> | <span data-ttu-id="fafe8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fafe8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fafe8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fafe8-127">Request body</span></span>

<span data-ttu-id="fafe8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fafe8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fafe8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fafe8-129">Response</span></span>

<span data-ttu-id="fafe8-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fafe8-130">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fafe8-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fafe8-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fafe8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fafe8-132">Request</span></span>

<span data-ttu-id="fafe8-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fafe8-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fafe8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fafe8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="fafe8-135">C#</span><span class="sxs-lookup"><span data-stu-id="fafe8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fafe8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fafe8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fafe8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fafe8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fafe8-138">Java</span><span class="sxs-lookup"><span data-stu-id="fafe8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegrations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fafe8-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fafe8-139">Response</span></span>

<span data-ttu-id="fafe8-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fafe8-140">The following is an example of the response.</span></span>

> <span data-ttu-id="fafe8-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fafe8-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


