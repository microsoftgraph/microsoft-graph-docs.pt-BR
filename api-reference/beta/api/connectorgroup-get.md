---
title: Obter connectorGroup
description: Recupere as propriedades de um objeto de conexão.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ba4879e4c951f53303a7d4282cd5a2ac328887fc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957411"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="28c42-103">Obter connectorGroup</span><span class="sxs-lookup"><span data-stu-id="28c42-103">Get connectorGroup</span></span>

<span data-ttu-id="28c42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28c42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28c42-105">Recupere as propriedades de um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="28c42-105">Retrieve the properties of a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28c42-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="28c42-106">Permissions</span></span>
<span data-ttu-id="28c42-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28c42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28c42-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28c42-109">Permission type</span></span>      | <span data-ttu-id="28c42-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28c42-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28c42-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28c42-111">Delegated (work or school account)</span></span> | <span data-ttu-id="28c42-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28c42-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28c42-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28c42-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28c42-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28c42-114">Not supported.</span></span>    |
|<span data-ttu-id="28c42-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28c42-115">Application</span></span> | <span data-ttu-id="28c42-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28c42-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="28c42-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28c42-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28c42-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28c42-118">Optional query parameters</span></span>
<span data-ttu-id="28c42-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28c42-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28c42-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28c42-120">Request headers</span></span>
| <span data-ttu-id="28c42-121">Nome</span><span class="sxs-lookup"><span data-stu-id="28c42-121">Name</span></span>      |<span data-ttu-id="28c42-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="28c42-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28c42-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="28c42-123">Authorization</span></span>  | <span data-ttu-id="28c42-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="28c42-124">Bearer.</span></span> <span data-ttu-id="28c42-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="28c42-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="28c42-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28c42-126">Request body</span></span>
<span data-ttu-id="28c42-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28c42-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28c42-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c42-128">Response</span></span>

<span data-ttu-id="28c42-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto de [teleconnector](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28c42-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28c42-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28c42-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="28c42-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28c42-131">Request</span></span>
<span data-ttu-id="28c42-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28c42-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28c42-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="28c42-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="28c42-134">C#</span><span class="sxs-lookup"><span data-stu-id="28c42-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28c42-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28c42-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28c42-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28c42-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28c42-137">Java</span><span class="sxs-lookup"><span data-stu-id="28c42-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28c42-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="28c42-138">Response</span></span>
<span data-ttu-id="28c42-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28c42-139">The following is an example of the response.</span></span> <span data-ttu-id="28c42-140">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="28c42-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="28c42-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28c42-141">All of the properties will be returned from an actual call.</span></span>
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
