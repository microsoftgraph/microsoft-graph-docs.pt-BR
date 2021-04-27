---
title: Listar securityActions
description: Recupere uma lista de objetos securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 45eac647d3bdae27109417e62440478301ebb5a0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051981"
---
# <a name="list-securityactions"></a><span data-ttu-id="94de3-103">Listar securityActions</span><span class="sxs-lookup"><span data-stu-id="94de3-103">List securityActions</span></span>

<span data-ttu-id="94de3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94de3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94de3-105">Recupere uma lista de [objetos securityAction.](../resources/securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="94de3-105">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="94de3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="94de3-106">Permissions</span></span>

<span data-ttu-id="94de3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94de3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94de3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94de3-109">Permission type</span></span>                        | <span data-ttu-id="94de3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94de3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="94de3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94de3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="94de3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94de3-112">Not supported.</span></span> |
| <span data-ttu-id="94de3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94de3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94de3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94de3-114">Not supported.</span></span> |
| <span data-ttu-id="94de3-115">Application</span><span class="sxs-lookup"><span data-stu-id="94de3-115">Application</span></span>                            | <span data-ttu-id="94de3-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94de3-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94de3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94de3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94de3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="94de3-118">Optional query parameters</span></span>

<span data-ttu-id="94de3-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="94de3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="94de3-120">Para obter informações gerais, consulte [Parâmetros de Consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="94de3-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="94de3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94de3-121">Request headers</span></span>

| <span data-ttu-id="94de3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="94de3-122">Name</span></span>      |<span data-ttu-id="94de3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="94de3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94de3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="94de3-124">Authorization</span></span> | <span data-ttu-id="94de3-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="94de3-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="94de3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94de3-126">Request body</span></span>

<span data-ttu-id="94de3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94de3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94de3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="94de3-128">Response</span></span>

<span data-ttu-id="94de3-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos securityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94de3-129">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="94de3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="94de3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="94de3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94de3-131">Request</span></span>

<span data-ttu-id="94de3-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="94de3-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94de3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="94de3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions
```
# <a name="c"></a>[<span data-ttu-id="94de3-134">C#</span><span class="sxs-lookup"><span data-stu-id="94de3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityactions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94de3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94de3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityactions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94de3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94de3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityactions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94de3-137">Java</span><span class="sxs-lookup"><span data-stu-id="94de3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityactions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="94de3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="94de3-138">Response</span></span>

<span data-ttu-id="94de3-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="94de3-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="94de3-140">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="94de3-140">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "actionReason": "actionReason-value",
      "appId": "appId-value",
      "azureTenantId": "azureTenantId-value",
      "clientContext": "clientContext-value",
      "completedDateTime": "datetime-value",
      "createdDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List securityActions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


