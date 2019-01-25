---
title: Atualizar synchronizationSchema
description: Atualize o esquema de sincronização para um determinado trabalho ou de um modelo. Esse método substitui totalmente o esquema atual com aquele fornecido na solicitação. Para atualizar o esquema de um modelo, faça a chamada no objeto application. Você deve ser o proprietário do aplicativo.
localization_priority: Normal
ms.openlocfilehash: 13ee7d996b0e02834b77cd222380747c02d7fcc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525546"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="e2a81-106">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="e2a81-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2a81-107">Atualize o esquema de sincronização para um determinado trabalho ou de um modelo.</span><span class="sxs-lookup"><span data-stu-id="e2a81-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="e2a81-108">Esse método substitui totalmente o esquema atual com aquele fornecido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2a81-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="e2a81-109">Para atualizar o esquema de um modelo, faça a chamada no objeto application.</span><span class="sxs-lookup"><span data-stu-id="e2a81-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="e2a81-110">Você deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2a81-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2a81-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2a81-111">Permissions</span></span>
<span data-ttu-id="e2a81-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2a81-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2a81-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2a81-114">Permission type</span></span>                        | <span data-ttu-id="e2a81-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2a81-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2a81-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2a81-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="e2a81-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2a81-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e2a81-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2a81-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e2a81-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2a81-119">Not supported.</span></span>|
|<span data-ttu-id="e2a81-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2a81-120">Application</span></span>                            |<span data-ttu-id="e2a81-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2a81-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="e2a81-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2a81-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="e2a81-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a81-123">Request headers</span></span>

| <span data-ttu-id="e2a81-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e2a81-124">Name</span></span>           | <span data-ttu-id="e2a81-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2a81-125">Type</span></span>    | <span data-ttu-id="e2a81-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2a81-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e2a81-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2a81-127">Authorization</span></span>  | <span data-ttu-id="e2a81-128">string</span><span class="sxs-lookup"><span data-stu-id="e2a81-128">string</span></span>  | <span data-ttu-id="e2a81-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2a81-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2a81-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a81-131">Request body</span></span>

<span data-ttu-id="e2a81-132">No corpo da solicitação, fornece o objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) para substituir o esquema existente com.</span><span class="sxs-lookup"><span data-stu-id="e2a81-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="e2a81-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a81-133">Response</span></span>

<span data-ttu-id="e2a81-134">Se tiver êxito, retorna um `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a81-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="e2a81-135">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a81-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2a81-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2a81-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2a81-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2a81-137">Request</span></span>
<span data-ttu-id="e2a81-138">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2a81-138">The following is an example of a request.</span></span>

><span data-ttu-id="e2a81-139">**Observação:** O objeto request mostrado aqui é abreviado para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2a81-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="e2a81-140">Fornece todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2a81-140">Supply all the properties in an actual call.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema

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

##### <a name="response"></a><span data-ttu-id="e2a81-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2a81-141">Response</span></span>
<span data-ttu-id="e2a81-142">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="e2a81-142">The following is an example of a response.</span></span>
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
