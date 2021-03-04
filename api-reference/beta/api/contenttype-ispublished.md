---
author: swapnil1993
title: 'contentType: isPublished'
description: Verifique o status de publicação de um tipo de conteúdo em um site de hub de tipo de conteúdo.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: d6f5700015dcb69ce3440be187654941816e0a9d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445869"
---
# <a name="contenttype-ispublished"></a><span data-ttu-id="dad70-103">contentType: isPublished</span><span class="sxs-lookup"><span data-stu-id="dad70-103">contentType: isPublished</span></span>
<span data-ttu-id="dad70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dad70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="dad70-105">Verifique o status de publicação de um [contentType][] em um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="dad70-105">Check the publishing status of a [contentType][] in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="dad70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dad70-106">Permissions</span></span>

<span data-ttu-id="dad70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dad70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dad70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dad70-109">Permission type</span></span>      | <span data-ttu-id="dad70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dad70-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dad70-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dad70-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dad70-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="dad70-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="dad70-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dad70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dad70-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="dad70-114">Not Supported</span></span>   |
|<span data-ttu-id="dad70-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dad70-115">Application</span></span> | <span data-ttu-id="dad70-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="dad70-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dad70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dad70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
><span data-ttu-id="dad70-118">**Observação:** O siteId representa um site de hub de tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="dad70-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dad70-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dad70-119">Request headers</span></span>
|<span data-ttu-id="dad70-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dad70-120">Name</span></span>|<span data-ttu-id="dad70-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dad70-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dad70-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dad70-122">Authorization</span></span>|<span data-ttu-id="dad70-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dad70-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="dad70-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dad70-125">Response</span></span>
<span data-ttu-id="dad70-126">Se tiver êxito, essa chamada retornará uma resposta e um valor booleano especificando o estado `200 OK` de publicação do tipo de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="dad70-126">If successful, this call returns a `200 OK` response and a boolean value specifying the publishing state of the content type.</span></span>

## <a name="request-body"></a><span data-ttu-id="dad70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dad70-127">Request body</span></span>
<span data-ttu-id="dad70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dad70-128">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="dad70-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dad70-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="dad70-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dad70-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```http
GET https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
### <a name="response"></a><span data-ttu-id="dad70-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dad70-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true 
}
```

[contentType]: ../resources/contentType.md
