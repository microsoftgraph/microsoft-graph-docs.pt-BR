---
title: Listar connectorGroups
description: Recupere uma lista de objetos de conexão.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 53918f700233c130a4b195eb4bc604901c3560a9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957355"
---
# <a name="list-connectorgroups"></a><span data-ttu-id="6261e-103">Listar connectorGroups</span><span class="sxs-lookup"><span data-stu-id="6261e-103">List connectorGroups</span></span>

<span data-ttu-id="6261e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6261e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6261e-105">Recupere uma lista de objetos de [conexão](../resources/connectorgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6261e-105">Retrieve a list of [connectorGroup](../resources/connectorgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="6261e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6261e-106">Permissions</span></span>
<span data-ttu-id="6261e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6261e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6261e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6261e-109">Permission type</span></span>      | <span data-ttu-id="6261e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6261e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6261e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6261e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6261e-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6261e-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6261e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6261e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6261e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6261e-114">Not supported.</span></span>    |
|<span data-ttu-id="6261e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6261e-115">Application</span></span> | <span data-ttu-id="6261e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6261e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6261e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6261e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6261e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6261e-118">Optional query parameters</span></span>
<span data-ttu-id="6261e-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6261e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6261e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6261e-120">Request headers</span></span>
| <span data-ttu-id="6261e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6261e-121">Name</span></span>      |<span data-ttu-id="6261e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6261e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6261e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6261e-123">Authorization</span></span>  | <span data-ttu-id="6261e-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="6261e-124">Bearer.</span></span> <span data-ttu-id="6261e-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="6261e-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="6261e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6261e-126">Request body</span></span>
<span data-ttu-id="6261e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6261e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6261e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6261e-128">Response</span></span>

<span data-ttu-id="6261e-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos do grupo de [conectores](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6261e-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6261e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6261e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6261e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6261e-131">Request</span></span>

<span data-ttu-id="6261e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6261e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6261e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6261e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
```
# <a name="c"></a>[<span data-ttu-id="6261e-134">C#</span><span class="sxs-lookup"><span data-stu-id="6261e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6261e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6261e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6261e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6261e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6261e-137">Java</span><span class="sxs-lookup"><span data-stu-id="6261e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectorgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6261e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6261e-138">Response</span></span>
<span data-ttu-id="6261e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6261e-139">The following is an example of the response.</span></span> <span data-ttu-id="6261e-140">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="6261e-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6261e-141">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6261e-141">All of the properties will be returned from an actual call.</span></span>
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
