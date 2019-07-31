---
title: Obter synchronizationSchema
description: Recupere o esquema de um determinado trabalho de sincronização ou modelo.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55f6b6935808cd96bf9eebf8e2662d0649bbb66c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977663"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="40a3c-103">Obter synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="40a3c-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40a3c-104">Recupere o esquema de um determinado trabalho de sincronização ou modelo.</span><span class="sxs-lookup"><span data-stu-id="40a3c-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="40a3c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="40a3c-105">Permissions</span></span>
<span data-ttu-id="40a3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40a3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40a3c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40a3c-108">Permission type</span></span>                        | <span data-ttu-id="40a3c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40a3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="40a3c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40a3c-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="40a3c-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40a3c-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="40a3c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40a3c-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="40a3c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40a3c-113">Not supported.</span></span> |
|<span data-ttu-id="40a3c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40a3c-114">Application</span></span>                            |<span data-ttu-id="40a3c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40a3c-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="40a3c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40a3c-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="40a3c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40a3c-117">Request headers</span></span>

| <span data-ttu-id="40a3c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="40a3c-118">Name</span></span>           | <span data-ttu-id="40a3c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="40a3c-119">Type</span></span>    | <span data-ttu-id="40a3c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="40a3c-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="40a3c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="40a3c-121">Authorization</span></span>  | <span data-ttu-id="40a3c-122">string</span><span class="sxs-lookup"><span data-stu-id="40a3c-122">string</span></span>  | <span data-ttu-id="40a3c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40a3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40a3c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40a3c-125">Request body</span></span>

<span data-ttu-id="40a3c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40a3c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40a3c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="40a3c-127">Response</span></span>

<span data-ttu-id="40a3c-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40a3c-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40a3c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40a3c-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="40a3c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40a3c-130">Request</span></span>
<span data-ttu-id="40a3c-131">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="40a3c-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="40a3c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="40a3c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="40a3c-133">C#</span><span class="sxs-lookup"><span data-stu-id="40a3c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="40a3c-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="40a3c-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="40a3c-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="40a3c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="40a3c-136">Java</span><span class="sxs-lookup"><span data-stu-id="40a3c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="40a3c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="40a3c-137">Response</span></span>
<span data-ttu-id="40a3c-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="40a3c-138">The following is an example of a response.</span></span>

><span data-ttu-id="40a3c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40a3c-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="40a3c-140">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40a3c-140">All the properties will be returned in an actual call.</span></span>
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
