---
title: Obter recurso
description: Recupere os dados binários do objeto resource de um arquivo ou imagem.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 9937040d9e53213946df9eb31cf9136bcfda7c71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946060"
---
# <a name="get-resource"></a><span data-ttu-id="06dc5-103">Obter recurso</span><span class="sxs-lookup"><span data-stu-id="06dc5-103">Get resource</span></span>

<span data-ttu-id="06dc5-104">Recupere os dados binários do objeto [resource](../resources/resource.md) de um arquivo ou imagem.</span><span class="sxs-lookup"><span data-stu-id="06dc5-104">Retrieve the binary data of a file or image [resource](../resources/resource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="06dc5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="06dc5-105">Permissions</span></span>
<span data-ttu-id="06dc5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06dc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06dc5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="06dc5-108">Permission type</span></span>      | <span data-ttu-id="06dc5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="06dc5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06dc5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="06dc5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06dc5-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06dc5-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="06dc5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="06dc5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06dc5-113">Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06dc5-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="06dc5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="06dc5-114">Application</span></span> | <span data-ttu-id="06dc5-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06dc5-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="06dc5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="06dc5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="06dc5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="06dc5-117">Request headers</span></span>
| <span data-ttu-id="06dc5-118">Nome</span><span class="sxs-lookup"><span data-stu-id="06dc5-118">Name</span></span>       | <span data-ttu-id="06dc5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="06dc5-119">Type</span></span> | <span data-ttu-id="06dc5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="06dc5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="06dc5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="06dc5-121">Authorization</span></span>  | <span data-ttu-id="06dc5-122">string</span><span class="sxs-lookup"><span data-stu-id="06dc5-122">string</span></span>  | <span data-ttu-id="06dc5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="06dc5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06dc5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="06dc5-125">Request body</span></span>
<span data-ttu-id="06dc5-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="06dc5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06dc5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="06dc5-127">Response</span></span>

<span data-ttu-id="06dc5-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e os dados binários do arquivo ou imagem no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06dc5-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="06dc5-129">Observação: As imagens não serão renderizadas diretamente em um navegador porque elas exigem autorização para recuperá-las, como o restante do conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="06dc5-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="06dc5-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06dc5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06dc5-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="06dc5-131">Request</span></span>
<span data-ttu-id="06dc5-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="06dc5-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="06dc5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="06dc5-133">Response</span></span>
<span data-ttu-id="06dc5-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="06dc5-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
