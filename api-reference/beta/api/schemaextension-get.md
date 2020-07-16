---
title: Get schemaExtension
description: Obtenha as propriedades da definição schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: e69342cff9789af6d208cbb7d071dfb43edba1b0
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863485"
---
# <a name="get-schemaextension"></a><span data-ttu-id="5e193-103">Get schemaExtension</span><span class="sxs-lookup"><span data-stu-id="5e193-103">Get schemaExtension</span></span>

<span data-ttu-id="5e193-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e193-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e193-105">Obtenha as propriedades da definição [schemaExtension](../resources/schemaextension.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="5e193-105">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e193-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5e193-106">Permissions</span></span>
<span data-ttu-id="5e193-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e193-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5e193-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5e193-109">Permission type</span></span>      | <span data-ttu-id="5e193-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5e193-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e193-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5e193-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5e193-112">User. Read, Application. Read. All</span><span class="sxs-lookup"><span data-stu-id="5e193-112">User.Read, Application.Read.All</span></span>  |
|<span data-ttu-id="5e193-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5e193-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e193-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5e193-114">Not supported.</span></span>    |
|<span data-ttu-id="5e193-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5e193-115">Application</span></span> | <span data-ttu-id="5e193-116">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e193-116">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5e193-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5e193-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5e193-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5e193-118">Optional query parameters</span></span>
<span data-ttu-id="5e193-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5e193-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e193-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5e193-120">Request headers</span></span>
| <span data-ttu-id="5e193-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5e193-121">Name</span></span>      |<span data-ttu-id="5e193-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e193-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5e193-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5e193-123">Authorization</span></span>  | <span data-ttu-id="5e193-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5e193-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e193-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e193-126">Content-Type</span></span>   | <span data-ttu-id="5e193-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5e193-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5e193-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5e193-128">Request body</span></span>
<span data-ttu-id="5e193-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5e193-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e193-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e193-130">Response</span></span>

<span data-ttu-id="5e193-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5e193-131">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e193-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5e193-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e193-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5e193-133">Request</span></span>
<span data-ttu-id="5e193-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5e193-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e193-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e193-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
# <a name="c"></a>[<span data-ttu-id="5e193-136">C#</span><span class="sxs-lookup"><span data-stu-id="5e193-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e193-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e193-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e193-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e193-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5e193-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="5e193-139">Response</span></span>
<span data-ttu-id="5e193-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5e193-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "id":"graphlearn_test",
    "description": "Yet another test schema",
    "targetTypes": [
        "User", "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "testName",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="5e193-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="5e193-143">See also</span></span>

- [<span data-ttu-id="5e193-144">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="5e193-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="5e193-145">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="5e193-145">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
