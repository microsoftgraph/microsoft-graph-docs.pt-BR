---
title: Enumerar sites
description: Listar os [sites] disponíveis em uma organização que corresponderam aos critérios de filtro e às opções de consulta fornecidas.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: c1b8af50227346e4440e4ca98873b20160ecd81b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475776"
---
# <a name="enumerate-sites"></a><span data-ttu-id="ab9d5-103">Enumerar sites</span><span class="sxs-lookup"><span data-stu-id="ab9d5-103">Enumerate sites</span></span>

<span data-ttu-id="ab9d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab9d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab9d5-105">Listar os [sites][] disponíveis em uma organização que corresponderem aos critérios de filtro e às opções de consulta fornecidas.</span><span class="sxs-lookup"><span data-stu-id="ab9d5-105">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="ab9d5-106">No momento, há suporte apenas para as seguintes opções de consulta:</span><span class="sxs-lookup"><span data-stu-id="ab9d5-106">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="ab9d5-107">Instrução Filter</span><span class="sxs-lookup"><span data-stu-id="ab9d5-107">Filter statement</span></span>             | <span data-ttu-id="ab9d5-108">Instrução Select</span><span class="sxs-lookup"><span data-stu-id="ab9d5-108">Select statement</span></span>        | <span data-ttu-id="ab9d5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab9d5-109">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="ab9d5-110">Lista todos os conjunto de sites de nível raiz na organização.</span><span class="sxs-lookup"><span data-stu-id="ab9d5-110">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="ab9d5-111">Útil para descobrir o site de cada geografia.</span><span class="sxs-lookup"><span data-stu-id="ab9d5-111">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="ab9d5-112">Além disso, você pode usar uma $search **[em][]** relação ao conjunto '/sites' para encontrar sites correspondentes a determinadas palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="ab9d5-112">In addition, you may use a **[$search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[$search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="ab9d5-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab9d5-115">Permissions</span></span>

<span data-ttu-id="ab9d5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab9d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab9d5-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab9d5-118">Permission type</span></span>                        | <span data-ttu-id="ab9d5-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab9d5-119">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="ab9d5-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab9d5-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="ab9d5-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab9d5-121">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="ab9d5-122">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab9d5-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab9d5-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab9d5-123">Not supported.</span></span>
|<span data-ttu-id="ab9d5-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab9d5-124">Application</span></span>                            | <span data-ttu-id="ab9d5-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab9d5-125">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="ab9d5-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab9d5-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="ab9d5-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab9d5-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ab9d5-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab9d5-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ab9d5-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab9d5-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-sites" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="ab9d5-130">C#</span><span class="sxs-lookup"><span data-stu-id="ab9d5-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab9d5-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab9d5-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab9d5-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab9d5-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab9d5-133">Java</span><span class="sxs-lookup"><span data-stu-id="ab9d5-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-sites-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ab9d5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab9d5-134">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Contoso USA",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso-jpn.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Contoso Japan",
      "root": { },
      "siteCollection": {
        "hostname": "contoso-jp.sharepoint.com",
        "dataLocationCode": "JPN",
        "root": { }
      },
      "webUrl": "https://contoso-jp.sharepoint.com"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
  ]
}
-->


