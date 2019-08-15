---
title: Atualizar synchronizationSchema
description: Atualize o esquema de sincronização de um determinado trabalho ou modelo. Esse método substitui completamente o esquema atual pelo fornecido na solicitação. Para atualizar o esquema de um modelo, faça a chamada no objeto Application. Você deve ser o proprietário do aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1c9d19fc9d35d5330f52b7e600df8b058b63702e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409650"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="e84ec-106">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e84ec-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e84ec-107">Atualize o esquema de sincronização de um determinado trabalho ou modelo.</span><span class="sxs-lookup"><span data-stu-id="e84ec-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="e84ec-108">Esse método substitui completamente o esquema atual pelo fornecido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="e84ec-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="e84ec-109">Para atualizar o esquema de um modelo, faça a chamada no objeto Application.</span><span class="sxs-lookup"><span data-stu-id="e84ec-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="e84ec-110">Você deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e84ec-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e84ec-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="e84ec-111">Permissions</span></span>
<span data-ttu-id="e84ec-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e84ec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e84ec-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e84ec-114">Permission type</span></span>                        | <span data-ttu-id="e84ec-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e84ec-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e84ec-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e84ec-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="e84ec-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e84ec-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e84ec-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e84ec-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e84ec-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e84ec-119">Not supported.</span></span>|
|<span data-ttu-id="e84ec-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e84ec-120">Application</span></span>                            |<span data-ttu-id="e84ec-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e84ec-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="e84ec-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e84ec-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="e84ec-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e84ec-123">Request headers</span></span>

| <span data-ttu-id="e84ec-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e84ec-124">Name</span></span>           | <span data-ttu-id="e84ec-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e84ec-125">Type</span></span>    | <span data-ttu-id="e84ec-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e84ec-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e84ec-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e84ec-127">Authorization</span></span>  | <span data-ttu-id="e84ec-128">string</span><span class="sxs-lookup"><span data-stu-id="e84ec-128">string</span></span>  | <span data-ttu-id="e84ec-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e84ec-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e84ec-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e84ec-131">Request body</span></span>

<span data-ttu-id="e84ec-132">No corpo da solicitação, forneça o objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) para substituir o esquema existente por.</span><span class="sxs-lookup"><span data-stu-id="e84ec-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="e84ec-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e84ec-133">Response</span></span>

<span data-ttu-id="e84ec-134">Se bem-sucedido, retorna um `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e84ec-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="e84ec-135">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e84ec-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e84ec-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e84ec-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e84ec-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e84ec-137">Request</span></span>
<span data-ttu-id="e84ec-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e84ec-138">The following is an example of a request.</span></span>

><span data-ttu-id="e84ec-139">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e84ec-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="e84ec-140">Forneça todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e84ec-140">Supply all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e84ec-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="e84ec-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="e84ec-142">C#</span><span class="sxs-lookup"><span data-stu-id="e84ec-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e84ec-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e84ec-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e84ec-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e84ec-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e84ec-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e84ec-145">Response</span></span>
<span data-ttu-id="e84ec-146">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="e84ec-146">The following is an example of a response.</span></span>
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
