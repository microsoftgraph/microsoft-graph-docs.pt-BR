---
title: Listar membros
description: Recupere uma lista de objetos Connector associados a um conector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1960f7394e2c1482d334812d390b1b60b07dafd9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996469"
---
# <a name="list-members"></a><span data-ttu-id="cf028-103">Listar membros</span><span class="sxs-lookup"><span data-stu-id="cf028-103">List members</span></span>

<span data-ttu-id="cf028-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf028-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf028-105">Recupere uma lista de objetos [Connector](../resources/connector.md) associados a um [conector](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="cf028-105">Retrieve a list of [connector](../resources/connector.md) objects associated with a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf028-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf028-106">Permissions</span></span>
<span data-ttu-id="cf028-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf028-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf028-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf028-109">Permission type</span></span>      | <span data-ttu-id="cf028-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf028-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf028-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf028-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cf028-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cf028-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cf028-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf028-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf028-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf028-114">Not supported.</span></span>    |
|<span data-ttu-id="cf028-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf028-115">Application</span></span> | <span data-ttu-id="cf028-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf028-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cf028-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf028-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf028-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf028-118">Optional query parameters</span></span>
<span data-ttu-id="cf028-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cf028-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf028-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf028-120">Request headers</span></span>
| <span data-ttu-id="cf028-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cf028-121">Name</span></span>      |<span data-ttu-id="cf028-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf028-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cf028-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf028-123">Authorization</span></span>  | <span data-ttu-id="cf028-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="cf028-124">Bearer.</span></span> <span data-ttu-id="cf028-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="cf028-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf028-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf028-126">Request body</span></span>
<span data-ttu-id="cf028-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf028-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf028-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf028-128">Response</span></span>

<span data-ttu-id="cf028-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [Connector](../resources/connector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf028-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf028-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf028-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf028-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf028-131">Request</span></span>
<span data-ttu-id="cf028-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf028-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cf028-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cf028-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="cf028-134">C#</span><span class="sxs-lookup"><span data-stu-id="cf028-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cf028-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cf028-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cf028-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cf028-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cf028-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf028-137">Response</span></span>
<span data-ttu-id="cf028-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf028-138">The following is an example of the response.</span></span> <span data-ttu-id="cf028-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="cf028-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cf028-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf028-140">All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


