---
title: Obter workforceIntegration
description: Recupere as propriedades e os relacionamentos do objeto workforceintegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 378ec619584b4b6dba67871bd927a0d6852feda8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451292"
---
# <a name="get-workforceintegration"></a><span data-ttu-id="78b9a-103">Obter workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="78b9a-103">Get workforceIntegration</span></span>

<span data-ttu-id="78b9a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="78b9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78b9a-105">Recupere as propriedades e os relacionamentos de um objeto [workforceintegration](../resources/workforceintegration.md) .</span><span class="sxs-lookup"><span data-stu-id="78b9a-105">Retrieve the properties and relationships of a [workforceintegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="78b9a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="78b9a-106">Permissions</span></span>

<span data-ttu-id="78b9a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78b9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="78b9a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78b9a-109">Permission type</span></span>                        | <span data-ttu-id="78b9a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78b9a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="78b9a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78b9a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="78b9a-112">WorkforceIntegration. Read. All, WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="78b9a-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="78b9a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78b9a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78b9a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78b9a-114">Not supported.</span></span> |
| <span data-ttu-id="78b9a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78b9a-115">Application</span></span>                            | <span data-ttu-id="78b9a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78b9a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78b9a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78b9a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78b9a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78b9a-118">Optional query parameters</span></span>

<span data-ttu-id="78b9a-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78b9a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="78b9a-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="78b9a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="78b9a-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78b9a-121">Request headers</span></span>

| <span data-ttu-id="78b9a-122">Nome</span><span class="sxs-lookup"><span data-stu-id="78b9a-122">Name</span></span>      |<span data-ttu-id="78b9a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="78b9a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78b9a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="78b9a-124">Authorization</span></span> | <span data-ttu-id="78b9a-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="78b9a-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="78b9a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78b9a-126">Request body</span></span>

<span data-ttu-id="78b9a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78b9a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78b9a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="78b9a-128">Response</span></span>

<span data-ttu-id="78b9a-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [workforceIntegration](../resources/workforceintegration.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78b9a-129">If successful, this method returns a `200 OK` response code and the requested [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78b9a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="78b9a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78b9a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78b9a-131">Request</span></span>

<span data-ttu-id="78b9a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="78b9a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="78b9a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="78b9a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceintegrationid}
```
# <a name="c"></a>[<span data-ttu-id="78b9a-134">C#</span><span class="sxs-lookup"><span data-stu-id="78b9a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78b9a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78b9a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78b9a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78b9a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="78b9a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="78b9a-137">Response</span></span>

<span data-ttu-id="78b9a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="78b9a-138">The following is an example of the response.</span></span>

> <span data-ttu-id="78b9a-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78b9a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "displayName": "KronosWorkforceIntegration",
  "apiVersion": 1,
  "isActive": true,
  "encryption": {
    "protocol": "sharedSecret",
    "secret": null
  },
  "url": "https://contosoWorkforceIntegration.com/Contoso/",
  "supports": "shift"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
