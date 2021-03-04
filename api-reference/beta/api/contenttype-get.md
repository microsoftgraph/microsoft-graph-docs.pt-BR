---
author: swapnil1993
title: Obter contentType
description: Obter um tipo de conteúdo em um site ou em uma lista.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 70b8ab5db2af4dd391df468dab31adbd26adc13e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445871"
---
# <a name="get-contenttype"></a><span data-ttu-id="f8401-103">Obter contentType</span><span class="sxs-lookup"><span data-stu-id="f8401-103">Get contentType</span></span>
<span data-ttu-id="f8401-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8401-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8401-105">Recupere os metadados de [um tipo de conteúdo][contentType] em um [site][] ou em uma [lista][].</span><span class="sxs-lookup"><span data-stu-id="f8401-105">Retrieve the metadata for a [content type][contentType] in a [site][] or a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="f8401-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f8401-106">Permissions</span></span>

<span data-ttu-id="f8401-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8401-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8401-109">Permission type</span></span>      | <span data-ttu-id="f8401-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f8401-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8401-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8401-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8401-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f8401-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="f8401-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8401-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8401-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8401-114">Not supported.</span></span>    |
|<span data-ttu-id="f8401-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8401-115">Application</span></span> | <span data-ttu-id="f8401-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f8401-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8401-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8401-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}

GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8401-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f8401-118">Optional query parameters</span></span>
<span data-ttu-id="f8401-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f8401-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f8401-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f8401-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8401-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8401-121">Request headers</span></span>
|<span data-ttu-id="f8401-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f8401-122">Name</span></span>|<span data-ttu-id="f8401-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8401-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8401-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8401-124">Authorization</span></span>|<span data-ttu-id="f8401-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8401-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8401-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8401-127">Request body</span></span>
<span data-ttu-id="f8401-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f8401-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8401-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8401-129">Response</span></span>

<span data-ttu-id="f8401-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [contentType](../resources/contenttype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8401-130">If successful, this method returns a `200 OK` response code and a [contentType](../resources/contenttype.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="f8401-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8401-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8401-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8401-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contenttype"
}
-->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```

### <a name="response"></a><span data-ttu-id="f8401-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8401-133">Response</span></span>
><span data-ttu-id="f8401-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f8401-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"0x0120D520",
  "description":"Create a document set when you want to manage multiple documents as a single work product.",
  "group":"Document Set Content Types",
  "hidden":false,
  "name":"Document Set",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
[list]: ../resources/list.md
