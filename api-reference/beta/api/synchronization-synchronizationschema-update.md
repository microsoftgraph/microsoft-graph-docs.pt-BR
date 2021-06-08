---
title: Atualizar sincronizaçãoSchema
description: Atualize o esquema de sincronização para um determinado trabalho ou modelo. Este método substitui totalmente o esquema atual pelo fornecido na solicitação. Para atualizar o esquema de um modelo, faça a chamada no objeto application. Você deve ser o proprietário do aplicativo.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bae3e92c82680dbf4f376e54bb5353ccb7851706
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786913"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="36659-106">Atualizar sincronizaçãoSchema</span><span class="sxs-lookup"><span data-stu-id="36659-106">Update synchronizationSchema</span></span>

<span data-ttu-id="36659-107">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36659-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36659-108">Atualize o esquema de sincronização para um determinado trabalho ou modelo.</span><span class="sxs-lookup"><span data-stu-id="36659-108">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="36659-109">Este método substitui totalmente o esquema atual pelo fornecido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="36659-109">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="36659-110">Para atualizar o esquema de um modelo, faça a chamada no objeto application.</span><span class="sxs-lookup"><span data-stu-id="36659-110">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="36659-111">Você deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="36659-111">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="36659-112">Permissions</span><span class="sxs-lookup"><span data-stu-id="36659-112">Permissions</span></span>
<span data-ttu-id="36659-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36659-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36659-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36659-115">Permission type</span></span>                        | <span data-ttu-id="36659-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36659-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="36659-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36659-117">Delegated (work or school account)</span></span>     |<span data-ttu-id="36659-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36659-118">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="36659-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36659-119">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="36659-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36659-120">Not supported.</span></span>|
|<span data-ttu-id="36659-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36659-121">Application</span></span>                            |<span data-ttu-id="36659-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36659-122">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="36659-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36659-123">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="36659-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36659-124">Request headers</span></span>

| <span data-ttu-id="36659-125">Nome</span><span class="sxs-lookup"><span data-stu-id="36659-125">Name</span></span>           | <span data-ttu-id="36659-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="36659-126">Type</span></span>    | <span data-ttu-id="36659-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="36659-127">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="36659-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="36659-128">Authorization</span></span>  | <span data-ttu-id="36659-129">string</span><span class="sxs-lookup"><span data-stu-id="36659-129">string</span></span>  | <span data-ttu-id="36659-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36659-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36659-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36659-132">Request body</span></span>

<span data-ttu-id="36659-133">No corpo da solicitação, fornece o [objeto synchronizationSchema](../resources/synchronization-synchronizationschema.md) para substituir o esquema existente por.</span><span class="sxs-lookup"><span data-stu-id="36659-133">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="36659-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="36659-134">Response</span></span>

<span data-ttu-id="36659-135">Se tiver êxito, retornará `204 No Content` um código de resposta.</span><span class="sxs-lookup"><span data-stu-id="36659-135">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="36659-136">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36659-136">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36659-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36659-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="36659-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36659-138">Request</span></span>
<span data-ttu-id="36659-139">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="36659-139">The following is an example of a request.</span></span>

><span data-ttu-id="36659-140">**Observação:** O objeto request mostrado aqui é reduzido para capacidade de leitura.</span><span class="sxs-lookup"><span data-stu-id="36659-140">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="36659-141">Fornecer todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36659-141">Supply all the properties in an actual call.</span></span>

# <a name="http"></a>[<span data-ttu-id="36659-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="36659-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="36659-143">C#</span><span class="sxs-lookup"><span data-stu-id="36659-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36659-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36659-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36659-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36659-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36659-146">Java</span><span class="sxs-lookup"><span data-stu-id="36659-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="36659-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="36659-147">Response</span></span>
<span data-ttu-id="36659-148">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="36659-148">The following is an example of a response.</span></span>
<!-- {
  "blockType": "response"
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


