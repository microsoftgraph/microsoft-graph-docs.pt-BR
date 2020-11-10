---
title: Obter synchronizationSchema
description: Recupere o esquema de um determinado trabalho de sincronização ou modelo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c952e2b8831a7d2d23964590fb944d8f5c3580c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969496"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="ef216-103">Obter synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="ef216-103">Get synchronizationSchema</span></span>

<span data-ttu-id="ef216-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef216-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef216-105">Recupere o esquema de um determinado trabalho de sincronização ou modelo.</span><span class="sxs-lookup"><span data-stu-id="ef216-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef216-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef216-106">Permissions</span></span>
<span data-ttu-id="ef216-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef216-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef216-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef216-109">Permission type</span></span>                        | <span data-ttu-id="ef216-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef216-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef216-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef216-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="ef216-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef216-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="ef216-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef216-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="ef216-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef216-114">Not supported.</span></span> |
|<span data-ttu-id="ef216-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef216-115">Application</span></span>                            |<span data-ttu-id="ef216-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef216-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ef216-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef216-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="ef216-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef216-118">Request headers</span></span>

| <span data-ttu-id="ef216-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ef216-119">Name</span></span>           | <span data-ttu-id="ef216-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef216-120">Type</span></span>    | <span data-ttu-id="ef216-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef216-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ef216-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef216-122">Authorization</span></span>  | <span data-ttu-id="ef216-123">string</span><span class="sxs-lookup"><span data-stu-id="ef216-123">string</span></span>  | <span data-ttu-id="ef216-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef216-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef216-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef216-126">Request body</span></span>

<span data-ttu-id="ef216-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef216-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef216-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef216-128">Response</span></span>

<span data-ttu-id="ef216-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef216-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef216-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef216-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ef216-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef216-131">Request</span></span>
<span data-ttu-id="ef216-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef216-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef216-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef216-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="ef216-134">C#</span><span class="sxs-lookup"><span data-stu-id="ef216-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef216-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef216-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef216-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef216-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef216-137">Java</span><span class="sxs-lookup"><span data-stu-id="ef216-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ef216-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef216-138">Response</span></span>
<span data-ttu-id="ef216-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="ef216-139">The following is an example of a response.</span></span>

><span data-ttu-id="ef216-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ef216-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ef216-141">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef216-141">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                }
            ]
        },
        {
            "name": "Salesforce",
            "objects": [{}]
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                        {}
                    ]
                },
                {}
            ]
        },
        {}
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


