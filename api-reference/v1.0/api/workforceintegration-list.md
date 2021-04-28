---
title: Listar workforceIntegrations
description: Recuperar uma lista de objetos workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d96aa5dcf131724fbd231ed7574606bd1b736d21
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031484"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="fa8f3-103">Listar workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="fa8f3-103">List workforceIntegrations</span></span>

<span data-ttu-id="fa8f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa8f3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa8f3-105">Recuperar uma lista de [objetos workforceIntegration.](../resources/workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="fa8f3-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa8f3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa8f3-106">Permissions</span></span>

<span data-ttu-id="fa8f3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa8f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa8f3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa8f3-109">Permission type</span></span>                        | <span data-ttu-id="fa8f3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa8f3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fa8f3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa8f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa8f3-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa8f3-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="fa8f3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa8f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa8f3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-114">Not supported.</span></span> |
| <span data-ttu-id="fa8f3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa8f3-115">Application</span></span>                            | <span data-ttu-id="fa8f3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-116">Not supported.</span></span> |

> <span data-ttu-id="fa8f3-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="fa8f3-118">Os administradores globais podem acessar grupos dos que não são membros.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="fa8f3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa8f3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa8f3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa8f3-120">Optional query parameters</span></span>

<span data-ttu-id="fa8f3-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fa8f3-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fa8f3-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa8f3-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa8f3-123">Request headers</span></span>

| <span data-ttu-id="fa8f3-124">Nome</span><span class="sxs-lookup"><span data-stu-id="fa8f3-124">Name</span></span>      |<span data-ttu-id="fa8f3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa8f3-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa8f3-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa8f3-126">Authorization</span></span> | <span data-ttu-id="fa8f3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa8f3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa8f3-129">Request body</span></span>

<span data-ttu-id="fa8f3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa8f3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa8f3-131">Response</span></span>

<span data-ttu-id="fa8f3-132">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-132">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa8f3-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa8f3-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fa8f3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa8f3-134">Request</span></span>

<span data-ttu-id="fa8f3-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fa8f3-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa8f3-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="fa8f3-137">C#</span><span class="sxs-lookup"><span data-stu-id="fa8f3-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa8f3-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa8f3-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa8f3-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa8f3-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa8f3-140">Java</span><span class="sxs-lookup"><span data-stu-id="fa8f3-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegrations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="fa8f3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa8f3-141">Response</span></span>

<span data-ttu-id="fa8f3-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-142">The following is an example of the response.</span></span>

> <span data-ttu-id="fa8f3-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fa8f3-143">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "supportedEntities": "supportedEntities-value"
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

