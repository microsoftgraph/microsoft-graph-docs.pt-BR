---
title: 'synchronizationSchema: filterOperators'
description: Liste todos os operadores compatíveis com os filtros de escopo.
localization_priority: Normal
ms.openlocfilehash: 6c7f15c684bb0017c8e8430e390015029204ef1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835753"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="cf356-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="cf356-103">synchronizationSchema: filterOperators</span></span>

> <span data-ttu-id="cf356-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf356-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf356-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf356-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf356-106">Liste todos os operadores compatíveis com os [filtros do escopo](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="cf356-106">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cf356-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="cf356-107">Permissions</span></span>
<span data-ttu-id="cf356-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf356-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf356-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf356-110">Permission type</span></span>                        | <span data-ttu-id="cf356-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf356-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf356-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf356-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="cf356-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf356-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="cf356-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf356-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="cf356-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf356-115">Not supported.</span></span>|
|<span data-ttu-id="cf356-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf356-116">Application</span></span>                            |<span data-ttu-id="cf356-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf356-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cf356-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf356-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="cf356-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf356-119">Request headers</span></span>

| <span data-ttu-id="cf356-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cf356-120">Name</span></span>           | <span data-ttu-id="cf356-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf356-121">Type</span></span>    | <span data-ttu-id="cf356-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf356-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="cf356-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf356-123">Authorization</span></span>  | <span data-ttu-id="cf356-124">string</span><span class="sxs-lookup"><span data-stu-id="cf356-124">string</span></span>  | <span data-ttu-id="cf356-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf356-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf356-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf356-127">Request body</span></span>

<span data-ttu-id="cf356-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf356-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf356-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf356-129">Response</span></span>

<span data-ttu-id="cf356-130">Se tiver êxito, este método retornará um `200, OK` código de resposta e um objeto da coleção [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf356-130">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf356-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf356-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cf356-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf356-132">Request</span></span>
<span data-ttu-id="cf356-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf356-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="cf356-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf356-134">Response</span></span>
<span data-ttu-id="cf356-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="cf356-135">The following is an example of a response.</span></span>

><span data-ttu-id="cf356-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cf356-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cf356-137">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf356-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
