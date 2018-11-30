---
title: Obter foto
description: Recupere as propriedades e os relacionamentos do objeto de foto.
ms.openlocfilehash: c7a18f5c765bcbd9f2bc6f9eb4844f11fc282058
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006274"
---
# <a name="get-photo"></a><span data-ttu-id="7d103-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="7d103-103">Get photo</span></span>

<span data-ttu-id="7d103-104">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="7d103-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d103-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d103-105">Permissions</span></span>
<span data-ttu-id="7d103-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d103-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d103-108">Permission type</span></span>      | <span data-ttu-id="7d103-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d103-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d103-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d103-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d103-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="7d103-111">Files.Read</span></span>    |
|<span data-ttu-id="7d103-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d103-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d103-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="7d103-113">Files.Read</span></span>    |
|<span data-ttu-id="7d103-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d103-114">Application</span></span> | <span data-ttu-id="7d103-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d103-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d103-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d103-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7d103-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7d103-117">Optional query parameters</span></span>
<span data-ttu-id="7d103-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7d103-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d103-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d103-119">Request headers</span></span>
| <span data-ttu-id="7d103-120">Nome</span><span class="sxs-lookup"><span data-stu-id="7d103-120">Name</span></span>       | <span data-ttu-id="7d103-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d103-121">Type</span></span> | <span data-ttu-id="7d103-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d103-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7d103-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d103-123">Authorization</span></span>  | <span data-ttu-id="7d103-124">string</span><span class="sxs-lookup"><span data-stu-id="7d103-124">string</span></span>  | <span data-ttu-id="7d103-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d103-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d103-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d103-127">Request body</span></span>
<span data-ttu-id="7d103-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d103-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d103-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d103-129">Response</span></span>

<span data-ttu-id="7d103-130">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d103-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7d103-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7d103-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7d103-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d103-132">Request</span></span>
<span data-ttu-id="7d103-133">Veja a seguir um exemplo de solicitação de metadados de fotos.</span><span class="sxs-lookup"><span data-stu-id="7d103-133">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="7d103-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d103-134">Response</span></span>
<span data-ttu-id="7d103-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d103-135">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="7d103-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d103-136">Request</span></span>
<span data-ttu-id="7d103-137">Veja a seguir um exemplo de solicitação de bytes de fotos.</span><span class="sxs-lookup"><span data-stu-id="7d103-137">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="7d103-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d103-138">Response</span></span>
<span data-ttu-id="7d103-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d103-139">Here is an example of the response.</span></span>

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
  "tocPath": ""
}-->
