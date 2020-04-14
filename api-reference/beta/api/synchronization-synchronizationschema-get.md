---
title: Obter synchronizationSchema
description: Recupere o esquema de um determinado trabalho de sincronização ou modelo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e7b7d961b70be43f569c391660ef567b1852c42d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471186"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="600a7-103">Obter synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="600a7-103">Get synchronizationSchema</span></span>

<span data-ttu-id="600a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="600a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="600a7-105">Recupere o esquema de um determinado trabalho de sincronização ou modelo.</span><span class="sxs-lookup"><span data-stu-id="600a7-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="600a7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="600a7-106">Permissions</span></span>
<span data-ttu-id="600a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="600a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="600a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="600a7-109">Permission type</span></span>                        | <span data-ttu-id="600a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="600a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="600a7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="600a7-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="600a7-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="600a7-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="600a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="600a7-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="600a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="600a7-114">Not supported.</span></span> |
|<span data-ttu-id="600a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="600a7-115">Application</span></span>                            |<span data-ttu-id="600a7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="600a7-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="600a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="600a7-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="600a7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="600a7-118">Request headers</span></span>

| <span data-ttu-id="600a7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="600a7-119">Name</span></span>           | <span data-ttu-id="600a7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="600a7-120">Type</span></span>    | <span data-ttu-id="600a7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="600a7-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="600a7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="600a7-122">Authorization</span></span>  | <span data-ttu-id="600a7-123">string</span><span class="sxs-lookup"><span data-stu-id="600a7-123">string</span></span>  | <span data-ttu-id="600a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="600a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="600a7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="600a7-126">Request body</span></span>

<span data-ttu-id="600a7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="600a7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="600a7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="600a7-128">Response</span></span>

<span data-ttu-id="600a7-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="600a7-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="600a7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="600a7-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="600a7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="600a7-131">Request</span></span>
<span data-ttu-id="600a7-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="600a7-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="600a7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="600a7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="600a7-134">C#</span><span class="sxs-lookup"><span data-stu-id="600a7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="600a7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="600a7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="600a7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="600a7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="600a7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="600a7-137">Response</span></span>
<span data-ttu-id="600a7-138">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="600a7-138">The following is an example of a response.</span></span>

><span data-ttu-id="600a7-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="600a7-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="600a7-140">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="600a7-140">All the properties will be returned in an actual call.</span></span>
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
