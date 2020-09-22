---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'Essa função retorna a URL do OneDrive onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados.  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0184f1cfafe25fc1222c48b12f24391c126a6443
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007809"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="c89f5-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="c89f5-103">educationAssignment: getResourcesFolderUrl</span></span>

<span data-ttu-id="c89f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c89f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c89f5-105">Essa função retorna a URL do OneDrive onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados.</span><span class="sxs-lookup"><span data-stu-id="c89f5-105">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="c89f5-106">Observe que os arquivos devem estar localizados nessa pasta para serem adicionados como recursos.</span><span class="sxs-lookup"><span data-stu-id="c89f5-106">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="c89f5-107">Apenas um professor na turma pode determinar quais arquivos carregar.</span><span class="sxs-lookup"><span data-stu-id="c89f5-107">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c89f5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c89f5-108">Permissions</span></span>
<span data-ttu-id="c89f5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c89f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c89f5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c89f5-111">Permission type</span></span>      | <span data-ttu-id="c89f5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c89f5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c89f5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c89f5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c89f5-114">EduAssignments. ReadBasic, EduAssignments. Read</span><span class="sxs-lookup"><span data-stu-id="c89f5-114">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="c89f5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c89f5-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c89f5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c89f5-116">Not supported.</span></span>  |
|<span data-ttu-id="c89f5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c89f5-117">Application</span></span> | <span data-ttu-id="c89f5-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c89f5-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c89f5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c89f5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="c89f5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c89f5-120">Request headers</span></span>
| <span data-ttu-id="c89f5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c89f5-121">Header</span></span>       | <span data-ttu-id="c89f5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c89f5-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c89f5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c89f5-123">Authorization</span></span>  | <span data-ttu-id="c89f5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c89f5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c89f5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c89f5-126">Request body</span></span>
<span data-ttu-id="c89f5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c89f5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c89f5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c89f5-128">Response</span></span>
<span data-ttu-id="c89f5-129">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="c89f5-129">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="c89f5-130">O corpo conterá a URL do OneDrive de uma pasta na qual colocar todos os recursos baseados em arquivo.</span><span class="sxs-lookup"><span data-stu-id="c89f5-130">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="c89f5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c89f5-131">Example</span></span>
<span data-ttu-id="c89f5-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c89f5-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c89f5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c89f5-133">Request</span></span>
<span data-ttu-id="c89f5-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c89f5-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c89f5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c89f5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="c"></a>[<span data-ttu-id="c89f5-136">C#</span><span class="sxs-lookup"><span data-stu-id="c89f5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c89f5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c89f5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c89f5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c89f5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c89f5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c89f5-139">Response</span></span>
<span data-ttu-id="c89f5-140">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c89f5-140">The following is an example of a response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Edm.String",
    "value": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


