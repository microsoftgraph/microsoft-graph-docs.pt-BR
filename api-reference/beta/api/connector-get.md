---
title: Obter conector
description: Recupere as propriedades de um objeto connector.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 32bca99004ff59b57729505674d7509ebe23cd73
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047207"
---
# <a name="get-connector"></a><span data-ttu-id="5537e-103">Obter conector</span><span class="sxs-lookup"><span data-stu-id="5537e-103">Get connector</span></span>

<span data-ttu-id="5537e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5537e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5537e-105">Recupere as propriedades e as relações de um [objeto conector.](../resources/connector.md)</span><span class="sxs-lookup"><span data-stu-id="5537e-105">Retrieve the properties and relationships of a [connector](../resources/connector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5537e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5537e-106">Permissions</span></span>
<span data-ttu-id="5537e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5537e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5537e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5537e-109">Permission type</span></span>      | <span data-ttu-id="5537e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5537e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5537e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5537e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5537e-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5537e-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5537e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5537e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5537e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5537e-114">Not supported.</span></span>    |
|<span data-ttu-id="5537e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5537e-115">Application</span></span> | <span data-ttu-id="5537e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5537e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5537e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5537e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5537e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5537e-118">Optional query parameters</span></span>
<span data-ttu-id="5537e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5537e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5537e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5537e-120">Request headers</span></span>
| <span data-ttu-id="5537e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5537e-121">Name</span></span>      |<span data-ttu-id="5537e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5537e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5537e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5537e-123">Authorization</span></span>  | <span data-ttu-id="5537e-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="5537e-124">Bearer.</span></span> <span data-ttu-id="5537e-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="5537e-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="5537e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5537e-126">Request body</span></span>
<span data-ttu-id="5537e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5537e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5537e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5537e-128">Response</span></span>

<span data-ttu-id="5537e-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [conector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5537e-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5537e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5537e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5537e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5537e-131">Request</span></span>

<span data-ttu-id="5537e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5537e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5537e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5537e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="5537e-134">C#</span><span class="sxs-lookup"><span data-stu-id="5537e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5537e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5537e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5537e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5537e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5537e-137">Java</span><span class="sxs-lookup"><span data-stu-id="5537e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connector-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5537e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5537e-138">Response</span></span>
<span data-ttu-id="5537e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5537e-139">The following is an example of the response.</span></span> <span data-ttu-id="5537e-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5537e-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

