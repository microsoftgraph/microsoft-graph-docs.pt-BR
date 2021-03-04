---
author: swapnil1993
title: 'site: getApplicableContentTypesForList'
description: Obter tipos de conteúdo de site que podem ser adicionados a uma lista.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 2cda6c5e62fc85db8d512d814064fd977fa36b9e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446199"
---
# <a name="site-getapplicablecontenttypesforlist"></a><span data-ttu-id="8d637-103">site: getApplicableContentTypesForList</span><span class="sxs-lookup"><span data-stu-id="8d637-103">site: getApplicableContentTypesForList</span></span>
<span data-ttu-id="8d637-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d637-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d637-105">Obter [][] [contentTypes][contentType] de site que podem ser adicionados a uma lista.</span><span class="sxs-lookup"><span data-stu-id="8d637-105">Get [site][] [contentTypes][contentType] that can be added to a list.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d637-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d637-106">Permissions</span></span>

<span data-ttu-id="8d637-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d637-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d637-109">Permission type</span></span>      | <span data-ttu-id="8d637-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d637-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d637-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d637-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d637-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8d637-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="8d637-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d637-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d637-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="8d637-114">Not Supported</span></span>    |
|<span data-ttu-id="8d637-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d637-115">Application</span></span> | <span data-ttu-id="8d637-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="8d637-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d637-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d637-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/getApplicableContentTypesForList
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d637-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8d637-118">Optional query parameters</span></span>

<span data-ttu-id="8d637-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8d637-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8d637-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8d637-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="8d637-121">Para listar apenas tipos de conteúdo personalizados, use `$filter=isBuiltin eq false` .</span><span class="sxs-lookup"><span data-stu-id="8d637-121">To list only custom content types, use `$filter=isBuiltin eq false`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d637-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d637-122">Request headers</span></span>
|<span data-ttu-id="8d637-123">Nome</span><span class="sxs-lookup"><span data-stu-id="8d637-123">Name</span></span>|<span data-ttu-id="8d637-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d637-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8d637-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d637-125">Authorization</span></span>|<span data-ttu-id="8d637-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d637-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d637-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d637-128">Request body</span></span>
<span data-ttu-id="8d637-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8d637-129">Do not supply a request body for this method.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="8d637-130">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="8d637-130">Function Parameters</span></span>
<span data-ttu-id="8d637-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="8d637-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="8d637-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="8d637-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="8d637-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8d637-133">Parameter</span></span>|<span data-ttu-id="8d637-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d637-134">Type</span></span>|<span data-ttu-id="8d637-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d637-135">Description</span></span>|
|-|-|-|-|
|<span data-ttu-id="8d637-136">listId</span><span class="sxs-lookup"><span data-stu-id="8d637-136">listId</span></span>| <span data-ttu-id="8d637-137">String</span><span class="sxs-lookup"><span data-stu-id="8d637-137">String</span></span> | <span data-ttu-id="8d637-138">GUID da lista para a qual os tipos de conteúdo aplicáveis precisam ser buscados.</span><span class="sxs-lookup"><span data-stu-id="8d637-138">GUID of the list for which the applicable content types need to be fetched.</span></span> <span data-ttu-id="8d637-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d637-139">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="8d637-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d637-140">Response</span></span>

<span data-ttu-id="8d637-141">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [contentType](../resources/contenttype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d637-141">If successful, this function returns a `200 OK` response code and a [contentType](../resources/contenttype.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d637-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d637-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d637-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d637-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "site_getapplicablecontenttypesforlist"
}
-->
```http
GET https://graph.microsoft.com/beta/sites/{siteId}/getApplicableContentTypesForList(listId='listId')
```

### <a name="response"></a><span data-ttu-id="8d637-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d637-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.contentType)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
