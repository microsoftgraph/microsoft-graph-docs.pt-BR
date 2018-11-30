---
title: 'educationAssignment: getResourcesFolderUrl'
description: 'Essa função retorna a URL de OneDrive onde todos os recursos com base em arquivo (Word, Excel e assim por diante) devem ser carregados.  '
ms.openlocfilehash: 129fa76d57e2016141397f967e833c765e737b19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038058"
---
# <a name="educationassignment-getresourcesfolderurl"></a><span data-ttu-id="cf5f6-103">educationAssignment: getResourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="cf5f6-103">educationAssignment: getResourcesFolderUrl</span></span>

> <span data-ttu-id="cf5f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf5f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf5f6-106">Essa função retorna a URL de OneDrive onde todos os recursos com base em arquivo (Word, Excel e assim por diante) devem ser carregados.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-106">This function returns the OneDrive URL where all file-based resources (Word, Excel, and so on) should be uploaded.</span></span>  
<span data-ttu-id="cf5f6-107">Observe que os arquivos devem estar localizados nesta pasta para ser adicionado como recursos.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-107">Note that files must be located in this folder in order to be added as resources.</span></span> <span data-ttu-id="cf5f6-108">Somente um professor na classe pode determinar quais arquivos para carregar.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-108">Only a teacher in the class can determine what files to upload.</span></span> 

## <a name="permissions"></a><span data-ttu-id="cf5f6-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="cf5f6-109">Permissions</span></span>
<span data-ttu-id="cf5f6-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf5f6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf5f6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf5f6-112">Permission type</span></span>      | <span data-ttu-id="cf5f6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf5f6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf5f6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf5f6-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="cf5f6-115">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="cf5f6-115">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="cf5f6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf5f6-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cf5f6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-117">Not supported.</span></span>  |
|<span data-ttu-id="cf5f6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf5f6-118">Application</span></span> | <span data-ttu-id="cf5f6-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cf5f6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf5f6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/getResourcesFolderUrl

```
## <a name="request-headers"></a><span data-ttu-id="cf5f6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5f6-121">Request headers</span></span>
| <span data-ttu-id="cf5f6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf5f6-122">Header</span></span>       | <span data-ttu-id="cf5f6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cf5f6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cf5f6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf5f6-124">Authorization</span></span>  | <span data-ttu-id="cf5f6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf5f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5f6-127">Request body</span></span>
<span data-ttu-id="cf5f6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cf5f6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf5f6-129">Response</span></span>
<span data-ttu-id="cf5f6-130">Se tiver êxito, este método retornará um código de resposta `200 Ok`.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-130">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="cf5f6-131">O corpo irá conter a URL de OneDrive de uma pasta na qual colocar todos os recursos baseados em arquivos.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-131">The body will contain the OneDrive URL of a folder in which to put all file-based resources.</span></span>

## <a name="example"></a><span data-ttu-id="cf5f6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf5f6-132">Example</span></span>
<span data-ttu-id="cf5f6-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-133">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cf5f6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf5f6-134">Request</span></span>
<span data-ttu-id="cf5f6-135">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-135">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/getResourcesFolderUrl
```

##### <a name="response"></a><span data-ttu-id="cf5f6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf5f6-136">Response</span></span>
<span data-ttu-id="cf5f6-137">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="cf5f6-137">The following is an example of a response.</span></span> 

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
