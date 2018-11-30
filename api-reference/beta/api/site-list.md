---
title: Enumerar os sites
description: Liste o [de] [sites] disponíveis em uma organização que correspondem a critérios de filtro fornecida e opções de consulta.
ms.openlocfilehash: 4e7d9d12f7b18df84a8b23cc3272084b310edb3a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037825"
---
# <a name="enumerate-sites"></a><span data-ttu-id="5debd-103">Enumerar os sites</span><span class="sxs-lookup"><span data-stu-id="5debd-103">Enumerate sites</span></span>

> <span data-ttu-id="5debd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5debd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5debd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5debd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5debd-106">Liste os [sites][] disponíveis em uma organização que coincidem com os critérios de filtro fornecida e opções de consulta.</span><span class="sxs-lookup"><span data-stu-id="5debd-106">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="5debd-107">Somente as seguintes opções de consulta são atualmente suportadas:</span><span class="sxs-lookup"><span data-stu-id="5debd-107">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="5debd-108">Instrução de filtro</span><span class="sxs-lookup"><span data-stu-id="5debd-108">Filter statement</span></span>             | <span data-ttu-id="5debd-109">Instrução Select</span><span class="sxs-lookup"><span data-stu-id="5debd-109">Select statement</span></span>        | <span data-ttu-id="5debd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5debd-110">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="5debd-111">Lista todos os conjuntos de sites de nível de raiz na organização.</span><span class="sxs-lookup"><span data-stu-id="5debd-111">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="5debd-112">É útil para descobrir o site inicial para cada região geográfica.</span><span class="sxs-lookup"><span data-stu-id="5debd-112">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="5debd-113">Além disso, você pode usar uma consulta de **[pesquisa][]** contra a coleção '/ sites' para encontrar sites correspondência determinados palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="5debd-113">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[pesquisa]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="5debd-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="5debd-116">Permissions</span></span>

<span data-ttu-id="5debd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5debd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5debd-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5debd-119">Permission type</span></span>                        | <span data-ttu-id="5debd-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5debd-120">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="5debd-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5debd-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="5debd-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5debd-122">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="5debd-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5debd-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5debd-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5debd-124">Not supported.</span></span>
|<span data-ttu-id="5debd-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5debd-125">Application</span></span>                            | <span data-ttu-id="5debd-126">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5debd-126">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5debd-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5debd-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="5debd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5debd-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5debd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5debd-129">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="5debd-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="5debd-130">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/List sites"
} -->
