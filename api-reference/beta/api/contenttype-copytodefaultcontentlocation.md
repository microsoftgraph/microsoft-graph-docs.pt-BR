---
author: swapnil1993
title: 'contentType: copyToDefaultContentLocation'
description: Copie um arquivo para um local de conteúdo padrão em um tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: afe4a5aebe4e19dd3957e0be0cca334a33035981
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201978"
---
# <a name="contenttype-copytodefaultcontentlocation"></a><span data-ttu-id="4d0a3-103">contentType: copyToDefaultContentLocation</span><span class="sxs-lookup"><span data-stu-id="4d0a3-103">contentType: copyToDefaultContentLocation</span></span>
<span data-ttu-id="4d0a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d0a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="4d0a3-105">Copie um arquivo para um local de conteúdo padrão em um [tipo de conteúdo][contentType].</span><span class="sxs-lookup"><span data-stu-id="4d0a3-105">Copy a file to a default content location in a [content type][contentType].</span></span> <span data-ttu-id="4d0a3-106">Em seguida, o arquivo pode ser adicionado como um arquivo ou modelo padrão por meio de uma operação POST.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-106">The file can then be added as a default file or template via a POST operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d0a3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d0a3-107">Permissions</span></span>  

<span data-ttu-id="4d0a3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d0a3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

  

|<span data-ttu-id="4d0a3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d0a3-110">Permission type</span></span> | <span data-ttu-id="4d0a3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d0a3-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d0a3-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d0a3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4d0a3-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="4d0a3-113">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>  |
|<span data-ttu-id="4d0a3-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d0a3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d0a3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-115">Not supported.</span></span> |
|<span data-ttu-id="4d0a3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d0a3-116">Application</span></span> | <span data-ttu-id="4d0a3-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="4d0a3-117">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="4d0a3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d0a3-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /sites/id/contentTypes/id/copyToDefaultContentLocation 
```

## <a name="request-headers"></a><span data-ttu-id="4d0a3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0a3-119">Request headers</span></span>
|<span data-ttu-id="4d0a3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4d0a3-120">Name</span></span>|<span data-ttu-id="4d0a3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d0a3-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4d0a3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d0a3-122">Authorization</span></span>|<span data-ttu-id="4d0a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4d0a3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d0a3-125">Content-Type</span></span>|<span data-ttu-id="4d0a3-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d0a3-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0a3-128">Request body</span></span>
<span data-ttu-id="4d0a3-129">No corpo da solicitação, fornece uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-129">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="4d0a3-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-130">The following table shows the parameters that can be used with this action.</span></span>


|<span data-ttu-id="4d0a3-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4d0a3-131">Parameter</span></span>|<span data-ttu-id="4d0a3-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d0a3-132">Type</span></span>|<span data-ttu-id="4d0a3-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d0a3-133">Description</span></span>|
|-|-|-|
|<span data-ttu-id="4d0a3-134">sourceFile</span><span class="sxs-lookup"><span data-stu-id="4d0a3-134">sourceFile</span></span>| [<span data-ttu-id="4d0a3-135">itemReference</span><span class="sxs-lookup"><span data-stu-id="4d0a3-135">itemReference</span></span>](../resources/itemreference.md) |<span data-ttu-id="4d0a3-136">Metadados sobre o arquivo de origem que precisa ser copiado para o local de conteúdo padrão.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-136">Metadata about the source file that needs to be copied to the default content location.</span></span> <span data-ttu-id="4d0a3-137">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-137">Required.</span></span>|
|<span data-ttu-id="4d0a3-138">destinationFileName</span><span class="sxs-lookup"><span data-stu-id="4d0a3-138">destinationFileName</span></span>| <span data-ttu-id="4d0a3-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d0a3-139">string</span></span> |<span data-ttu-id="4d0a3-140">Nome do arquivo de destino.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-140">Destination filename.</span></span> 

## <a name="response"></a><span data-ttu-id="4d0a3-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d0a3-141">Response</span></span>


<span data-ttu-id="4d0a3-142">Se tiver êxito, essa chamada retornará uma `204 No Content` resposta.</span><span class="sxs-lookup"><span data-stu-id="4d0a3-142">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="4d0a3-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d0a3-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d0a3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d0a3-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4d0a3-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d0a3-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_copytodefaultcontentlocation"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{id}/contentTypes/{contentTypeId}/copyToDefaultContentLocation 
Content-Type: application/json

{
   "sourceFile":{
      "sharepointIds":{
         "listId":"e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0",
         "listItemId":"2"
      }
   },
   "destinationFileName":"newname.txt"
}
```
# <a name="c"></a>[<span data-ttu-id="4d0a3-146">C#</span><span class="sxs-lookup"><span data-stu-id="4d0a3-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-copytodefaultcontentlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d0a3-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d0a3-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-copytodefaultcontentlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d0a3-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d0a3-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-copytodefaultcontentlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d0a3-149">Java</span><span class="sxs-lookup"><span data-stu-id="4d0a3-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-copytodefaultcontentlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




### <a name="response"></a><span data-ttu-id="4d0a3-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d0a3-150">Response</span></span>


<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

  

[contentType]: ../resources/contentType.md
