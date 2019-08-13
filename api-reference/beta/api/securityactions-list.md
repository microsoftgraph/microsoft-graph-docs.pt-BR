---
title: Listar securityActions
description: Recupere uma lista de objetos SecurityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 02538a80ed8264b4e61bbeff57034d71a9cc011b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364135"
---
# <a name="list-securityactions"></a><span data-ttu-id="a5670-103">Listar securityActions</span><span class="sxs-lookup"><span data-stu-id="a5670-103">List securityActions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5670-104">Recupere uma lista de [](../resources/securityaction.md) objetos SecurityAction.</span><span class="sxs-lookup"><span data-stu-id="a5670-104">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5670-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5670-105">Permissions</span></span>

<span data-ttu-id="a5670-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5670-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5670-108">Permission type</span></span>                        | <span data-ttu-id="a5670-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5670-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5670-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5670-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5670-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5670-111">Not supported.</span></span> |
| <span data-ttu-id="a5670-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5670-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5670-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5670-113">Not supported.</span></span> |
| <span data-ttu-id="a5670-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5670-114">Application</span></span>                            | <span data-ttu-id="a5670-115">SecurityActions. Read. All, SecurityActions. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a5670-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5670-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5670-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5670-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5670-117">Optional query parameters</span></span>

<span data-ttu-id="a5670-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5670-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a5670-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a5670-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5670-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5670-120">Request headers</span></span>

| <span data-ttu-id="a5670-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a5670-121">Name</span></span>      |<span data-ttu-id="a5670-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5670-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5670-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5670-123">Authorization</span></span> | <span data-ttu-id="a5670-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a5670-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5670-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5670-125">Request body</span></span>

<span data-ttu-id="a5670-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5670-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a5670-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5670-127">Response</span></span>

<span data-ttu-id="a5670-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [SecurityAction](../resources/securityaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5670-128">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5670-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5670-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5670-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5670-130">Request</span></span>

<span data-ttu-id="a5670-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5670-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a5670-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5670-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5670-133">C#</span><span class="sxs-lookup"><span data-stu-id="a5670-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityactions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5670-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5670-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityactions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5670-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a5670-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityactions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a5670-136">Java</span><span class="sxs-lookup"><span data-stu-id="a5670-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityactions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5670-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5670-137">Response</span></span>

<span data-ttu-id="a5670-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5670-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a5670-139">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5670-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5670-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5670-140">All the properties will be returned from an actual call.</span></span>

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
