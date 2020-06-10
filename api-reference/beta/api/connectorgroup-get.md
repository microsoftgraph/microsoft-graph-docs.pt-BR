---
title: Obter um conector de conexão
description: Recupere as propriedades de um objeto de conexão.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f6a069bf1b3baafadf46bd3b1ef53abcc84fc79
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681428"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="5dad4-103">Obter um conector de conexão</span><span class="sxs-lookup"><span data-stu-id="5dad4-103">Get connectorGroup</span></span>

<span data-ttu-id="5dad4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dad4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dad4-105">Recupere as propriedades de um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="5dad4-105">Retrieve the properties of a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5dad4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dad4-106">Permissions</span></span>
<span data-ttu-id="5dad4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dad4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dad4-109">Permission type</span></span>      | <span data-ttu-id="5dad4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dad4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dad4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dad4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5dad4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5dad4-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5dad4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dad4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dad4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dad4-114">Not supported.</span></span>    |
|<span data-ttu-id="5dad4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dad4-115">Application</span></span> | <span data-ttu-id="5dad4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dad4-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5dad4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dad4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5dad4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5dad4-118">Optional query parameters</span></span>
<span data-ttu-id="5dad4-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5dad4-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dad4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dad4-120">Request headers</span></span>
| <span data-ttu-id="5dad4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5dad4-121">Name</span></span>      |<span data-ttu-id="5dad4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dad4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5dad4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dad4-123">Authorization</span></span>  | <span data-ttu-id="5dad4-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="5dad4-124">Bearer.</span></span> <span data-ttu-id="5dad4-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="5dad4-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dad4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dad4-126">Request body</span></span>
<span data-ttu-id="5dad4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5dad4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dad4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dad4-128">Response</span></span>

<span data-ttu-id="5dad4-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto de [teleconnector](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dad4-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dad4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dad4-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5dad4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dad4-131">Request</span></span>
<span data-ttu-id="5dad4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dad4-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5dad4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5dad4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="5dad4-134">C#</span><span class="sxs-lookup"><span data-stu-id="5dad4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5dad4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5dad4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5dad4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5dad4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5dad4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dad4-137">Response</span></span>
<span data-ttu-id="5dad4-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5dad4-138">The following is an example of the response.</span></span> <span data-ttu-id="5dad4-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="5dad4-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5dad4-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dad4-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
