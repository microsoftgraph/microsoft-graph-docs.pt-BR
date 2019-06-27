---
title: Obter foto
description: Recupere as propriedades e os relacionamentos do objeto de foto.
localization_priority: Normal
ms.openlocfilehash: c1746a347d93dad375635eaf68365af64dfadac9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264481"
---
# <a name="get-photo"></a><span data-ttu-id="27be6-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="27be6-103">Get photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27be6-104">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="27be6-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="27be6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="27be6-105">Permissions</span></span>
<span data-ttu-id="27be6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27be6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27be6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27be6-108">Permission type</span></span>      | <span data-ttu-id="27be6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="27be6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="27be6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27be6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="27be6-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="27be6-111">Files.Read</span></span>    |
|<span data-ttu-id="27be6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27be6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27be6-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="27be6-113">Files.Read</span></span>    |
|<span data-ttu-id="27be6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27be6-114">Application</span></span> | <span data-ttu-id="27be6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27be6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27be6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27be6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="27be6-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="27be6-117">Optional query parameters</span></span>
<span data-ttu-id="27be6-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="27be6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="27be6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27be6-119">Request headers</span></span>
| <span data-ttu-id="27be6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="27be6-120">Name</span></span>       | <span data-ttu-id="27be6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="27be6-121">Type</span></span> | <span data-ttu-id="27be6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="27be6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="27be6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27be6-123">Authorization</span></span>  | <span data-ttu-id="27be6-124">string</span><span class="sxs-lookup"><span data-stu-id="27be6-124">string</span></span>  | <span data-ttu-id="27be6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27be6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27be6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27be6-127">Request body</span></span>
<span data-ttu-id="27be6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="27be6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="27be6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="27be6-129">Response</span></span>

<span data-ttu-id="27be6-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27be6-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="27be6-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="27be6-131">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="27be6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27be6-132">Request</span></span>
<span data-ttu-id="27be6-133">Veja a seguir um exemplo de solicitação de metadados de fotos.</span><span class="sxs-lookup"><span data-stu-id="27be6-133">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="27be6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="27be6-134">Response</span></span>
<span data-ttu-id="27be6-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27be6-135">Here is an example of the response.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="27be6-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="27be6-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="27be6-137">C#</span><span class="sxs-lookup"><span data-stu-id="27be6-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="27be6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="27be6-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photo-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="27be6-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="27be6-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_photo-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="27be6-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27be6-140">Request</span></span>
<span data-ttu-id="27be6-141">Veja a seguir um exemplo de solicitação de bytes de fotos.</span><span class="sxs-lookup"><span data-stu-id="27be6-141">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="27be6-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="27be6-142">Response</span></span>
<span data-ttu-id="27be6-143">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27be6-143">Here is an example of the response.</span></span>

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
    "Error: /api-reference/beta/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
