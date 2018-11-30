---
title: Obter synchronizationSchema
description: Recupere o esquema de um modelo ou um trabalho de sincronização de determinado.
ms.openlocfilehash: 93624a334c928b6402851ebc566e6e29e341ca1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034734"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="bd8a8-103">Obter synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="bd8a8-103">Get synchronizationSchema</span></span>

> <span data-ttu-id="bd8a8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd8a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd8a8-106">Recupere o esquema de um modelo ou um trabalho de sincronização de determinado.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-106">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd8a8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="bd8a8-107">Permissions</span></span>
<span data-ttu-id="bd8a8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd8a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd8a8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd8a8-110">Permission type</span></span>                        | <span data-ttu-id="bd8a8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd8a8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd8a8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd8a8-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="bd8a8-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd8a8-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="bd8a8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd8a8-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="bd8a8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-115">Not supported.</span></span> |
|<span data-ttu-id="bd8a8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd8a8-116">Application</span></span>                            |<span data-ttu-id="bd8a8-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bd8a8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd8a8-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="bd8a8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd8a8-119">Request headers</span></span>

| <span data-ttu-id="bd8a8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="bd8a8-120">Name</span></span>           | <span data-ttu-id="bd8a8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd8a8-121">Type</span></span>    | <span data-ttu-id="bd8a8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd8a8-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="bd8a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd8a8-123">Authorization</span></span>  | <span data-ttu-id="bd8a8-124">string</span><span class="sxs-lookup"><span data-stu-id="bd8a8-124">string</span></span>  | <span data-ttu-id="bd8a8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd8a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd8a8-127">Request body</span></span>

<span data-ttu-id="bd8a8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd8a8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd8a8-129">Response</span></span>

<span data-ttu-id="bd8a8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [synchronizationSchema](../resources/synchronization-synchronizationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-130">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd8a8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bd8a8-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bd8a8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd8a8-132">Request</span></span>
<span data-ttu-id="bd8a8-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

##### <a name="response"></a><span data-ttu-id="bd8a8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd8a8-134">Response</span></span>
<span data-ttu-id="bd8a8-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-135">The following is an example of a response.</span></span>

><span data-ttu-id="bd8a8-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bd8a8-137">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd8a8-137">All the properties will be returned in an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->