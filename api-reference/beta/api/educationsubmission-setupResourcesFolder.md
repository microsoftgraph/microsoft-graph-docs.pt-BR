---
title: 'educationSubmission: setUpResourcesFolder'
description: Acionar a criação da pasta de recursos SharePoint onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados para um determinado envio.
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d7be17b22434b08e5b83479201e59b17a91d26e1
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664762"
---
# <a name="educationsubmission-setupresourcesfolder"></a><span data-ttu-id="6e380-103">educationSubmission: setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="6e380-103">educationSubmission: setUpResourcesFolder</span></span>

<span data-ttu-id="6e380-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e380-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e380-105">Acionar a criação da pasta de recursos SharePoint onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados para um determinado envio.</span><span class="sxs-lookup"><span data-stu-id="6e380-105">Trigger the creation of the SharePoint resource folder where all file-based resources (Word, Excel, and so on) should be uploaded for a given submission.</span></span>

<span data-ttu-id="6e380-106">Observe que os arquivos devem estar localizados nesta pasta para serem adicionados como recursos.</span><span class="sxs-lookup"><span data-stu-id="6e380-106">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="6e380-107">Somente um aluno na classe pode determinar quais arquivos carregar em uma determinada pasta de recursos de nível de envio.</span><span class="sxs-lookup"><span data-stu-id="6e380-107">Only a student in the class can determine what files to upload in a given submission-level resource folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6e380-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e380-108">Permissions</span></span>
<span data-ttu-id="6e380-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e380-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e380-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e380-111">Permission type</span></span>      | <span data-ttu-id="6e380-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e380-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e380-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e380-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="6e380-114">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="6e380-114">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="6e380-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6e380-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6e380-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e380-116">Not supported.</span></span>  |
|<span data-ttu-id="6e380-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e380-117">Application</span></span> | <span data-ttu-id="6e380-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e380-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="6e380-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e380-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/setUpResourcesFolder
```

## <a name="request-headers"></a><span data-ttu-id="6e380-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e380-120">Request headers</span></span>
| <span data-ttu-id="6e380-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e380-121">Header</span></span>       | <span data-ttu-id="6e380-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6e380-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e380-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e380-123">Authorization</span></span>  | <span data-ttu-id="6e380-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e380-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e380-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e380-126">Request body</span></span>
<span data-ttu-id="6e380-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e380-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6e380-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e380-128">Response</span></span>
<span data-ttu-id="6e380-129">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="6e380-129">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="6e380-130">O corpo conterá o modelo de envio.</span><span class="sxs-lookup"><span data-stu-id="6e380-130">The body will contain the submission model.</span></span>

## <a name="example"></a><span data-ttu-id="6e380-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e380-131">Example</span></span>
<span data-ttu-id="6e380-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="6e380-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="6e380-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6e380-133">Request</span></span>
<span data-ttu-id="6e380-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e380-134">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6e380-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e380-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationsubmission_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/submissions/20302/setUpResourcesFolder
```
# <a name="c"></a>[<span data-ttu-id="6e380-136">C#</span><span class="sxs-lookup"><span data-stu-id="6e380-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationsubmission-setupresourcesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e380-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e380-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationsubmission-setupresourcesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e380-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e380-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationsubmission-setupresourcesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6e380-139">Java</span><span class="sxs-lookup"><span data-stu-id="6e380-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationsubmission-setupresourcesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="6e380-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e380-140">Response</span></span>
<span data-ttu-id="6e380-141">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="6e380-141">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions/$entity",
    "status": "working",
    "submittedDateTime": null,
    "unsubmittedDateTime": null,
    "returnedDateTime": null,
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!6SQl0y4WHkS2P5MeIsSGpKwfynEIaD1OvPVeH4wbOp_1uyhNwJMSSpseJneB7Z4F/items/01YT2AIJRQLVYT24IWWFAJHMRRNYCB3GE2",
    "id": "803fb5dd-3553-455f-3d94-f79fb54a1003",
    "recipient": {
        "@odata.type": "#microsoft.graph.educationSubmissionIndividualRecipient",
        "userId": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1"
    },
    "submittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "f8bbb2a4-2cdd-4d49-ac81-d4113fc72dc1",
            "displayName": null
        }
    },
    "unsubmittedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "returnedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": null,
            "displayName": null
        }
    },
    "resources@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions('803fb5dd-3553-455f-3d94-f79fb54a1003')/resources",
    "resources": [],
    "submittedResources@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('b07edbef-7420-4b3d-8f7c-d599cf21e069')/assignments('1e5222bd-b7d2-4d64-8a22-74b722ce2fc6')/submissions('803fb5dd-3553-455f-3d94-f79fb54a1003')/submittedResources",
    "submittedResources": []
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-d4113fc72dc1
2021-05-12 12:00:00 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission: setUpResourcesFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


