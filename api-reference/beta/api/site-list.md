---
title: Enumerar os sites
description: Liste o [de] [sites] disponíveis em uma organização que correspondem a critérios de filtro fornecida e opções de consulta.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f225d9990637f8251ae40e3f66b0f993bbf74f32
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520337"
---
# <a name="enumerate-sites"></a><span data-ttu-id="56fab-103">Enumerar os sites</span><span class="sxs-lookup"><span data-stu-id="56fab-103">Enumerate sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56fab-104">Liste os [sites][] disponíveis em uma organização que coincidem com os critérios de filtro fornecida e opções de consulta.</span><span class="sxs-lookup"><span data-stu-id="56fab-104">List the available [sites][] in an organization that match provided filter criteria and query options.</span></span>

<span data-ttu-id="56fab-105">Somente as seguintes opções de consulta são atualmente suportadas:</span><span class="sxs-lookup"><span data-stu-id="56fab-105">Only the following query options are currently supported:</span></span>

| <span data-ttu-id="56fab-106">Instrução de filtro</span><span class="sxs-lookup"><span data-stu-id="56fab-106">Filter statement</span></span>             | <span data-ttu-id="56fab-107">Instrução SELECT</span><span class="sxs-lookup"><span data-stu-id="56fab-107">Select statement</span></span>        | <span data-ttu-id="56fab-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="56fab-108">Description</span></span>
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | <span data-ttu-id="56fab-109">Lista todos os conjuntos de sites de nível de raiz na organização.</span><span class="sxs-lookup"><span data-stu-id="56fab-109">Lists all root-level site collections in the organization.</span></span> <span data-ttu-id="56fab-110">É útil para descobrir o site inicial para cada região geográfica.</span><span class="sxs-lookup"><span data-stu-id="56fab-110">Useful for discovering the home site for each geography.</span></span>

<span data-ttu-id="56fab-111">Além disso, você pode usar uma consulta de **[pesquisa][]** contra a coleção '/ sites' para encontrar sites correspondência determinados palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="56fab-111">In addition, you may use a **[search][]** query against the '/sites' collection to find sites matching given keywords.</span></span>

[Search]: site-search.md
[search]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="56fab-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="56fab-114">Permissions</span></span>

<span data-ttu-id="56fab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56fab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56fab-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56fab-117">Permission type</span></span>                        | <span data-ttu-id="56fab-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56fab-118">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="56fab-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56fab-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="56fab-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56fab-120">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="56fab-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56fab-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56fab-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56fab-122">Not supported.</span></span>
|<span data-ttu-id="56fab-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56fab-123">Application</span></span>                            | <span data-ttu-id="56fab-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56fab-124">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="56fab-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56fab-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a><span data-ttu-id="56fab-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56fab-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="56fab-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56fab-127">Request</span></span>

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a><span data-ttu-id="56fab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="56fab-128">Response</span></span>

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
    "Error: /api-reference/beta/api/site-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
