---
title: Obter foto
description: Recupere as propriedades e os relacionamentos do objeto de foto.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 48ba8ef11dedc266a24cb84dc29dd4de1bd9af81
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730061"
---
# <a name="get-photo"></a><span data-ttu-id="d326d-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="d326d-103">Get photo</span></span>

<span data-ttu-id="d326d-104">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="d326d-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d326d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d326d-105">Permissions</span></span>
<span data-ttu-id="d326d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d326d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d326d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d326d-108">Permission type</span></span>      | <span data-ttu-id="d326d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d326d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d326d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d326d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d326d-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="d326d-111">Files.Read</span></span>    |
|<span data-ttu-id="d326d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d326d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d326d-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="d326d-113">Files.Read</span></span>    |
|<span data-ttu-id="d326d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d326d-114">Application</span></span> | <span data-ttu-id="d326d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d326d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d326d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d326d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d326d-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d326d-117">Optional query parameters</span></span>
<span data-ttu-id="d326d-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d326d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d326d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d326d-119">Request headers</span></span>
| <span data-ttu-id="d326d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d326d-120">Name</span></span>       | <span data-ttu-id="d326d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d326d-121">Type</span></span> | <span data-ttu-id="d326d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d326d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d326d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d326d-123">Authorization</span></span>  | <span data-ttu-id="d326d-124">string</span><span class="sxs-lookup"><span data-stu-id="d326d-124">string</span></span>  | <span data-ttu-id="d326d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d326d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d326d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d326d-127">Request body</span></span>
<span data-ttu-id="d326d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d326d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d326d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d326d-129">Response</span></span>

<span data-ttu-id="d326d-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d326d-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d326d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d326d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d326d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d326d-132">Request</span></span>
<span data-ttu-id="d326d-133">Veja a seguir um exemplo de solicitação de metadados de fotos.</span><span class="sxs-lookup"><span data-stu-id="d326d-133">Here is an example of the request for photo metadata.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d326d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d326d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d326d-135">C#</span><span class="sxs-lookup"><span data-stu-id="d326d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d326d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d326d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d326d-137">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d326d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d326d-138">Java</span><span class="sxs-lookup"><span data-stu-id="d326d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d326d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d326d-139">Response</span></span>
<span data-ttu-id="d326d-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d326d-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="request"></a><span data-ttu-id="d326d-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d326d-141">Request</span></span>
<span data-ttu-id="d326d-142">Veja a seguir um exemplo de solicitação de bytes de fotos.</span><span class="sxs-lookup"><span data-stu-id="d326d-142">Here is an example of the request for the photo bytes.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d326d-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d326d-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d326d-144">C#</span><span class="sxs-lookup"><span data-stu-id="d326d-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d326d-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d326d-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d326d-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="d326d-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d326d-147">Java</span><span class="sxs-lookup"><span data-stu-id="d326d-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d326d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="d326d-148">Response</span></span>
<span data-ttu-id="d326d-149">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d326d-149">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Edm.Stream" } -->

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: image/jpeg
ETag: "A19A6498"
request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
client-request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
x-ms-ags-diagnostic: {"ServerInfo":{"DataCenter":"West US","Slice":"SliceA","Ring":"5","ScaleUnit":"003","Host":"AGSFE_IN_14","ADSiteName":"WST"}}
Access-Control-Allow-Origin: *
Access-Control-Expose-Headers: ETag, Location, Preference-Applied, Content-Range, request-id, client-request-id
Duration: 125.9389
Date: Wed, 13 Dec 2017 22:02:17 GMT
Content-Length: 250526

<binary image data>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
