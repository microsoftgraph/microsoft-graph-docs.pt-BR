---
title: Obter conector
description: Recupere as propriedades de um objeto connector.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b978663f17e4aa17a5599b055633ff4eb2622c80
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947175"
---
# <a name="get-connector"></a><span data-ttu-id="3ca61-103">Obter conector</span><span class="sxs-lookup"><span data-stu-id="3ca61-103">Get connector</span></span>

<span data-ttu-id="3ca61-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ca61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ca61-105">Recupere as propriedades e as relações de um [objeto conector.](../resources/connector.md)</span><span class="sxs-lookup"><span data-stu-id="3ca61-105">Retrieve the properties and relationships of a [connector](../resources/connector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ca61-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ca61-106">Permissions</span></span>
<span data-ttu-id="3ca61-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ca61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ca61-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ca61-109">Permission type</span></span>      | <span data-ttu-id="3ca61-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ca61-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ca61-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ca61-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ca61-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ca61-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ca61-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ca61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ca61-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ca61-114">Not supported.</span></span>    |
|<span data-ttu-id="3ca61-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ca61-115">Application</span></span> | <span data-ttu-id="3ca61-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ca61-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3ca61-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ca61-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ca61-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ca61-118">Optional query parameters</span></span>
<span data-ttu-id="3ca61-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3ca61-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ca61-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ca61-120">Request headers</span></span>
| <span data-ttu-id="3ca61-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3ca61-121">Name</span></span>      |<span data-ttu-id="3ca61-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ca61-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ca61-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ca61-123">Authorization</span></span>  | <span data-ttu-id="3ca61-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="3ca61-124">Bearer.</span></span> <span data-ttu-id="3ca61-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="3ca61-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ca61-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ca61-126">Request body</span></span>
<span data-ttu-id="3ca61-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ca61-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ca61-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ca61-128">Response</span></span>

<span data-ttu-id="3ca61-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [conector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ca61-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ca61-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ca61-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ca61-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ca61-131">Request</span></span>

<span data-ttu-id="3ca61-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ca61-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ca61-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ca61-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="3ca61-134">C#</span><span class="sxs-lookup"><span data-stu-id="3ca61-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ca61-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ca61-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ca61-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ca61-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3ca61-137">Java</span><span class="sxs-lookup"><span data-stu-id="3ca61-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connector-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3ca61-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ca61-138">Response</span></span>
<span data-ttu-id="3ca61-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ca61-139">The following is an example of the response.</span></span> <span data-ttu-id="3ca61-140">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3ca61-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3ca61-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ca61-141">All of the properties will be returned from an actual call.</span></span>
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

