---
title: Listar sites
description: Liste todos os sites disponíveis em uma organização ou liste os sites que correspondem aos critérios de filtro fornecidos e às opções de consulta.
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: f78db6d9ad4d4b2f772ed79451ff16853a514d4e
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66578098"
---
# <a name="list-sites"></a>Listar sites

Namespace: microsoft.graph

Listar todos os [sites disponíveis][] em uma organização.

Também há suporte para critérios de filtro e opções de consulta específicos e descritos abaixo:

| Instrução Filter             | Instrução Select        | Descrição
|:-----------------------------|:------------------------|:--------------------
|`siteCollection/root ne null` | `siteCollection,webUrl` | Lista todos os conjuntos de sites de nível raiz na organização. Útil para descobrir o site inicial para cada geografia.

Além disso, você pode usar uma **[$search][]** consulta `/sites` em relação à coleção para localizar sites correspondentes a determinadas palavras-chave.

[$search]: site-search.md
[sites]: ../resources/site.md

Para obter mais diretrizes sobre como criar aplicativos que usam a descoberta de sites para fins de verificação, consulte as práticas recomendadas para descobrir arquivos e [detectar alterações em escala](/onedrive/developer/rest-api/concepts/scan-guidance?view=odsp-graph-online).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="list-all-site-collections"></a>Listar todos os conjuntos de sites

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte.                              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Sites.Read.All, Sites.ReadWrite.All         |

### <a name="discover-the-home-site-for-each-geography"></a>Descobrir o site inicial de cada geografia

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sites.Read.All, Sites.ReadWrite.All         |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Sites.Read.All, Sites.ReadWrite.All         |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /sites
GET /sites?$filter=siteCollection/root ne null
```

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/sites?$select=siteCollection,webUrl&$filter=siteCollection/root%20ne%20null
```

### <a name="response"></a>Resposta

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

### <a name="request"></a>Solicitação

<!-- { "blockType": "ignored" } -->

```http
GET https://graph.microsoft.com/v1.0/sites
```

### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,bf6fb551-d508-4946-a439-b2a6154fc1d9,65a04b8b-1f44-442b-a1fc-9e5852fb946c",
      "name": "Root Site",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com",
        "dataLocationCode": "NAM",
        "root": { }
      },
      "webUrl": "https://contoso.sharepoint.com"
    },
    {
      "id": "contoso.sharepoint.com,d9ecf079-9b13-4376-ac5d-f242dda55626,746dbcc1-fa2b-4120-b657-2670bae5bb6f",
      "name": "Site A",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com"
      },
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,fd1a778f-263e-4c43-acdf-d5c2519d80eb,c06016db-dfec-4f79-83a1-09c6dbfd7022",
      "name": "Site B",
      "root": { },
      "siteCollection": {
        "hostname": "contoso.sharepoint.com"
      },
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
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


