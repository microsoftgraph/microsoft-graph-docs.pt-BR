---
title: Obter foto
description: Recupere as propriedades e os relacionamentos do objeto de foto.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: MSGraphDocsVteam
ms.openlocfilehash: 5f010abf89299b9e25660205f5180c2bd068af57
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806762"
---
# <a name="get-photo"></a><span data-ttu-id="3ff9c-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="3ff9c-103">Get photo</span></span>

<span data-ttu-id="3ff9c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ff9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ff9c-105">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-105">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ff9c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ff9c-106">Permissions</span></span>
<span data-ttu-id="3ff9c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ff9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ff9c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ff9c-109">Permission type</span></span>      | <span data-ttu-id="3ff9c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ff9c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ff9c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ff9c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ff9c-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="3ff9c-112">Files.Read</span></span>    |
|<span data-ttu-id="3ff9c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ff9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ff9c-114">Files.Read</span><span class="sxs-lookup"><span data-stu-id="3ff9c-114">Files.Read</span></span>    |
|<span data-ttu-id="3ff9c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ff9c-115">Application</span></span> | <span data-ttu-id="3ff9c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ff9c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ff9c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ff9c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ff9c-118">Optional query parameters</span></span>
<span data-ttu-id="3ff9c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ff9c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ff9c-120">Request headers</span></span>
| <span data-ttu-id="3ff9c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3ff9c-121">Name</span></span>       | <span data-ttu-id="3ff9c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ff9c-122">Type</span></span> | <span data-ttu-id="3ff9c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ff9c-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ff9c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ff9c-124">Authorization</span></span>  | <span data-ttu-id="3ff9c-125">string</span><span class="sxs-lookup"><span data-stu-id="3ff9c-125">string</span></span>  | <span data-ttu-id="3ff9c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ff9c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ff9c-128">Request body</span></span>
<span data-ttu-id="3ff9c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ff9c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ff9c-130">Response</span></span>

<span data-ttu-id="3ff9c-131">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-131">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="3ff9c-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3ff9c-132">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="3ff9c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ff9c-133">Request</span></span>
<span data-ttu-id="3ff9c-134">Veja a seguir um exemplo de solicitação de metadados de fotos.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-134">Here is an example of the request for photo metadata.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ff9c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ff9c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
# <a name="c"></a>[<span data-ttu-id="3ff9c-136">C#</span><span class="sxs-lookup"><span data-stu-id="3ff9c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ff9c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ff9c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ff9c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ff9c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3ff9c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ff9c-139">Response</span></span>
<span data-ttu-id="3ff9c-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-140">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="3ff9c-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ff9c-141">Request</span></span>
<span data-ttu-id="3ff9c-142">Veja a seguir um exemplo de solicitação de bytes de fotos.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-142">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="3ff9c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ff9c-143">Response</span></span>
<span data-ttu-id="3ff9c-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ff9c-144">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored","@odata.type": "stream" } -->

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
<!--
{
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
