---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'Essa função retorna a URL do OneDrive onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados.  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 97730a35e107cbaa3f3901fac8eceb473e89c602
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436169"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="11e95-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="11e95-103">educationAssignment: getResourcesFolderUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11e95-104">Essa função retorna a URL do OneDrive onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados.</span><span class="sxs-lookup"><span data-stu-id="11e95-104">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="11e95-105">Observe que os arquivos devem estar localizados nessa pasta para serem adicionados como recursos.</span><span class="sxs-lookup"><span data-stu-id="11e95-105">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="11e95-106">Apenas um professor na turma pode determinar quais arquivos carregar.</span><span class="sxs-lookup"><span data-stu-id="11e95-106">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="11e95-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="11e95-107">Permissions</span></span>
<span data-ttu-id="11e95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11e95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11e95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11e95-110">Permission type</span></span>      | <span data-ttu-id="11e95-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11e95-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11e95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11e95-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="11e95-113">EduAssignments. ReadBasic, EduAssignments. Read</span><span class="sxs-lookup"><span data-stu-id="11e95-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="11e95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11e95-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="11e95-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11e95-115">Not supported.</span></span>  |
|<span data-ttu-id="11e95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11e95-116">Application</span></span> | <span data-ttu-id="11e95-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11e95-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="11e95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11e95-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="11e95-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11e95-119">Request headers</span></span>
| <span data-ttu-id="11e95-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="11e95-120">Header</span></span>       | <span data-ttu-id="11e95-121">Valor</span><span class="sxs-lookup"><span data-stu-id="11e95-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11e95-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="11e95-122">Authorization</span></span>  | <span data-ttu-id="11e95-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11e95-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11e95-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11e95-125">Request body</span></span>
<span data-ttu-id="11e95-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="11e95-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="11e95-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e95-127">Response</span></span>
<span data-ttu-id="11e95-128">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="11e95-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="11e95-129">O corpo conterá a URL do OneDrive de uma pasta na qual colocar todos os recursos baseados em arquivo.</span><span class="sxs-lookup"><span data-stu-id="11e95-129">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="11e95-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="11e95-130">Example</span></span>
<span data-ttu-id="11e95-131">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="11e95-131">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="11e95-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11e95-132">Request</span></span>
<span data-ttu-id="11e95-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="11e95-133">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="11e95-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="11e95-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="11e95-135">C#</span><span class="sxs-lookup"><span data-stu-id="11e95-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11e95-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="11e95-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11e95-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="11e95-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="11e95-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="11e95-138">Response</span></span>
<span data-ttu-id="11e95-139">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="11e95-139">The following is an example of a response.</span></span> 

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
