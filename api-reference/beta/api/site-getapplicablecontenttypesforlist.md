---
author: swapnil1993
title: 'site: getApplicableContentTypesForList'
description: Obter tipos de conteúdo de site que podem ser adicionados a uma lista.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 99ca8f23b153f8835fc841e142b79684601bd293
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772447"
---
# <a name="site-getapplicablecontenttypesforlist"></a><span data-ttu-id="f1ba0-103">site: getApplicableContentTypesForList</span><span class="sxs-lookup"><span data-stu-id="f1ba0-103">site: getApplicableContentTypesForList</span></span>
<span data-ttu-id="f1ba0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1ba0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1ba0-105">Obter [][] [contentTypes][contentType] de site que podem ser adicionados a uma lista.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-105">Get [site][] [contentTypes][contentType] that can be added to a list.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1ba0-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1ba0-106">Permissions</span></span>

<span data-ttu-id="f1ba0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1ba0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ba0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1ba0-109">Permission type</span></span>      | <span data-ttu-id="f1ba0-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1ba0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1ba0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1ba0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f1ba0-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f1ba0-112">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="f1ba0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1ba0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1ba0-114">Não suportado</span><span class="sxs-lookup"><span data-stu-id="f1ba0-114">Not Supported</span></span>    |
|<span data-ttu-id="f1ba0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1ba0-115">Application</span></span> | <span data-ttu-id="f1ba0-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f1ba0-116">Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1ba0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1ba0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/getApplicableContentTypesForList
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1ba0-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1ba0-118">Optional query parameters</span></span>

<span data-ttu-id="f1ba0-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f1ba0-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f1ba0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="f1ba0-121">Para listar apenas tipos de conteúdo personalizados, use `$filter=isBuiltin eq false` .</span><span class="sxs-lookup"><span data-stu-id="f1ba0-121">To list only custom content types, use `$filter=isBuiltin eq false`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1ba0-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ba0-122">Request headers</span></span>
|<span data-ttu-id="f1ba0-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f1ba0-123">Name</span></span>|<span data-ttu-id="f1ba0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1ba0-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f1ba0-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1ba0-125">Authorization</span></span>|<span data-ttu-id="f1ba0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1ba0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ba0-128">Request body</span></span>
<span data-ttu-id="f1ba0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-129">Do not supply a request body for this method.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="f1ba0-130">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="f1ba0-130">Function Parameters</span></span>
<span data-ttu-id="f1ba0-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="f1ba0-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="f1ba0-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f1ba0-133">Parameter</span></span>|<span data-ttu-id="f1ba0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1ba0-134">Type</span></span>|<span data-ttu-id="f1ba0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1ba0-135">Description</span></span>|
|-|-|-|-|
|<span data-ttu-id="f1ba0-136">listId</span><span class="sxs-lookup"><span data-stu-id="f1ba0-136">listId</span></span>| <span data-ttu-id="f1ba0-137">String</span><span class="sxs-lookup"><span data-stu-id="f1ba0-137">String</span></span> | <span data-ttu-id="f1ba0-138">GUID da lista para a qual os tipos de conteúdo aplicáveis precisam ser buscados.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-138">GUID of the list for which the applicable content types need to be fetched.</span></span> <span data-ttu-id="f1ba0-139">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-139">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="f1ba0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1ba0-140">Response</span></span>

<span data-ttu-id="f1ba0-141">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [contentType](../resources/contenttype.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1ba0-141">If successful, this function returns a `200 OK` response code and a [contentType](../resources/contenttype.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1ba0-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1ba0-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1ba0-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ba0-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f1ba0-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1ba0-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "site_getapplicablecontenttypesforlist"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{siteId}/getApplicableContentTypesForList(listId='listId')
```
# <a name="c"></a>[<span data-ttu-id="f1ba0-145">C#</span><span class="sxs-lookup"><span data-stu-id="f1ba0-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-getapplicablecontenttypesforlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1ba0-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1ba0-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-getapplicablecontenttypesforlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1ba0-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1ba0-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-getapplicablecontenttypesforlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f1ba0-148">Java</span><span class="sxs-lookup"><span data-stu-id="f1ba0-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/site-getapplicablecontenttypesforlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f1ba0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1ba0-149">Response</span></span>

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
