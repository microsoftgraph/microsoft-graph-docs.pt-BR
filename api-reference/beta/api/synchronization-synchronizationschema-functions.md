---
title: 'synchronizationSchema: funções'
description: Listar todas as funções atualmente suportadas no attributeMappingSource.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4d47a20fd9a2ddc36b18d411c4fb55939b97362f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471201"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="fe002-103">synchronizationSchema: funções</span><span class="sxs-lookup"><span data-stu-id="fe002-103">synchronizationSchema: functions</span></span>

<span data-ttu-id="fe002-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe002-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe002-105">Listar todas as funções atualmente suportadas no [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="fe002-105">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe002-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe002-106">Permissions</span></span>
<span data-ttu-id="fe002-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe002-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe002-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe002-109">Permission type</span></span>                        | <span data-ttu-id="fe002-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe002-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe002-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe002-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="fe002-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe002-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="fe002-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe002-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="fe002-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe002-114">Not supported.</span></span>|
|<span data-ttu-id="fe002-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe002-115">Application</span></span>                            |<span data-ttu-id="fe002-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe002-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fe002-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe002-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="fe002-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe002-118">Request headers</span></span>

| <span data-ttu-id="fe002-119">Nome</span><span class="sxs-lookup"><span data-stu-id="fe002-119">Name</span></span>           | <span data-ttu-id="fe002-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe002-120">Type</span></span>    | <span data-ttu-id="fe002-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe002-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="fe002-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe002-122">Authorization</span></span>  | <span data-ttu-id="fe002-123">string</span><span class="sxs-lookup"><span data-stu-id="fe002-123">string</span></span>  | <span data-ttu-id="fe002-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe002-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe002-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe002-126">Request body</span></span>

<span data-ttu-id="fe002-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fe002-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe002-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe002-128">Response</span></span>

<span data-ttu-id="fe002-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe002-129">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe002-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe002-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fe002-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe002-131">Request</span></span>
<span data-ttu-id="fe002-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe002-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe002-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe002-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```
# <a name="c"></a>[<span data-ttu-id="fe002-134">C#</span><span class="sxs-lookup"><span data-stu-id="fe002-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-functions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe002-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe002-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-functions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe002-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe002-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-functions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fe002-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe002-137">Response</span></span>
<span data-ttu-id="fe002-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="fe002-138">The following is an example of a response.</span></span>

><span data-ttu-id="fe002-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="fe002-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fe002-140">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe002-140">All the properties will be returned in an actual call.</span></span>

<!--
{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        }
    ]
}
```

<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "IsNothing",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Join",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "separator",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Prepend",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "prefix",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Mid",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "start",
                    "required": true,
                    "type": "Integer"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "length",
                    "required": true,
                    "type": "Integer"
                }
            ]
        },
        {
            "name": "Not",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Replace",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Find",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpression",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpressionGroupName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Replacement",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "ReplacementPropertyName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Template",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "SingleAppRoleAssignment",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Split",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "delimiter",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "StripSpaces",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Switch",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "defaultValue",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "switchValue",
                    "required": false,
                    "type": "String"
                }
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
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
