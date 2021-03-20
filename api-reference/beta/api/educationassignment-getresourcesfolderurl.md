---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'Essa função retorna a URL do OneDrive onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados.  '
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ce5f35560a25f2a57742d93293788038e13cb179
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951830"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="3a041-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="3a041-103">educationAssignment: getResourcesFolderUrl</span></span>

<span data-ttu-id="3a041-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a041-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a041-105">Essa função retorna a URL do OneDrive onde todos os recursos baseados em arquivo (Word, Excel e assim por diante) devem ser carregados.</span><span class="sxs-lookup"><span data-stu-id="3a041-105">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="3a041-106">Observe que os arquivos devem estar localizados nesta pasta para serem adicionados como recursos.</span><span class="sxs-lookup"><span data-stu-id="3a041-106">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="3a041-107">Somente um professor da classe pode determinar quais arquivos carregar.</span><span class="sxs-lookup"><span data-stu-id="3a041-107">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3a041-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3a041-108">Permissions</span></span>
<span data-ttu-id="3a041-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a041-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a041-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3a041-111">Permission type</span></span>      | <span data-ttu-id="3a041-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3a041-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a041-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3a041-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="3a041-114">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="3a041-114">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="3a041-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3a041-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3a041-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a041-116">Not supported.</span></span>  |
|<span data-ttu-id="3a041-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3a041-117">Application</span></span> | <span data-ttu-id="3a041-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3a041-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3a041-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3a041-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="3a041-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3a041-120">Request headers</span></span>
| <span data-ttu-id="3a041-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3a041-121">Header</span></span>       | <span data-ttu-id="3a041-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3a041-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a041-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3a041-123">Authorization</span></span>  | <span data-ttu-id="3a041-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3a041-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a041-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3a041-126">Request body</span></span>
<span data-ttu-id="3a041-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3a041-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3a041-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a041-128">Response</span></span>
<span data-ttu-id="3a041-129">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="3a041-129">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="3a041-130">O corpo conterá a URL do OneDrive de uma pasta na qual todos os recursos baseados em arquivo serão colocados.</span><span class="sxs-lookup"><span data-stu-id="3a041-130">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="3a041-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a041-131">Example</span></span>
<span data-ttu-id="3a041-132">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3a041-132">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3a041-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3a041-133">Request</span></span>
<span data-ttu-id="3a041-134">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="3a041-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3a041-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a041-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```
# <a name="c"></a>[<span data-ttu-id="3a041-136">C#</span><span class="sxs-lookup"><span data-stu-id="3a041-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-publish-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a041-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a041-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-publish-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a041-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a041-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-publish-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a041-139">Java</span><span class="sxs-lookup"><span data-stu-id="3a041-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-publish-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3a041-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="3a041-140">Response</span></span>
<span data-ttu-id="3a041-141">Veja a seguir um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="3a041-141">The following is an example of a response.</span></span> 

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


