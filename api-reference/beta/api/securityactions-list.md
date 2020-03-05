---
title: Listar securityActions
description: Recupere uma lista de objetos SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 1634f2bd678ebfa20cc24e948ef86faf95981623
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453596"
---
# <a name="list-securityactions"></a><span data-ttu-id="aa2c9-103">Listar securityActions</span><span class="sxs-lookup"><span data-stu-id="aa2c9-103">List securityActions</span></span>

<span data-ttu-id="aa2c9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aa2c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa2c9-105">Recupere uma lista de objetos [SecurityAction](../resources/securityaction.md) .</span><span class="sxs-lookup"><span data-stu-id="aa2c9-105">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa2c9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa2c9-106">Permissions</span></span>

<span data-ttu-id="aa2c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa2c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aa2c9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa2c9-109">Permission type</span></span>                        | <span data-ttu-id="aa2c9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa2c9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aa2c9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa2c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="aa2c9-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-112">Not supported.</span></span> |
| <span data-ttu-id="aa2c9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa2c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa2c9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-114">Not supported.</span></span> |
| <span data-ttu-id="aa2c9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa2c9-115">Application</span></span>                            | <span data-ttu-id="aa2c9-116">SecurityActions. Read. All, SecurityActions. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="aa2c9-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa2c9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa2c9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa2c9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa2c9-118">Optional query parameters</span></span>

<span data-ttu-id="aa2c9-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="aa2c9-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="aa2c9-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa2c9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa2c9-121">Request headers</span></span>

| <span data-ttu-id="aa2c9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="aa2c9-122">Name</span></span>      |<span data-ttu-id="aa2c9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa2c9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aa2c9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa2c9-124">Authorization</span></span> | <span data-ttu-id="aa2c9-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="aa2c9-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa2c9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa2c9-126">Request body</span></span>

<span data-ttu-id="aa2c9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa2c9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa2c9-128">Response</span></span>

<span data-ttu-id="aa2c9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-129">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aa2c9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="aa2c9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="aa2c9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa2c9-131">Request</span></span>

<span data-ttu-id="aa2c9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa2c9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa2c9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions
```
# <a name="c"></a>[<span data-ttu-id="aa2c9-134">C#</span><span class="sxs-lookup"><span data-stu-id="aa2c9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityactions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa2c9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa2c9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityactions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa2c9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa2c9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityactions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="aa2c9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa2c9-137">Response</span></span>

<span data-ttu-id="aa2c9-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="aa2c9-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aa2c9-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa2c9-140">All the properties will be returned from an actual call.</span></span>

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
