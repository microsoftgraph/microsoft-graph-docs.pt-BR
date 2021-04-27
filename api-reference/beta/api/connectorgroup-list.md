---
title: Listar connectorGroups
description: Recupere uma lista de objetos connectorgroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: bfb1fa038bf187c4932693d6b4362d3c61e2516e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047165"
---
# <a name="list-connectorgroups"></a><span data-ttu-id="672d6-103">Listar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="672d6-103">List connectorGroups</span></span>

<span data-ttu-id="672d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="672d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="672d6-105">Recupere uma lista de [objetos connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="672d6-105">Retrieve a list of [connectorGroup](../resources/connectorgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="672d6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="672d6-106">Permissions</span></span>
<span data-ttu-id="672d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="672d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="672d6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="672d6-109">Permission type</span></span>      | <span data-ttu-id="672d6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="672d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="672d6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="672d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="672d6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="672d6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="672d6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="672d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="672d6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="672d6-114">Not supported.</span></span>    |
|<span data-ttu-id="672d6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="672d6-115">Application</span></span> | <span data-ttu-id="672d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="672d6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="672d6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="672d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="672d6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="672d6-118">Optional query parameters</span></span>
<span data-ttu-id="672d6-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="672d6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="672d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="672d6-120">Request headers</span></span>
| <span data-ttu-id="672d6-121">Nome</span><span class="sxs-lookup"><span data-stu-id="672d6-121">Name</span></span>      |<span data-ttu-id="672d6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="672d6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="672d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="672d6-123">Authorization</span></span>  | <span data-ttu-id="672d6-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="672d6-124">Bearer.</span></span> <span data-ttu-id="672d6-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="672d6-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="672d6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="672d6-126">Request body</span></span>
<span data-ttu-id="672d6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="672d6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="672d6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="672d6-128">Response</span></span>

<span data-ttu-id="672d6-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="672d6-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="672d6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="672d6-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="672d6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="672d6-131">Request</span></span>

<span data-ttu-id="672d6-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="672d6-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="672d6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="672d6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
```
# <a name="c"></a>[<span data-ttu-id="672d6-134">C#</span><span class="sxs-lookup"><span data-stu-id="672d6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="672d6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="672d6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="672d6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="672d6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="672d6-137">Java</span><span class="sxs-lookup"><span data-stu-id="672d6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectorgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="672d6-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="672d6-138">Response</span></span>
<span data-ttu-id="672d6-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="672d6-139">The following is an example of the response.</span></span> <span data-ttu-id="672d6-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="672d6-140">Note: The response object shown here might be shortened for readability.</span></span>
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

