---
title: Obter foto
description: Recupere as propriedades e os relacionamentos do objeto de foto.
localization_priority: Normal
ms.openlocfilehash: ff46fca695140cabf363f9bccfcc61bc4fb50279
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824461"
---
# <a name="get-photo"></a><span data-ttu-id="c807d-103">Obter foto</span><span class="sxs-lookup"><span data-stu-id="c807d-103">Get photo</span></span>

> <span data-ttu-id="c807d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c807d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c807d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c807d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c807d-106">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="c807d-106">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c807d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c807d-107">Permissions</span></span>
<span data-ttu-id="c807d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c807d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c807d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c807d-110">Permission type</span></span>      | <span data-ttu-id="c807d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c807d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c807d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c807d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c807d-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="c807d-113">Files.Read</span></span>    |
|<span data-ttu-id="c807d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c807d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c807d-115">Files.Read</span><span class="sxs-lookup"><span data-stu-id="c807d-115">Files.Read</span></span>    |
|<span data-ttu-id="c807d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c807d-116">Application</span></span> | <span data-ttu-id="c807d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c807d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c807d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c807d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c807d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c807d-119">Optional query parameters</span></span>
<span data-ttu-id="c807d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c807d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c807d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c807d-121">Request headers</span></span>
| <span data-ttu-id="c807d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c807d-122">Name</span></span>       | <span data-ttu-id="c807d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c807d-123">Type</span></span> | <span data-ttu-id="c807d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c807d-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c807d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c807d-125">Authorization</span></span>  | <span data-ttu-id="c807d-126">string</span><span class="sxs-lookup"><span data-stu-id="c807d-126">string</span></span>  | <span data-ttu-id="c807d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c807d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c807d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c807d-129">Request body</span></span>
<span data-ttu-id="c807d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c807d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c807d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c807d-131">Response</span></span>

<span data-ttu-id="c807d-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c807d-132">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="c807d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c807d-133">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="c807d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c807d-134">Request</span></span>
<span data-ttu-id="c807d-135">Veja a seguir um exemplo de solicitação de metadados de fotos.</span><span class="sxs-lookup"><span data-stu-id="c807d-135">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="c807d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c807d-136">Response</span></span>
<span data-ttu-id="c807d-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c807d-137">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="c807d-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c807d-138">Request</span></span>
<span data-ttu-id="c807d-139">Veja a seguir um exemplo de solicitação de bytes de fotos.</span><span class="sxs-lookup"><span data-stu-id="c807d-139">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="c807d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c807d-140">Response</span></span>
<span data-ttu-id="c807d-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c807d-141">Here is an example of the response.</span></span>

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
