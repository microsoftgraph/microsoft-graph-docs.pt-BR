---
title: 'educationAssignment: getResourcesFolderUrl (preterido)'
description: 'Essa função retorna a URL OneDrive onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados.  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 44c7caec25b4d96b225598041f59bfcaa3f5d3ac
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/01/2021
ms.locfileid: "52119002"
---
# <a name="educationassignment-getresourcesfolderurl-deprecated"></a><span data-ttu-id="80c6c-103">educationAssignment: getResourcesFolderUrl (preterido)</span><span class="sxs-lookup"><span data-stu-id="80c6c-103">educationAssignment: getResourcesFolderUrl (deprecated)</span></span>

<span data-ttu-id="80c6c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80c6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 [!CAUTION] <span data-ttu-id="80c6c-105">A API getResourcesFolderUrl está preterida e interromperá o retorno de dados em 31 de maio de 2021.</span><span class="sxs-lookup"><span data-stu-id="80c6c-105">The getResourcesFolderUrl API is deprecated and will stop returning data on May 31, 2021.</span></span> <span data-ttu-id="80c6c-106">Use a nova propriedade exposta `resourcesFolderUrl` na entidade [educationAssignment](../resources/educationassignment.md) para buscar essas informações.</span><span class="sxs-lookup"><span data-stu-id="80c6c-106">Please use the new property `resourcesFolderUrl` exposed on [educationAssignment](../resources/educationassignment.md) entity to fetch this info.</span></span> 

<span data-ttu-id="80c6c-107">Essa função retorna a URL OneDrive onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados.</span><span class="sxs-lookup"><span data-stu-id="80c6c-107">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="80c6c-108">Observe que os arquivos devem estar localizados nesta pasta para serem adicionados como recursos.</span><span class="sxs-lookup"><span data-stu-id="80c6c-108">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="80c6c-109">Somente um professor da classe pode determinar quais arquivos carregar.</span><span class="sxs-lookup"><span data-stu-id="80c6c-109">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="80c6c-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="80c6c-110">Permissions</span></span>
<span data-ttu-id="80c6c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80c6c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80c6c-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80c6c-113">Permission type</span></span>      | <span data-ttu-id="80c6c-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80c6c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80c6c-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80c6c-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="80c6c-116">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="80c6c-116">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="80c6c-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80c6c-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="80c6c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80c6c-118">Not supported.</span></span>  |
|<span data-ttu-id="80c6c-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80c6c-119">Application</span></span> | <span data-ttu-id="80c6c-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80c6c-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="80c6c-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80c6c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="80c6c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80c6c-122">Request headers</span></span>
| <span data-ttu-id="80c6c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80c6c-123">Header</span></span>       | <span data-ttu-id="80c6c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="80c6c-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="80c6c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="80c6c-125">Authorization</span></span>  | <span data-ttu-id="80c6c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80c6c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="80c6c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80c6c-128">Request body</span></span>
<span data-ttu-id="80c6c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="80c6c-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="80c6c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="80c6c-130">Response</span></span>
<span data-ttu-id="80c6c-131">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="80c6c-131">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="80c6c-132">O corpo conterá a URL OneDrive de uma pasta na qual todos os recursos baseados em arquivo serão colocados.</span><span class="sxs-lookup"><span data-stu-id="80c6c-132">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="80c6c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80c6c-133">Example</span></span>
<span data-ttu-id="80c6c-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="80c6c-134">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="80c6c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80c6c-135">Request</span></span>
<span data-ttu-id="80c6c-136">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="80c6c-136">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80c6c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="80c6c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="c"></a>[<span data-ttu-id="80c6c-138">C#</span><span class="sxs-lookup"><span data-stu-id="80c6c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80c6c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80c6c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80c6c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80c6c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80c6c-141">Java</span><span class="sxs-lookup"><span data-stu-id="80c6c-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="80c6c-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="80c6c-142">Response</span></span>
<span data-ttu-id="80c6c-143">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="80c6c-143">The following is an example of a response.</span></span> 

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


