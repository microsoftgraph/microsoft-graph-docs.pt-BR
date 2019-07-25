---
title: Atualizar synchronizationSchema
description: Atualize o esquema de sincronização de um determinado trabalho ou modelo. Esse método substitui completamente o esquema atual pelo fornecido na solicitação. Para atualizar o esquema de um modelo, faça a chamada no objeto Application. Você deve ser o proprietário do aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 63e1ed50035cd7d04775a3af66b0127d6da17395
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869102"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="8503f-106">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="8503f-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8503f-107">Atualize o esquema de sincronização de um determinado trabalho ou modelo.</span><span class="sxs-lookup"><span data-stu-id="8503f-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="8503f-108">Esse método substitui completamente o esquema atual pelo fornecido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="8503f-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="8503f-109">Para atualizar o esquema de um modelo, faça a chamada no objeto Application.</span><span class="sxs-lookup"><span data-stu-id="8503f-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="8503f-110">Você deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8503f-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="8503f-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="8503f-111">Permissions</span></span>
<span data-ttu-id="8503f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8503f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8503f-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8503f-114">Permission type</span></span>                        | <span data-ttu-id="8503f-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8503f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8503f-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8503f-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="8503f-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8503f-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="8503f-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8503f-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="8503f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8503f-119">Not supported.</span></span>|
|<span data-ttu-id="8503f-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8503f-120">Application</span></span>                            |<span data-ttu-id="8503f-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8503f-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="8503f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8503f-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="8503f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8503f-123">Request headers</span></span>

| <span data-ttu-id="8503f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8503f-124">Name</span></span>           | <span data-ttu-id="8503f-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="8503f-125">Type</span></span>    | <span data-ttu-id="8503f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8503f-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="8503f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="8503f-127">Authorization</span></span>  | <span data-ttu-id="8503f-128">string</span><span class="sxs-lookup"><span data-stu-id="8503f-128">string</span></span>  | <span data-ttu-id="8503f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8503f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8503f-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8503f-131">Request body</span></span>

<span data-ttu-id="8503f-132">No corpo da solicitação, forneça o objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) para substituir o esquema existente por.</span><span class="sxs-lookup"><span data-stu-id="8503f-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="8503f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="8503f-133">Response</span></span>

<span data-ttu-id="8503f-134">Se bem-sucedido, retorna um `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="8503f-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="8503f-135">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8503f-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8503f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8503f-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8503f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8503f-137">Request</span></span>
<span data-ttu-id="8503f-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="8503f-138">The following is an example of a request.</span></span>

><span data-ttu-id="8503f-139">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8503f-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="8503f-140">Forneça todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8503f-140">Supply all the properties in an actual call.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8503f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8503f-141">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="8503f-142">C#</span><span class="sxs-lookup"><span data-stu-id="8503f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8503f-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="8503f-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8503f-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8503f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8503f-145">Java</span><span class="sxs-lookup"><span data-stu-id="8503f-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8503f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8503f-146">Response</span></span>
<span data-ttu-id="8503f-147">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="8503f-147">The following is an example of a response.</span></span>
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
