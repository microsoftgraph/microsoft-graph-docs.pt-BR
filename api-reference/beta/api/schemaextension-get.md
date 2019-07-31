---
title: Get schemaExtension
description: Obtenha as propriedades da definição schemaExtension especificada.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: cee5bf517598adfeb659e2d21fa75445cfa0e7a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982958"
---
# <a name="get-schemaextension"></a><span data-ttu-id="fc8d9-103">Get schemaExtension</span><span class="sxs-lookup"><span data-stu-id="fc8d9-103">Get schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc8d9-104">Obtenha as propriedades da definição [schemaExtension](../resources/schemaextension.md) especificada.</span><span class="sxs-lookup"><span data-stu-id="fc8d9-104">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc8d9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fc8d9-105">Permissions</span></span>
<span data-ttu-id="fc8d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc8d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc8d9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc8d9-108">Permission type</span></span>      | <span data-ttu-id="fc8d9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc8d9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc8d9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc8d9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc8d9-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc8d9-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc8d9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc8d9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc8d9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc8d9-113">Not supported.</span></span>    |
|<span data-ttu-id="fc8d9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc8d9-114">Application</span></span> | <span data-ttu-id="fc8d9-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc8d9-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc8d9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc8d9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc8d9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fc8d9-117">Optional query parameters</span></span>
<span data-ttu-id="fc8d9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fc8d9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc8d9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8d9-119">Request headers</span></span>
| <span data-ttu-id="fc8d9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fc8d9-120">Name</span></span>      |<span data-ttu-id="fc8d9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc8d9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fc8d9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc8d9-122">Authorization</span></span>  | <span data-ttu-id="fc8d9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc8d9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc8d9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc8d9-125">Content-Type</span></span>   | <span data-ttu-id="fc8d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc8d9-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc8d9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8d9-127">Request body</span></span>
<span data-ttu-id="fc8d9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fc8d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc8d9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc8d9-129">Response</span></span>

<span data-ttu-id="fc8d9-130">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc8d9-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc8d9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc8d9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc8d9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc8d9-132">Request</span></span>
<span data-ttu-id="fc8d9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc8d9-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fc8d9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc8d9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc8d9-135">C#</span><span class="sxs-lookup"><span data-stu-id="fc8d9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc8d9-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="fc8d9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc8d9-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fc8d9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fc8d9-138">Java</span><span class="sxs-lookup"><span data-stu-id="fc8d9-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fc8d9-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc8d9-139">Response</span></span>
<span data-ttu-id="fc8d9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc8d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fc8d9-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="fc8d9-143">See also</span></span>

- [<span data-ttu-id="fc8d9-144">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="fc8d9-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fc8d9-145">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="fc8d9-145">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
