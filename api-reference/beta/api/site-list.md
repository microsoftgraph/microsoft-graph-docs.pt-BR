---
title: Enumerar sites
description: Liste [sites] [] em uma organização que corresponda aos critérios de filtro e opções de consulta fornecidos.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: ''
ms.openlocfilehash: 266f88af6b71317b271bec5ede1d2984d4e704fa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453209"
---
# <a name="enumerate-sites"></a><span data-ttu-id="de3d2-103">Enumerar sites</span><span class="sxs-lookup"><span data-stu-id="de3d2-103">Enumerate sites</span></span>

<span data-ttu-id="de3d2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="de3d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de3d2-105">Listar os [sites][] disponíveis em uma organização que correspondam aos critérios de filtro e opções de consulta fornecidos.</span><span class="sxs-lookup"><span data-stu-id="de3d2-105">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="de3d2-106">Há suporte apenas para as seguintes opções de consulta:</span><span class="sxs-lookup"><span data-stu-id="de3d2-106">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="de3d2-107">Instrução Filter</span><span class="sxs-lookup"><span data-stu-id="de3d2-107">Filter statement</span></span>             | <span data-ttu-id="de3d2-108">Instrução SELECT</span><span class="sxs-lookup"><span data-stu-id="de3d2-108">Select statement</span></span>        | <span data-ttu-id="de3d2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="de3d2-109">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="de3d2-110">Lista todos os conjuntos de sites de nível de raiz na organização.</span><span class="sxs-lookup"><span data-stu-id="de3d2-110">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="de3d2-111">Útil para descobrir o site de casa de cada geografia.</span><span class="sxs-lookup"><span data-stu-id="de3d2-111">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="de3d2-112">Além disso, você pode usar uma consulta **[$Search][]** em relação à coleção '/sites ' para localizar sites que correspondem a palavras-chave dadas.</span><span class="sxs-lookup"><span data-stu-id="de3d2-112">In addition, you may use a **[$search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[$search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="de3d2-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="de3d2-115">Permissions</span></span>

<span data-ttu-id="de3d2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de3d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de3d2-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de3d2-118">Permission type</span></span>                        | <span data-ttu-id="de3d2-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de3d2-119">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="de3d2-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de3d2-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="de3d2-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de3d2-121">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="de3d2-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de3d2-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de3d2-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de3d2-123">Not supported.</span></span>
|<span data-ttu-id="de3d2-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de3d2-124">Application</span></span>                            | <span data-ttu-id="de3d2-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de3d2-125">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="de3d2-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de3d2-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="de3d2-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de3d2-127">Example</span></span>

#### <a name="request"></a><span data-ttu-id="de3d2-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de3d2-128">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="de3d2-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="de3d2-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-sites" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="de3d2-130">C#</span><span class="sxs-lookup"><span data-stu-id="de3d2-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="de3d2-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de3d2-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="de3d2-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de3d2-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="de3d2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="de3d2-133">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
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
