---
title: Listar connectorGroups
description: Recupere uma lista de objetos connectorgroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7d8ad142840abba411fb6f2c3b9f0f49c55acd56
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130098"
---
# <a name="list-connectorgroups"></a><span data-ttu-id="b3274-103">Listar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="b3274-103">List connectorGroups</span></span>

<span data-ttu-id="b3274-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3274-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3274-105">Recupere uma lista de [objetos connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b3274-105">Retrieve a list of [connectorGroup](../resources/connectorgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3274-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3274-106">Permissions</span></span>
<span data-ttu-id="b3274-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3274-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3274-109">Permission type</span></span>      | <span data-ttu-id="b3274-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3274-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3274-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3274-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3274-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3274-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3274-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3274-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3274-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3274-114">Not supported.</span></span>    |
|<span data-ttu-id="b3274-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3274-115">Application</span></span> | <span data-ttu-id="b3274-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3274-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3274-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3274-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3274-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3274-118">Optional query parameters</span></span>
<span data-ttu-id="b3274-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3274-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3274-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3274-120">Request headers</span></span>
| <span data-ttu-id="b3274-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b3274-121">Name</span></span>      |<span data-ttu-id="b3274-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3274-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3274-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3274-123">Authorization</span></span>  | <span data-ttu-id="b3274-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="b3274-124">Bearer.</span></span> <span data-ttu-id="b3274-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="b3274-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3274-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3274-126">Request body</span></span>
<span data-ttu-id="b3274-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3274-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3274-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3274-128">Response</span></span>

<span data-ttu-id="b3274-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3274-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3274-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3274-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3274-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3274-131">Request</span></span>

<span data-ttu-id="b3274-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3274-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3274-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3274-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
```
# <a name="c"></a>[<span data-ttu-id="b3274-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3274-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3274-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3274-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3274-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3274-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3274-137">Java</span><span class="sxs-lookup"><span data-stu-id="b3274-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectorgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3274-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3274-138">Response</span></span>
<span data-ttu-id="b3274-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3274-139">The following is an example of the response.</span></span> <span data-ttu-id="b3274-140">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="b3274-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b3274-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3274-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true,
      "region": "region-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectorGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

