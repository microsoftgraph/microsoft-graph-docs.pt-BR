---
title: Atualizar synchronizationSchema
description: Atualize o esquema de sincronização de um determinado trabalho ou modelo. Esse método substitui completamente o esquema atual pelo fornecido na solicitação. Para atualizar o esquema de um modelo, faça a chamada no objeto Application. Você deve ser o proprietário do aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8211b5fc15e6648fea9ba1b4b44c28a93eb5e0f5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452901"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="19624-106">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="19624-106">Update synchronizationSchema</span></span>

<span data-ttu-id="19624-107">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="19624-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19624-108">Atualize o esquema de sincronização de um determinado trabalho ou modelo.</span><span class="sxs-lookup"><span data-stu-id="19624-108">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="19624-109">Esse método substitui completamente o esquema atual pelo fornecido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="19624-109">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="19624-110">Para atualizar o esquema de um modelo, faça a chamada no objeto Application.</span><span class="sxs-lookup"><span data-stu-id="19624-110">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="19624-111">Você deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="19624-111">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="19624-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="19624-112">Permissions</span></span>
<span data-ttu-id="19624-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19624-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19624-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19624-115">Permission type</span></span>                        | <span data-ttu-id="19624-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19624-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="19624-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19624-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="19624-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19624-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="19624-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19624-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="19624-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19624-120">Not supported.</span></span>|
|<span data-ttu-id="19624-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19624-121">Application</span></span>                            |<span data-ttu-id="19624-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19624-122">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="19624-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19624-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="19624-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19624-124">Request headers</span></span>

| <span data-ttu-id="19624-125">Nome</span><span class="sxs-lookup"><span data-stu-id="19624-125">Name</span></span>           | <span data-ttu-id="19624-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="19624-126">Type</span></span>    | <span data-ttu-id="19624-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="19624-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="19624-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="19624-128">Authorization</span></span>  | <span data-ttu-id="19624-129">string</span><span class="sxs-lookup"><span data-stu-id="19624-129">string</span></span>  | <span data-ttu-id="19624-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19624-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19624-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19624-132">Request body</span></span>

<span data-ttu-id="19624-133">No corpo da solicitação, forneça o objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) para substituir o esquema existente por.</span><span class="sxs-lookup"><span data-stu-id="19624-133">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="19624-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="19624-134">Response</span></span>

<span data-ttu-id="19624-135">Se bem-sucedido, retorna um `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="19624-135">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="19624-136">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19624-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19624-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19624-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="19624-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19624-138">Request</span></span>
<span data-ttu-id="19624-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="19624-139">The following is an example of a request.</span></span>

><span data-ttu-id="19624-140">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="19624-140">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="19624-141">Forneça todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19624-141">Supply all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="19624-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="19624-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
Content-type: application/json

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
                },
            ]
        },
        {
            "name": "Salesforce",
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
                    ]
                },
            ]
        },
    ]
}

```
# <a name="c"></a>[<span data-ttu-id="19624-143">C#</span><span class="sxs-lookup"><span data-stu-id="19624-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="19624-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19624-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="19624-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19624-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="19624-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="19624-146">Response</span></span>
<span data-ttu-id="19624-147">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="19624-147">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
