---
title: 'directoryDefinition: descobrir'
description: 'Descubra a definição de esquema mais recente para provisionamento para um aplicativo. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 4b83168464b8f8ab563ffa549d601e35929684bb
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625882"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="814bd-103">directoryDefinition: descobrir</span><span class="sxs-lookup"><span data-stu-id="814bd-103">directoryDefinition: discover</span></span>

<span data-ttu-id="814bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="814bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="814bd-105">Descubra a definição de esquema mais recente para provisionamento para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="814bd-105">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="814bd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="814bd-106">Permissions</span></span>

<span data-ttu-id="814bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="814bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="814bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="814bd-109">Permission type</span></span>                        | <span data-ttu-id="814bd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="814bd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="814bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="814bd-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="814bd-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="814bd-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="814bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="814bd-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="814bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="814bd-114">Not supported.</span></span>|
|<span data-ttu-id="814bd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="814bd-115">Application</span></span>                            |<span data-ttu-id="814bd-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="814bd-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="814bd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="814bd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="814bd-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="814bd-118">Request headers</span></span>

| <span data-ttu-id="814bd-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="814bd-119">Header</span></span>        | <span data-ttu-id="814bd-120">Valor</span><span class="sxs-lookup"><span data-stu-id="814bd-120">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="814bd-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="814bd-121">Authorization</span></span> | <span data-ttu-id="814bd-122">{token} do portador (obrigatório)</span><span class="sxs-lookup"><span data-stu-id="814bd-122">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="814bd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="814bd-123">Request body</span></span>

<span data-ttu-id="814bd-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="814bd-124">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="814bd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="814bd-125">Response</span></span>

<span data-ttu-id="814bd-126">Se tiver êxito, este método retornará `200 OK` uma resposta com um objeto [directoryDefinition.](../resources/synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="814bd-126">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="814bd-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="814bd-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="814bd-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="814bd-128">Request</span></span>
<span data-ttu-id="814bd-129">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="814bd-129">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="814bd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="814bd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="c"></a>[<span data-ttu-id="814bd-131">C#</span><span class="sxs-lookup"><span data-stu-id="814bd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="814bd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="814bd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="814bd-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="814bd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="814bd-134">Java</span><span class="sxs-lookup"><span data-stu-id="814bd-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/discover-directorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="814bd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="814bd-135">Response</span></span>

<span data-ttu-id="814bd-136">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="814bd-136">The following is an example of a response.</span></span>

><span data-ttu-id="814bd-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="814bd-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "discoverabilities": "AttributeNames, AttributeDataTypes",
  "discoveryDateTime": "2019-03-20T15:47:50.4707552Z",
  "id": "directoryDefinitionId",
  "objects": [{
        "name": "User",
        "attributes": [{
                "name": "Id",
                "type": "String"
            }, {
                "name": "FirstName",
                "type": "String"
            },
            {
                "name": "CustomExendedAttribute",
                "type": "String"
            }  
        ]
    }],
  "version": "bf8c03ac-d45e-47fe-b3a1-711a9418b2b1"
}
 ```


