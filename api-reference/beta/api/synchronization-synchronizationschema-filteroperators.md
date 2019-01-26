---
title: 'synchronizationSchema: filterOperators'
description: Liste todos os operadores compatíveis com os filtros de escopo.
localization_priority: Normal
ms.openlocfilehash: c564142aa6a26b3f83fa5f82036e3b97dc13e672
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573225"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="2e4ba-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="2e4ba-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e4ba-104">Liste todos os operadores compatíveis com os [filtros do escopo](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="2e4ba-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2e4ba-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e4ba-105">Permissions</span></span>
<span data-ttu-id="2e4ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e4ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e4ba-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e4ba-108">Permission type</span></span>                        | <span data-ttu-id="2e4ba-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e4ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e4ba-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e4ba-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="2e4ba-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e4ba-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="2e4ba-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e4ba-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="2e4ba-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-113">Not supported.</span></span>|
|<span data-ttu-id="2e4ba-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e4ba-114">Application</span></span>                            |<span data-ttu-id="2e4ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2e4ba-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e4ba-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="2e4ba-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4ba-117">Request headers</span></span>

| <span data-ttu-id="2e4ba-118">Nome</span><span class="sxs-lookup"><span data-stu-id="2e4ba-118">Name</span></span>           | <span data-ttu-id="2e4ba-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e4ba-119">Type</span></span>    | <span data-ttu-id="2e4ba-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e4ba-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="2e4ba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e4ba-121">Authorization</span></span>  | <span data-ttu-id="2e4ba-122">string</span><span class="sxs-lookup"><span data-stu-id="2e4ba-122">string</span></span>  | <span data-ttu-id="2e4ba-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e4ba-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4ba-125">Request body</span></span>

<span data-ttu-id="2e4ba-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e4ba-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4ba-127">Response</span></span>

<span data-ttu-id="2e4ba-128">Se tiver êxito, este método retornará um `200, OK` código de resposta e um objeto da coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e4ba-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e4ba-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2e4ba-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e4ba-130">Request</span></span>
<span data-ttu-id="2e4ba-131">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="2e4ba-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e4ba-132">Response</span></span>
<span data-ttu-id="2e4ba-133">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-133">The following is an example of a response.</span></span>

><span data-ttu-id="2e4ba-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2e4ba-135">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e4ba-135">All the properties will be returned in an actual call.</span></span>

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
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [                
                "@string"
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
               "Boolean"
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
                "Boolean"
            ]
        },
        {
            "name": "IS NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
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
                "Boolean"
            ]
        },
        {
            "name": "NOT REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-filteroperators.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
