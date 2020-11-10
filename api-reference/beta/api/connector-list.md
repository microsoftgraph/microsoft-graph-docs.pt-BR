---
title: Listar conectores
description: Recupere uma lista de objetos Connector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b72968bc9404e0936219cb96dfd33467784024e0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957460"
---
# <a name="list-connectors"></a><span data-ttu-id="7cd13-103">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="7cd13-103">List connectors</span></span>

<span data-ttu-id="7cd13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cd13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cd13-105">Recupere uma lista de objetos [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="7cd13-105">Retrieve a list of [connector](../resources/connector.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cd13-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7cd13-106">Permissions</span></span>
<span data-ttu-id="7cd13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cd13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cd13-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cd13-109">Permission type</span></span>      | <span data-ttu-id="7cd13-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cd13-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cd13-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cd13-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7cd13-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7cd13-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7cd13-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cd13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cd13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cd13-114">Not supported.</span></span>    |
|<span data-ttu-id="7cd13-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cd13-115">Application</span></span> | <span data-ttu-id="7cd13-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cd13-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cd13-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cd13-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7cd13-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7cd13-118">Optional query parameters</span></span>
<span data-ttu-id="7cd13-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7cd13-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7cd13-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd13-120">Request headers</span></span>
| <span data-ttu-id="7cd13-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7cd13-121">Name</span></span>      |<span data-ttu-id="7cd13-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cd13-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7cd13-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cd13-123">Authorization</span></span>  | <span data-ttu-id="7cd13-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="7cd13-124">Bearer.</span></span> <span data-ttu-id="7cd13-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="7cd13-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cd13-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd13-126">Request body</span></span>
<span data-ttu-id="7cd13-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7cd13-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cd13-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd13-128">Response</span></span>

<span data-ttu-id="7cd13-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cd13-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cd13-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cd13-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7cd13-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd13-131">Request</span></span>
<span data-ttu-id="7cd13-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cd13-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7cd13-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cd13-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors
```
# <a name="c"></a>[<span data-ttu-id="7cd13-134">C#</span><span class="sxs-lookup"><span data-stu-id="7cd13-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cd13-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cd13-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cd13-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cd13-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cd13-137">Java</span><span class="sxs-lookup"><span data-stu-id="7cd13-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7cd13-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd13-138">Response</span></span>
<span data-ttu-id="7cd13-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7cd13-139">The following is an example of the response.</span></span> <span data-ttu-id="7cd13-140">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7cd13-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7cd13-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cd13-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
