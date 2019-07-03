---
title: 'synchronizationSchema: filterOperators'
description: Liste todos os operadores com suporte nos filtros de escopo.
localization_priority: Normal
ms.openlocfilehash: 75c82fd5512094b6f2c3fec8d1e9207657097b79
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456978"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="3cfd6-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="3cfd6-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cfd6-104">Liste todos os operadores com suporte nos [filtros de escopo](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="3cfd6-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3cfd6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cfd6-105">Permissions</span></span>
<span data-ttu-id="3cfd6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cfd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cfd6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cfd6-108">Permission type</span></span>                        | <span data-ttu-id="3cfd6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cfd6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cfd6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cfd6-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="3cfd6-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cfd6-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3cfd6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cfd6-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3cfd6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-113">Not supported.</span></span>|
|<span data-ttu-id="3cfd6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cfd6-114">Application</span></span>                            |<span data-ttu-id="3cfd6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3cfd6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfd6-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="3cfd6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfd6-117">Request headers</span></span>

| <span data-ttu-id="3cfd6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3cfd6-118">Name</span></span>           | <span data-ttu-id="3cfd6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cfd6-119">Type</span></span>    | <span data-ttu-id="3cfd6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cfd6-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3cfd6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cfd6-121">Authorization</span></span>  | <span data-ttu-id="3cfd6-122">string</span><span class="sxs-lookup"><span data-stu-id="3cfd6-122">string</span></span>  | <span data-ttu-id="3cfd6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cfd6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfd6-125">Request body</span></span>

<span data-ttu-id="3cfd6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cfd6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cfd6-127">Response</span></span>

<span data-ttu-id="3cfd6-128">Se tiver êxito, este método retornará `200, OK` um código de resposta e um objeto da coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cfd6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cfd6-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3cfd6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cfd6-130">Request</span></span>
<span data-ttu-id="3cfd6-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3cfd6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfd6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3cfd6-133">C#</span><span class="sxs-lookup"><span data-stu-id="3cfd6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cfd6-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cfd6-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3cfd6-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3cfd6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3cfd6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cfd6-136">Response</span></span>
<span data-ttu-id="3cfd6-137">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-137">The following is an example of a response.</span></span>

><span data-ttu-id="3cfd6-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3cfd6-139">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3cfd6-139">All the properties will be returned in an actual call.</span></span>

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
