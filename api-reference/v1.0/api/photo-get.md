---
title: Obter foto
description: Recupere as propriedades e os relacionamentos do objeto de foto.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8f2aac2615c570e245b39b37006e12743c48da6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511023"
---
# <a name="get-photo"></a><span data-ttu-id="d059c-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="d059c-103">Get photo</span></span>

<span data-ttu-id="d059c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d059c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d059c-105">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="d059c-105">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d059c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d059c-106">Permissions</span></span>
<span data-ttu-id="d059c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d059c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d059c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d059c-109">Permission type</span></span>      | <span data-ttu-id="d059c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d059c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d059c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d059c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d059c-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="d059c-112">Files.Read</span></span>    |
|<span data-ttu-id="d059c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d059c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d059c-114">Files.Read</span><span class="sxs-lookup"><span data-stu-id="d059c-114">Files.Read</span></span>    |
|<span data-ttu-id="d059c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d059c-115">Application</span></span> | <span data-ttu-id="d059c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d059c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d059c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d059c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d059c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d059c-118">Optional query parameters</span></span>
<span data-ttu-id="d059c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d059c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d059c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d059c-120">Request headers</span></span>
| <span data-ttu-id="d059c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="d059c-121">Name</span></span>       | <span data-ttu-id="d059c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="d059c-122">Type</span></span> | <span data-ttu-id="d059c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d059c-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d059c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d059c-124">Authorization</span></span>  | <span data-ttu-id="d059c-125">string</span><span class="sxs-lookup"><span data-stu-id="d059c-125">string</span></span>  | <span data-ttu-id="d059c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d059c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d059c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d059c-128">Request body</span></span>
<span data-ttu-id="d059c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d059c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d059c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d059c-130">Response</span></span>

<span data-ttu-id="d059c-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d059c-131">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d059c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d059c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d059c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d059c-133">Request</span></span>
<span data-ttu-id="d059c-134">Veja a seguir um exemplo de solicitação de metadados de fotos.</span><span class="sxs-lookup"><span data-stu-id="d059c-134">Here is an example of the request for photo metadata.</span></span>

# <a name="http"></a>[<span data-ttu-id="d059c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d059c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="c"></a>[<span data-ttu-id="d059c-136">C#</span><span class="sxs-lookup"><span data-stu-id="d059c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d059c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d059c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d059c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d059c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d059c-139">Java</span><span class="sxs-lookup"><span data-stu-id="d059c-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d059c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d059c-140">Response</span></span>
<span data-ttu-id="d059c-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d059c-141">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="d059c-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d059c-142">Request</span></span>
<span data-ttu-id="d059c-143">Veja a seguir um exemplo de solicitação de bytes de fotos.</span><span class="sxs-lookup"><span data-stu-id="d059c-143">Here is an example of the request for the photo bytes.</span></span>

# <a name="http"></a>[<span data-ttu-id="d059c-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d059c-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
# <a name="c"></a>[<span data-ttu-id="d059c-145">C#</span><span class="sxs-lookup"><span data-stu-id="d059c-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d059c-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d059c-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d059c-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d059c-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d059c-148">Java</span><span class="sxs-lookup"><span data-stu-id="d059c-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-photo-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d059c-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d059c-149">Response</span></span>
<span data-ttu-id="d059c-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d059c-150">Here is an example of the response.</span></span>

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
