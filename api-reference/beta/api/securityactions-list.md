---
title: Listar securityActions
description: Recupere uma lista de objetos SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 5f48f75ea88aca81dc780b2c09d139cff9fea683
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970924"
---
# <a name="list-securityactions"></a><span data-ttu-id="792de-103">Listar securityActions</span><span class="sxs-lookup"><span data-stu-id="792de-103">List securityActions</span></span>

<span data-ttu-id="792de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="792de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="792de-105">Recupere uma lista de objetos [SecurityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="792de-105">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="792de-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="792de-106">Permissions</span></span>

<span data-ttu-id="792de-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="792de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="792de-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="792de-109">Permission type</span></span>                        | <span data-ttu-id="792de-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="792de-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="792de-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="792de-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="792de-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="792de-112">Not supported.</span></span> |
| <span data-ttu-id="792de-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="792de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="792de-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="792de-114">Not supported.</span></span> |
| <span data-ttu-id="792de-115">Application</span><span class="sxs-lookup"><span data-stu-id="792de-115">Application</span></span>                            | <span data-ttu-id="792de-116">SecurityActions. Read. All, SecurityActions. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="792de-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="792de-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="792de-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="792de-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="792de-118">Optional query parameters</span></span>

<span data-ttu-id="792de-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="792de-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="792de-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="792de-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="792de-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="792de-121">Request headers</span></span>

| <span data-ttu-id="792de-122">Nome</span><span class="sxs-lookup"><span data-stu-id="792de-122">Name</span></span>      |<span data-ttu-id="792de-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="792de-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="792de-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="792de-124">Authorization</span></span> | <span data-ttu-id="792de-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="792de-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="792de-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="792de-126">Request body</span></span>

<span data-ttu-id="792de-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="792de-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="792de-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="792de-128">Response</span></span>

<span data-ttu-id="792de-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="792de-129">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="792de-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="792de-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="792de-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="792de-131">Request</span></span>

<span data-ttu-id="792de-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="792de-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="792de-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="792de-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions
```
# <a name="c"></a>[<span data-ttu-id="792de-134">C#</span><span class="sxs-lookup"><span data-stu-id="792de-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityactions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="792de-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="792de-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityactions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="792de-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="792de-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityactions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="792de-137">Java</span><span class="sxs-lookup"><span data-stu-id="792de-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityactions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="792de-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="792de-138">Response</span></span>

<span data-ttu-id="792de-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="792de-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="792de-140">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="792de-140">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="792de-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="792de-141">All the properties will be returned from an actual call.</span></span>

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


