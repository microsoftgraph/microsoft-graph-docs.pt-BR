---
title: Obter foto
description: Recupere as propriedades e os relacionamentos do objeto de foto.
ms.openlocfilehash: 16e0849d3cc1a9a98226b6f34221a8a37cec72b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033130"
---
# <a name="get-photo"></a><span data-ttu-id="843ff-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="843ff-103">Get photo</span></span>

> <span data-ttu-id="843ff-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="843ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="843ff-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="843ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="843ff-106">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="843ff-106">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="843ff-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="843ff-107">Permissions</span></span>
<span data-ttu-id="843ff-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="843ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="843ff-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="843ff-110">Permission type</span></span>      | <span data-ttu-id="843ff-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="843ff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="843ff-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="843ff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="843ff-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="843ff-113">Files.Read</span></span>    |
|<span data-ttu-id="843ff-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="843ff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="843ff-115">Files.Read</span><span class="sxs-lookup"><span data-stu-id="843ff-115">Files.Read</span></span>    |
|<span data-ttu-id="843ff-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="843ff-116">Application</span></span> | <span data-ttu-id="843ff-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="843ff-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="843ff-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="843ff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="843ff-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="843ff-119">Optional query parameters</span></span>
<span data-ttu-id="843ff-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="843ff-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="843ff-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="843ff-121">Request headers</span></span>
| <span data-ttu-id="843ff-122">Nome</span><span class="sxs-lookup"><span data-stu-id="843ff-122">Name</span></span>       | <span data-ttu-id="843ff-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="843ff-123">Type</span></span> | <span data-ttu-id="843ff-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="843ff-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="843ff-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="843ff-125">Authorization</span></span>  | <span data-ttu-id="843ff-126">string</span><span class="sxs-lookup"><span data-stu-id="843ff-126">string</span></span>  | <span data-ttu-id="843ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="843ff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="843ff-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="843ff-129">Request body</span></span>
<span data-ttu-id="843ff-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="843ff-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="843ff-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="843ff-131">Response</span></span>

<span data-ttu-id="843ff-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="843ff-132">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="843ff-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="843ff-133">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="843ff-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="843ff-134">Request</span></span>
<span data-ttu-id="843ff-135">Veja a seguir um exemplo de solicitação de metadados de fotos.</span><span class="sxs-lookup"><span data-stu-id="843ff-135">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="843ff-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="843ff-136">Response</span></span>
<span data-ttu-id="843ff-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="843ff-137">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="843ff-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="843ff-138">Request</span></span>
<span data-ttu-id="843ff-139">Veja a seguir um exemplo de solicitação de bytes de fotos.</span><span class="sxs-lookup"><span data-stu-id="843ff-139">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="843ff-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="843ff-140">Response</span></span>
<span data-ttu-id="843ff-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="843ff-141">Here is an example of the response.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
