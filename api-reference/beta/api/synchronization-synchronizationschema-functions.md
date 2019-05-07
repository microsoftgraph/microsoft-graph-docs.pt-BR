---
title: 'synchronizationSchema: funções'
description: Listar todas as funções atualmente suportadas no attributeMappingSource.
localization_priority: Normal
ms.openlocfilehash: c1563255a7444c65030799de3477bbadcaf7a196
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637987"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="7f54c-103">synchronizationSchema: funções</span><span class="sxs-lookup"><span data-stu-id="7f54c-103">synchronizationSchema: functions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f54c-104">Listar todas as funções atualmente suportadas no [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="7f54c-104">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f54c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7f54c-105">Permissions</span></span>
<span data-ttu-id="7f54c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f54c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f54c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f54c-108">Permission type</span></span>                        | <span data-ttu-id="7f54c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f54c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f54c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f54c-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="7f54c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f54c-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7f54c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f54c-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7f54c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f54c-113">Not supported.</span></span>|
|<span data-ttu-id="7f54c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f54c-114">Application</span></span>                            |<span data-ttu-id="7f54c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f54c-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7f54c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f54c-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="7f54c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f54c-117">Request headers</span></span>

| <span data-ttu-id="7f54c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="7f54c-118">Name</span></span>           | <span data-ttu-id="7f54c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f54c-119">Type</span></span>    | <span data-ttu-id="7f54c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f54c-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7f54c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f54c-121">Authorization</span></span>  | <span data-ttu-id="7f54c-122">string</span><span class="sxs-lookup"><span data-stu-id="7f54c-122">string</span></span>  | <span data-ttu-id="7f54c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7f54c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f54c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f54c-125">Request body</span></span>

<span data-ttu-id="7f54c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f54c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f54c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f54c-127">Response</span></span>

<span data-ttu-id="7f54c-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f54c-128">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f54c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f54c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7f54c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f54c-130">Request</span></span>
<span data-ttu-id="7f54c-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f54c-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="7f54c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f54c-132">Response</span></span>
<span data-ttu-id="7f54c-133">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7f54c-133">The following is an example of a response.</span></span>

><span data-ttu-id="7f54c-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7f54c-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7f54c-135">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f54c-135">All the properties will be returned in an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7f54c-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="7f54c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7f54c-137">Basic</span><span class="sxs-lookup"><span data-stu-id="7f54c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationschema_functions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f54c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f54c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationschema_functions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-functions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-functions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
