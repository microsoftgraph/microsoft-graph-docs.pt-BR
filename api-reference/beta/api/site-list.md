---
title: Enumerar sites
description: Liste [sites] [] em uma organização que corresponda aos critérios de filtro e opções de consulta fornecidos.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29b1a3c043712de4eca359b5b58c27308b78ee22
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453646"
---
# <a name="enumerate-sites"></a><span data-ttu-id="076d3-103">Enumerar sites</span><span class="sxs-lookup"><span data-stu-id="076d3-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="076d3-104">Listar os [sites][] disponíveis em uma organização que correspondam aos critérios de filtro e opções de consulta fornecidos.</span><span class="sxs-lookup"><span data-stu-id="076d3-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="076d3-105">Há suporte apenas para as seguintes opções de consulta:</span><span class="sxs-lookup"><span data-stu-id="076d3-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="076d3-106">Instrução Filter</span><span class="sxs-lookup"><span data-stu-id="076d3-106">Filter statement</span></span>             | <span data-ttu-id="076d3-107">Instrução SELECT</span><span class="sxs-lookup"><span data-stu-id="076d3-107">Select statement</span></span>        | <span data-ttu-id="076d3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="076d3-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="076d3-109">Lista todos os conjuntos de sites de nível de raiz na organização.</span><span class="sxs-lookup"><span data-stu-id="076d3-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="076d3-110">Útil para descobrir o site de casa de cada geografia.</span><span class="sxs-lookup"><span data-stu-id="076d3-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="076d3-111">Além disso, você pode usar uma consulta de **[pesquisa][]** em relação à coleção de '/sites ' para localizar sites que correspondem a palavras-chave dadas.</span><span class="sxs-lookup"><span data-stu-id="076d3-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[consulte]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="076d3-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="076d3-114">Permissions</span></span>

<span data-ttu-id="076d3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="076d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="076d3-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="076d3-117">Permission type</span></span>                        | <span data-ttu-id="076d3-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="076d3-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="076d3-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="076d3-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="076d3-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="076d3-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="076d3-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="076d3-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="076d3-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="076d3-122">Not supported.</span></span>
|<span data-ttu-id="076d3-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="076d3-123">Application</span></span>                            | <span data-ttu-id="076d3-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="076d3-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="076d3-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="076d3-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="076d3-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="076d3-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="076d3-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="076d3-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="076d3-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="076d3-128">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="076d3-129">C#</span><span class="sxs-lookup"><span data-stu-id="076d3-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-sites-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="076d3-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="076d3-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-sites-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="076d3-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="076d3-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-sites-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="076d3-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="076d3-132">Response</span></span>

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
