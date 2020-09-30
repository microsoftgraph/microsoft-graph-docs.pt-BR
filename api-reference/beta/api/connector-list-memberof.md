---
title: Listar memberOf
description: Recupere o MemberGroup do qual o conector é membro.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9c3bb8517ff0e22d0e346304d8290f1a3a2151aa
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312982"
---
# <a name="list-memberof"></a><span data-ttu-id="f9902-103">Listar memberOf</span><span class="sxs-lookup"><span data-stu-id="f9902-103">List memberOf</span></span>

<span data-ttu-id="f9902-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9902-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9902-105">Recupere o [MemberGroup do qual o](../resources/connectorgroup.md) [conector](../resources/connector.md) é membro.</span><span class="sxs-lookup"><span data-stu-id="f9902-105">Retrieve the [connectorGroup](../resources/connectorgroup.md) the [connector](../resources/connector.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9902-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f9902-106">Permissions</span></span>
<span data-ttu-id="f9902-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9902-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f9902-109">Permission type</span></span>      | <span data-ttu-id="f9902-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f9902-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9902-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f9902-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9902-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9902-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f9902-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f9902-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9902-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9902-114">Not supported.</span></span>    |
|<span data-ttu-id="f9902-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f9902-115">Application</span></span> | <span data-ttu-id="f9902-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f9902-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f9902-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f9902-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f9902-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f9902-118">Optional query parameters</span></span>
<span data-ttu-id="f9902-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f9902-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9902-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f9902-120">Request headers</span></span>
| <span data-ttu-id="f9902-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f9902-121">Name</span></span>      |<span data-ttu-id="f9902-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9902-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9902-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f9902-123">Authorization</span></span>  | <span data-ttu-id="f9902-124">Portador.</span><span class="sxs-lookup"><span data-stu-id="f9902-124">Bearer.</span></span> <span data-ttu-id="f9902-125">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="f9902-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9902-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f9902-126">Request body</span></span>
<span data-ttu-id="f9902-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f9902-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9902-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9902-128">Response</span></span>

<span data-ttu-id="f9902-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos do grupo de [conectores](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f9902-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f9902-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f9902-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9902-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f9902-131">Request</span></span>
<span data-ttu-id="f9902-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f9902-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9902-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9902-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="f9902-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9902-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9902-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9902-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9902-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9902-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f9902-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f9902-137">Response</span></span>
<span data-ttu-id="f9902-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f9902-138">The following is an example of the response.</span></span> <span data-ttu-id="f9902-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f9902-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f9902-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f9902-140">All of the properties will be returned from an actual call.</span></span>
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
      "isDefault": false,
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->