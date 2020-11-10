---
title: 'synchronizationSchema: filterOperators'
description: Liste todos os operadores com suporte nos filtros de escopo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 37b6fa4eccbf6afe3f4f9b16dec91bbf6e95fec2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980297"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="fdf0a-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="fdf0a-103">synchronizationSchema: filterOperators</span></span>

<span data-ttu-id="fdf0a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdf0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdf0a-105">Liste todos os operadores com suporte nos [filtros de escopo](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="fdf0a-105">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fdf0a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fdf0a-106">Permissions</span></span>
<span data-ttu-id="fdf0a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdf0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdf0a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdf0a-109">Permission type</span></span>                        | <span data-ttu-id="fdf0a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fdf0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdf0a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdf0a-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="fdf0a-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf0a-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="fdf0a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdf0a-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="fdf0a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-114">Not supported.</span></span>|
|<span data-ttu-id="fdf0a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdf0a-115">Application</span></span>                            |<span data-ttu-id="fdf0a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fdf0a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdf0a-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="fdf0a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf0a-118">Request headers</span></span>

| <span data-ttu-id="fdf0a-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fdf0a-119">Name</span></span>           | <span data-ttu-id="fdf0a-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdf0a-120">Type</span></span>    | <span data-ttu-id="fdf0a-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdf0a-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="fdf0a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdf0a-122">Authorization</span></span>  | <span data-ttu-id="fdf0a-123">string</span><span class="sxs-lookup"><span data-stu-id="fdf0a-123">string</span></span>  | <span data-ttu-id="fdf0a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fdf0a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf0a-126">Request body</span></span>

<span data-ttu-id="fdf0a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdf0a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf0a-128">Response</span></span>

<span data-ttu-id="fdf0a-129">Se tiver êxito, este método retornará um `200, OK` código de resposta e um objeto da coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-129">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdf0a-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdf0a-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fdf0a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdf0a-131">Request</span></span>
<span data-ttu-id="fdf0a-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fdf0a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fdf0a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="c"></a>[<span data-ttu-id="fdf0a-134">C#</span><span class="sxs-lookup"><span data-stu-id="fdf0a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fdf0a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fdf0a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fdf0a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fdf0a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fdf0a-137">Java</span><span class="sxs-lookup"><span data-stu-id="fdf0a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-filteroperators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fdf0a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdf0a-138">Response</span></span>
<span data-ttu-id="fdf0a-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-139">The following is an example of a response.</span></span>

><span data-ttu-id="fdf0a-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fdf0a-141">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdf0a-141">All the properties will be returned in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "String",
                "Integer"
            ]
        }
    ]
}
```
<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "IS FALSE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "IS NOT NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS TRUE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "NOT EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "NOT REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        }
    ]
}
-->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: synchronizationschema_filteroperators/container/arity:\r\n       Expected type String but actual was Binary. Property: arity, actual value: 'Binary'"
  ]
}
-->


