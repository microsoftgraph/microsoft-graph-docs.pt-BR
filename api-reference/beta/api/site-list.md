---
title: Enumerar sites
description: Liste [sites] [] em uma organização que corresponda aos critérios de filtro e opções de consulta fornecidos.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f61aab6a7a333e83438f5cc6d03c6ac79e277df2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638638"
---
# <a name="enumerate-sites"></a><span data-ttu-id="688a9-103">Enumerar sites</span><span class="sxs-lookup"><span data-stu-id="688a9-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="688a9-104">Listar os [sites][] disponíveis em uma organização que correspondam aos critérios de filtro e opções de consulta fornecidos.</span><span class="sxs-lookup"><span data-stu-id="688a9-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="688a9-105">Há suporte apenas para as seguintes opções de consulta:</span><span class="sxs-lookup"><span data-stu-id="688a9-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="688a9-106">Instrução Filter</span><span class="sxs-lookup"><span data-stu-id="688a9-106">Filter statement</span></span>             | <span data-ttu-id="688a9-107">Instrução SELECT</span><span class="sxs-lookup"><span data-stu-id="688a9-107">Select statement</span></span>        | <span data-ttu-id="688a9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="688a9-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="688a9-109">Lista todos os conjuntos de sites de nível de raiz na organização.</span><span class="sxs-lookup"><span data-stu-id="688a9-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="688a9-110">Útil para descobrir o site de casa de cada geografia.</span><span class="sxs-lookup"><span data-stu-id="688a9-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="688a9-111">Além disso, você pode usar uma consulta de **[pesquisa][]** em relação à coleção de '/sites ' para localizar sites que correspondem a palavras-chave dadas.</span><span class="sxs-lookup"><span data-stu-id="688a9-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[consulte]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="688a9-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="688a9-114">Permissions</span></span>

<span data-ttu-id="688a9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="688a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="688a9-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="688a9-117">Permission type</span></span>                        | <span data-ttu-id="688a9-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="688a9-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="688a9-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="688a9-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="688a9-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="688a9-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="688a9-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="688a9-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="688a9-122">Not supported.</span></span>
|<span data-ttu-id="688a9-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="688a9-123">Application</span></span>                            | <span data-ttu-id="688a9-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="688a9-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="688a9-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="688a9-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="688a9-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="688a9-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="688a9-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="688a9-127">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="688a9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="688a9-128">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="688a9-129">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="688a9-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="688a9-130">Basic</span><span class="sxs-lookup"><span data-stu-id="688a9-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/list-sites-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="688a9-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="688a9-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/list-sites-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites",
  "suppressions": [
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/site-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
