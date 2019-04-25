---
title: Atualizar synchronizationSchema
description: Atualize o esquema de sincronização de um determinado trabalho ou modelo. Esse método substitui completamente o esquema atual pelo fornecido na solicitação. Para atualizar o esquema de um modelo, faça a chamada no objeto Application. Você deve ser o proprietário do aplicativo.
localization_priority: Normal
ms.openlocfilehash: 13ee7d996b0e02834b77cd222380747c02d7fcc2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536954"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="0d789-106">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="0d789-106">Update synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d789-107">Atualize o esquema de sincronização de um determinado trabalho ou modelo.</span><span class="sxs-lookup"><span data-stu-id="0d789-107">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="0d789-108">Esse método substitui completamente o esquema atual pelo fornecido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d789-108">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="0d789-109">Para atualizar o esquema de um modelo, faça a chamada no objeto Application.</span><span class="sxs-lookup"><span data-stu-id="0d789-109">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="0d789-110">Você deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0d789-110">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d789-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d789-111">Permissions</span></span>
<span data-ttu-id="0d789-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d789-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d789-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d789-114">Permission type</span></span>                        | <span data-ttu-id="0d789-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d789-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d789-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d789-116">Delegated (work or school account)</span></span>     |<span data-ttu-id="0d789-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d789-117">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0d789-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d789-118">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0d789-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d789-119">Not supported.</span></span>|
|<span data-ttu-id="0d789-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d789-120">Application</span></span>                            |<span data-ttu-id="0d789-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d789-121">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="0d789-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d789-122">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="0d789-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d789-123">Request headers</span></span>

| <span data-ttu-id="0d789-124">Nome</span><span class="sxs-lookup"><span data-stu-id="0d789-124">Name</span></span>           | <span data-ttu-id="0d789-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d789-125">Type</span></span>    | <span data-ttu-id="0d789-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d789-126">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="0d789-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d789-127">Authorization</span></span>  | <span data-ttu-id="0d789-128">string</span><span class="sxs-lookup"><span data-stu-id="0d789-128">string</span></span>  | <span data-ttu-id="0d789-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0d789-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d789-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d789-131">Request body</span></span>

<span data-ttu-id="0d789-132">No corpo da solicitação, forneça o objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) para substituir o esquema existente por.</span><span class="sxs-lookup"><span data-stu-id="0d789-132">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="0d789-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d789-133">Response</span></span>

<span data-ttu-id="0d789-134">Se bem-sucedido, retorna um `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d789-134">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="0d789-135">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0d789-135">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d789-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0d789-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0d789-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d789-137">Request</span></span>
<span data-ttu-id="0d789-138">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d789-138">The following is an example of a request.</span></span>

><span data-ttu-id="0d789-139">**Observação:** O objeto Request mostrado aqui é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0d789-139">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="0d789-140">Forneça todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0d789-140">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="0d789-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d789-141">Response</span></span>
<span data-ttu-id="0d789-142">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0d789-142">The following is an example of a response.</span></span>
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
