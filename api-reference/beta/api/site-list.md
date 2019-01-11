---
title: Enumerar os sites
description: Liste o [de] [sites] disponíveis em uma organização que correspondem a critérios de filtro fornecida e opções de consulta.
localization_priority: Normal
ms.openlocfilehash: 87ce5b68ccadffa6e0422c413ab79ee784f361c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855814"
---
# <a name="enumerate-sites"></a>Enumerar os sites

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Liste os [sites][] disponíveis em uma organização que coincidem com os critérios de filtro fornecida e opções de consulta.

Somente as seguintes opções de consulta são atualmente suportadas:

| Instrução de filtro             | Instrução Select        | Descrição
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | Lista todos os conjuntos de sites de nível de raiz na organização. É útil para descobrir o site inicial para cada região geográfica.

Além disso, você pode usar uma consulta de **[pesquisa][]** contra a coleção '/ sites' para encontrar sites correspondência determinados palavras-chave.

[pesquisa]: site-search.md
[sites]: ../resources/site.md

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)
|:--------------------------------------|:-------------------------------------
|Delegado (conta corporativa ou de estudante)     | Sites.Read.All, Sites.ReadWrite.All
|Delegado (conta pessoal da Microsoft) | Sem suporte.
|Aplicativo                            | Sites.Read.All, Sites.ReadWrite.All

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/beta/sites?filter=siteCollection/root ne null
```

## <a name="example"></a>Exemplo

#### <a name="request"></a>Solicitação

<!-- { "blockType": "request", "name": "list-sites" } -->

```http
GET https://graph.microsoft.com/beta/sites?select=siteCollection,webUrl&filter=siteCollection/root%20ne%20null
```

#### <a name="response"></a>Resposta

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
