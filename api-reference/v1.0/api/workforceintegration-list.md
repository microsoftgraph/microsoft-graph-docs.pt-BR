---
title: Listar workforceIntegrations
description: Recupere uma lista de objetos workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: eb019555d012a9373b21571291687a703beb5b8e
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848203"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="36eb6-103">Listar workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="36eb6-103">List workforceIntegrations</span></span>

<span data-ttu-id="36eb6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36eb6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36eb6-105">Recupere uma lista de objetos [workforceIntegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="36eb6-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="36eb6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36eb6-106">Permissions</span></span>

<span data-ttu-id="36eb6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36eb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36eb6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36eb6-109">Permission type</span></span>                        | <span data-ttu-id="36eb6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36eb6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36eb6-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36eb6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36eb6-112">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="36eb6-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="36eb6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36eb6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36eb6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36eb6-114">Not supported.</span></span> |
| <span data-ttu-id="36eb6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36eb6-115">Application</span></span>                            | <span data-ttu-id="36eb6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36eb6-116">Not supported.</span></span> |

> <span data-ttu-id="36eb6-117">**Observação** : esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="36eb6-117">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="36eb6-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="36eb6-118">Global admins can access groups that they are not a member of.</span></span>


## <a name="http-request"></a><span data-ttu-id="36eb6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36eb6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36eb6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36eb6-120">Optional query parameters</span></span>

<span data-ttu-id="36eb6-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36eb6-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="36eb6-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="36eb6-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="36eb6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36eb6-123">Request headers</span></span>

| <span data-ttu-id="36eb6-124">Nome</span><span class="sxs-lookup"><span data-stu-id="36eb6-124">Name</span></span>      |<span data-ttu-id="36eb6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="36eb6-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36eb6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="36eb6-126">Authorization</span></span> | <span data-ttu-id="36eb6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36eb6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36eb6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36eb6-129">Request body</span></span>

<span data-ttu-id="36eb6-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36eb6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36eb6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="36eb6-131">Response</span></span>

<span data-ttu-id="36eb6-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [workforceIntegration](../resources/workforceintegration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36eb6-132">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="36eb6-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="36eb6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36eb6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36eb6-134">Request</span></span>

<span data-ttu-id="36eb6-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="36eb6-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36eb6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="36eb6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="36eb6-137">C#</span><span class="sxs-lookup"><span data-stu-id="36eb6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36eb6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36eb6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36eb6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36eb6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36eb6-140">Java</span><span class="sxs-lookup"><span data-stu-id="36eb6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-workforceintegrations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="36eb6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="36eb6-141">Response</span></span>

<span data-ttu-id="36eb6-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="36eb6-142">The following is an example of the response.</span></span>

> <span data-ttu-id="36eb6-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36eb6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

