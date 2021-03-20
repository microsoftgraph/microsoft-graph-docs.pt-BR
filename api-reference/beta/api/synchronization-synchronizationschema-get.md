---
title: Obter synchronizationSchema
description: Recupere o esquema para um determinado trabalho ou modelo de sincronização.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bd321f3375623914afa6cc9c803b18e2a22d1ed4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952940"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="7dae8-103">Obter synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="7dae8-103">Get synchronizationSchema</span></span>

<span data-ttu-id="7dae8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7dae8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dae8-105">Recupere o esquema para um determinado trabalho ou modelo de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7dae8-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dae8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dae8-106">Permissions</span></span>
<span data-ttu-id="7dae8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dae8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dae8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dae8-109">Permission type</span></span>                        | <span data-ttu-id="7dae8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dae8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dae8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dae8-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="7dae8-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7dae8-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="7dae8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dae8-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7dae8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dae8-114">Not supported.</span></span> |
|<span data-ttu-id="7dae8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dae8-115">Application</span></span>                            |<span data-ttu-id="7dae8-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dae8-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7dae8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dae8-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="7dae8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dae8-118">Request headers</span></span>

| <span data-ttu-id="7dae8-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7dae8-119">Name</span></span>           | <span data-ttu-id="7dae8-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dae8-120">Type</span></span>    | <span data-ttu-id="7dae8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dae8-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7dae8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dae8-122">Authorization</span></span>  | <span data-ttu-id="7dae8-123">string</span><span class="sxs-lookup"><span data-stu-id="7dae8-123">string</span></span>  | <span data-ttu-id="7dae8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dae8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dae8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dae8-126">Request body</span></span>

<span data-ttu-id="7dae8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7dae8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dae8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dae8-128">Response</span></span>

<span data-ttu-id="7dae8-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto synchronizationSchema](../resources/synchronization-synchronizationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dae8-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dae8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dae8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7dae8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dae8-131">Request</span></span>
<span data-ttu-id="7dae8-132">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dae8-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7dae8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7dae8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="7dae8-134">C#</span><span class="sxs-lookup"><span data-stu-id="7dae8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7dae8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7dae8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7dae8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7dae8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7dae8-137">Java</span><span class="sxs-lookup"><span data-stu-id="7dae8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7dae8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dae8-138">Response</span></span>
<span data-ttu-id="7dae8-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7dae8-139">The following is an example of a response.</span></span>

><span data-ttu-id="7dae8-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7dae8-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7dae8-141">Todas as propriedades serão retornadas em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dae8-141">All the properties will be returned in an actual call.</span></span>
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


