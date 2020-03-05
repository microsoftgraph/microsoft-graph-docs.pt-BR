---
title: Obter securityAction
description: Recupere as propriedades e os relacionamentos do objeto SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 206f0384fe3c592ca1daf67c0d401eb16b7aed16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453573"
---
# <a name="get-securityaction"></a><span data-ttu-id="05be3-103">Obter securityAction</span><span class="sxs-lookup"><span data-stu-id="05be3-103">Get securityAction</span></span>

<span data-ttu-id="05be3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="05be3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05be3-105">Recupere as propriedades e os relacionamentos de um objeto [SecurityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="05be3-105">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="05be3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="05be3-106">Permissions</span></span>

<span data-ttu-id="05be3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05be3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="05be3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="05be3-109">Permission type</span></span>                        | <span data-ttu-id="05be3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="05be3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="05be3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="05be3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="05be3-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05be3-112">Not supported.</span></span> |
| <span data-ttu-id="05be3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="05be3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05be3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="05be3-114">Not supported.</span></span> |
| <span data-ttu-id="05be3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="05be3-115">Application</span></span>                            | <span data-ttu-id="05be3-116">SecurityActions. Read. All, SecurityActions. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="05be3-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05be3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="05be3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="05be3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="05be3-118">Optional query parameters</span></span>

<span data-ttu-id="05be3-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="05be3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="05be3-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="05be3-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="05be3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="05be3-121">Request headers</span></span>

| <span data-ttu-id="05be3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="05be3-122">Name</span></span>      |<span data-ttu-id="05be3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="05be3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05be3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="05be3-124">Authorization</span></span> | <span data-ttu-id="05be3-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="05be3-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="05be3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="05be3-126">Request body</span></span>

<span data-ttu-id="05be3-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="05be3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05be3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="05be3-128">Response</span></span>

<span data-ttu-id="05be3-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="05be3-129">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="05be3-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="05be3-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05be3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="05be3-131">Request</span></span>

<span data-ttu-id="05be3-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="05be3-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05be3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="05be3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```
# <a name="c"></a>[<span data-ttu-id="05be3-134">C#</span><span class="sxs-lookup"><span data-stu-id="05be3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05be3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05be3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05be3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05be3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05be3-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="05be3-137">Response</span></span>

<span data-ttu-id="05be3-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="05be3-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="05be3-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="05be3-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="05be3-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="05be3-140">All the properties will be returned from an actual call.</span></span>

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
