---
title: Listar securityActions
description: Recupere uma lista de objetos SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: e19284ad513158914b86318b51c9b244699bfe1a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410391"
---
# <a name="list-securityactions"></a><span data-ttu-id="661bb-103">Listar securityActions</span><span class="sxs-lookup"><span data-stu-id="661bb-103">List securityActions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="661bb-104">Recupere uma lista de [](../resources/securityaction.md) objetos SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="661bb-104">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="661bb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="661bb-105">Permissions</span></span>

<span data-ttu-id="661bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="661bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="661bb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="661bb-108">Permission type</span></span>                        | <span data-ttu-id="661bb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="661bb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="661bb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="661bb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="661bb-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="661bb-111">Not supported.</span></span> |
| <span data-ttu-id="661bb-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="661bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="661bb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="661bb-113">Not supported.</span></span> |
| <span data-ttu-id="661bb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="661bb-114">Application</span></span>                            | <span data-ttu-id="661bb-115">SecurityActions. Read. All, SecurityActions. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="661bb-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="661bb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="661bb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="661bb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="661bb-117">Optional query parameters</span></span>

<span data-ttu-id="661bb-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="661bb-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="661bb-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="661bb-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="661bb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="661bb-120">Request headers</span></span>

| <span data-ttu-id="661bb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="661bb-121">Name</span></span>      |<span data-ttu-id="661bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="661bb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="661bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="661bb-123">Authorization</span></span> | <span data-ttu-id="661bb-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="661bb-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="661bb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="661bb-125">Request body</span></span>

<span data-ttu-id="661bb-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="661bb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="661bb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="661bb-127">Response</span></span>

<span data-ttu-id="661bb-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="661bb-128">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="661bb-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="661bb-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="661bb-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="661bb-130">Request</span></span>

<span data-ttu-id="661bb-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="661bb-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="661bb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="661bb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="661bb-133">C#</span><span class="sxs-lookup"><span data-stu-id="661bb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityactions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="661bb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="661bb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityactions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="661bb-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="661bb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityactions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="661bb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="661bb-136">Response</span></span>

<span data-ttu-id="661bb-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="661bb-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="661bb-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="661bb-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="661bb-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="661bb-139">All the properties will be returned from an actual call.</span></span>

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
