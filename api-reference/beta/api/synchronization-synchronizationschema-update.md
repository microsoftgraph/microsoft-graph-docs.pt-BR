---
title: Atualizar synchronizationSchema
description: Atualize o esquema de sincronização para um determinado trabalho ou de um modelo. Esse método substitui totalmente o esquema atual com aquele fornecido na solicitação. Para atualizar o esquema de um modelo, faça a chamada no objeto application. Você deve ser o proprietário do aplicativo.
localization_priority: Normal
ms.openlocfilehash: d4f3f3540fe0d304b4edc3a5fcaec7b3366dbb0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826135"
---
# <a name="update-synchronizationschema"></a><span data-ttu-id="caca6-106">Atualizar synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="caca6-106">Update synchronizationSchema</span></span>

> <span data-ttu-id="caca6-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="caca6-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="caca6-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="caca6-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="caca6-109">Atualize o esquema de sincronização para um determinado trabalho ou de um modelo.</span><span class="sxs-lookup"><span data-stu-id="caca6-109">Update the synchronization schema for a given job or template.</span></span> <span data-ttu-id="caca6-110">Esse método substitui totalmente o esquema atual com aquele fornecido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="caca6-110">This method fully replaces the current schema with the one provided in the request.</span></span> <span data-ttu-id="caca6-111">Para atualizar o esquema de um modelo, faça a chamada no objeto application.</span><span class="sxs-lookup"><span data-stu-id="caca6-111">To update the schema of a template, make the call on the application object.</span></span> <span data-ttu-id="caca6-112">Você deve ser o proprietário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="caca6-112">You must be the owner of the application.</span></span>

## <a name="permissions"></a><span data-ttu-id="caca6-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="caca6-113">Permissions</span></span>
<span data-ttu-id="caca6-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caca6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caca6-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="caca6-116">Permission type</span></span>                        | <span data-ttu-id="caca6-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="caca6-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="caca6-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="caca6-118">Delegated (work or school account)</span></span>     |<span data-ttu-id="caca6-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caca6-119">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="caca6-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="caca6-120">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="caca6-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caca6-121">Not supported.</span></span>|
|<span data-ttu-id="caca6-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="caca6-122">Application</span></span>                            |<span data-ttu-id="caca6-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="caca6-123">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="caca6-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="caca6-124">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="caca6-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="caca6-125">Request headers</span></span>

| <span data-ttu-id="caca6-126">Nome</span><span class="sxs-lookup"><span data-stu-id="caca6-126">Name</span></span>           | <span data-ttu-id="caca6-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="caca6-127">Type</span></span>    | <span data-ttu-id="caca6-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="caca6-128">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="caca6-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="caca6-129">Authorization</span></span>  | <span data-ttu-id="caca6-130">string</span><span class="sxs-lookup"><span data-stu-id="caca6-130">string</span></span>  | <span data-ttu-id="caca6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="caca6-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="caca6-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="caca6-133">Request body</span></span>

<span data-ttu-id="caca6-134">No corpo da solicitação, fornece o objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) para substituir o esquema existente com.</span><span class="sxs-lookup"><span data-stu-id="caca6-134">In the request body, supply the [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object to replace the existing schema with.</span></span>

## <a name="response"></a><span data-ttu-id="caca6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="caca6-135">Response</span></span>

<span data-ttu-id="caca6-136">Se tiver êxito, retorna um `204 No Content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="caca6-136">If successful, returns a `204 No Content` response code.</span></span> <span data-ttu-id="caca6-137">Ele não retornará nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="caca6-137">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caca6-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="caca6-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="caca6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="caca6-139">Request</span></span>
<span data-ttu-id="caca6-140">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="caca6-140">The following is an example of a request.</span></span>

><span data-ttu-id="caca6-141">**Observação:** O objeto request mostrado aqui é abreviado para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="caca6-141">**Note:** The request object shown here is shortened for readability.</span></span> <span data-ttu-id="caca6-142">Fornece todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="caca6-142">Supply all the properties in an actual call.</span></span>
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

##### <a name="response"></a><span data-ttu-id="caca6-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="caca6-143">Response</span></span>
<span data-ttu-id="caca6-144">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="caca6-144">The following is an example of a response.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
