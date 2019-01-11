---
title: 'synchronizationSchema: funções'
description: Liste todas as funções atualmente compatíveis com o attributeMappingSource.
localization_priority: Normal
ms.openlocfilehash: 5dc7734e9d747ac1e832aebb7d9c7355c2fbb52f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841003"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="c3a82-103">synchronizationSchema: funções</span><span class="sxs-lookup"><span data-stu-id="c3a82-103">synchronizationSchema: functions</span></span>

> <span data-ttu-id="c3a82-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c3a82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3a82-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c3a82-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3a82-106">Liste todas as funções atualmente compatíveis com o [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="c3a82-106">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c3a82-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="c3a82-107">Permissions</span></span>
<span data-ttu-id="c3a82-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3a82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3a82-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3a82-110">Permission type</span></span>                        | <span data-ttu-id="c3a82-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3a82-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3a82-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3a82-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="c3a82-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a82-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c3a82-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3a82-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c3a82-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3a82-115">Not supported.</span></span>|
|<span data-ttu-id="c3a82-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3a82-116">Application</span></span>                            |<span data-ttu-id="c3a82-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3a82-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c3a82-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3a82-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="c3a82-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3a82-119">Request headers</span></span>

| <span data-ttu-id="c3a82-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c3a82-120">Name</span></span>           | <span data-ttu-id="c3a82-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3a82-121">Type</span></span>    | <span data-ttu-id="c3a82-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3a82-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c3a82-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3a82-123">Authorization</span></span>  | <span data-ttu-id="c3a82-124">string</span><span class="sxs-lookup"><span data-stu-id="c3a82-124">string</span></span>  | <span data-ttu-id="c3a82-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3a82-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3a82-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3a82-127">Request body</span></span>

<span data-ttu-id="c3a82-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c3a82-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3a82-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3a82-129">Response</span></span>

<span data-ttu-id="c3a82-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3a82-130">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3a82-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3a82-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c3a82-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3a82-132">Request</span></span>
<span data-ttu-id="c3a82-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3a82-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="c3a82-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3a82-134">Response</span></span>
<span data-ttu-id="c3a82-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c3a82-135">The following is an example of a response.</span></span>

><span data-ttu-id="c3a82-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c3a82-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c3a82-137">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3a82-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
