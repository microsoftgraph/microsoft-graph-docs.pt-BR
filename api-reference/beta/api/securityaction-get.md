---
title: Obter securityAction
description: Recupere as propriedades e as relações do objeto securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 328a54bb73517611b3fc96603601309cbb1a7ea7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050868"
---
# <a name="get-securityaction"></a><span data-ttu-id="57bdd-103">Obter securityAction</span><span class="sxs-lookup"><span data-stu-id="57bdd-103">Get securityAction</span></span>

<span data-ttu-id="57bdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57bdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57bdd-105">Recupere as propriedades e as relações de um [objeto securityAction.](../resources/securityaction.md)</span><span class="sxs-lookup"><span data-stu-id="57bdd-105">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57bdd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="57bdd-106">Permissions</span></span>

<span data-ttu-id="57bdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57bdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57bdd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57bdd-109">Permission type</span></span>                        | <span data-ttu-id="57bdd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57bdd-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57bdd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57bdd-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="57bdd-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57bdd-112">Not supported.</span></span> |
| <span data-ttu-id="57bdd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57bdd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57bdd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57bdd-114">Not supported.</span></span> |
| <span data-ttu-id="57bdd-115">Application</span><span class="sxs-lookup"><span data-stu-id="57bdd-115">Application</span></span>                            | <span data-ttu-id="57bdd-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57bdd-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57bdd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57bdd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57bdd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="57bdd-118">Optional query parameters</span></span>

<span data-ttu-id="57bdd-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57bdd-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="57bdd-120">Para obter informações gerais, consulte [Parâmetros de Consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="57bdd-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="57bdd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57bdd-121">Request headers</span></span>

| <span data-ttu-id="57bdd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="57bdd-122">Name</span></span>      |<span data-ttu-id="57bdd-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="57bdd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57bdd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="57bdd-124">Authorization</span></span> | <span data-ttu-id="57bdd-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="57bdd-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="57bdd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57bdd-126">Request body</span></span>

<span data-ttu-id="57bdd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57bdd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57bdd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="57bdd-128">Response</span></span>

<span data-ttu-id="57bdd-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [securityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57bdd-129">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57bdd-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="57bdd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57bdd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57bdd-131">Request</span></span>

<span data-ttu-id="57bdd-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="57bdd-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57bdd-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="57bdd-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```
# <a name="c"></a>[<span data-ttu-id="57bdd-134">C#</span><span class="sxs-lookup"><span data-stu-id="57bdd-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57bdd-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57bdd-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57bdd-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57bdd-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57bdd-137">Java</span><span class="sxs-lookup"><span data-stu-id="57bdd-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57bdd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="57bdd-138">Response</span></span>

<span data-ttu-id="57bdd-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="57bdd-139">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="57bdd-140">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="57bdd-140">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


