---
title: Trabalhar com sites do SharePoint no Microsoft Graph
description: 'A API do SharePoint no Microsoft Graph oferece suporte aos seguintes cenários principais:'
localization_priority: Priority
ms.prod: sharepoint
doc_type: conceptualPageType
author: JeremyKelley
ms.openlocfilehash: c21b2f23b260051aadc663ad915ec1e1853c37f54bd1b93c0241f67f4dbd681e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54131091"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a>Trabalhar com sites do SharePoint no Microsoft Graph

A API do SharePoint no Microsoft Graph oferece suporte aos seguintes cenários principais:

* Acesso aos **sites**, **lists** e **drives** do SharePoint (bibliotecas de documentos)
* Suporte somente leitura para recursos de **site** (nenhuma capacidade de criar novos sites)
* Suporte a leitura e gravação para **lists**, **listItems** e **driveItems**
* Lidar com recursos por ID do SharePoint, URL ou caminho relativo

A API do SharePoint expõe três tipos de recursos principais:

* [Site](site.md) _(objeto de nível superior)_
* [Lista](list.md)
* [ListItem](listitem.md)

A seguir está um exemplo de um recurso listItem.

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

Recursos expõem dados de três maneiras diferentes:

* _Propriedades_ (como **id** e **name**) expõem valores simples.
* _Facetas_ (como **campos** e **createdBy**) expõem valores complexos.
* _Referências_ (como **itens**) apontam para conjuntos de outros recursos.

Você pode expandir referências na URL com o parâmetro de consulta _expand_; por exemplo, `?expand=fields`.
Você pode solicitar propriedades e facetas específicas com o parâmetro de consulta _select_; por exemplo, `?select=id,name`.
Por padrão, a maioria das propriedades e facetas retorna enquanto todas as referências ficam ocultas.
Por questões de eficiência, recomendamos que você especifique _selecionar_ e _expandir_ para só retornar os dados mais importantes para você.

## <a name="sharepoint-api-root-resources"></a>Recursos de raiz da API do SharePoint

Os exemplos a seguir são relativos a `https://graph.microsoft.com/beta`.

| Caminho                                   | Descrição
|:---------------------------------------|:------------------------------------
| /sites/root                            | [Site][] padrão da organização.
| /sites/{site-id}                       | Acessar um [site][] específico por sua identificação.
| /sites/{site-id}/drive                 | Acessar a [unidade](drive.md) padrão (biblioteca de documentos) desse [site][].
| /sites/{site-id}/drives                | Enumerar as [unidades](drive.md) (bibliotecas de documentos) no [site][].
| /sites/{site-id}/sites                 | Enumerar os subsites no [site][].
| /sites/{site-id}/lists                 | Enumerar as [listas](list.md) sob o [site](site.md).
| /sites/{site-id}/lists/{list-id}/items | Enumerar [listItems](listitem.md) sob a [lista](list.md).
| /groups/{group-id}/sites/root          | Acesse um [site][] de equipe do grupo.

Sites também podem ser tratados pelo caminho usando o nome de host do SharePoint, seguido por dois pontos e o caminho relativo para o site. Opcionalmente, você pode fazer a transição para lidar com o modelo de recurso colocando outros dois pontos no final.

| Caminho                                           | Descrição
|:-----------------------------------------------|:-----------------------------------
| /sites/contoso.sharepoint.com:/teams/hr        | O site associado comhttps://contoso.sharepoint.com/teams/hr
| /sites/contoso.sharepoint.com:/teams/hr:/drive | Acessar a [unidade](drive.md) padrão desse.

## <a name="note-for-existing-sharepoint-developers"></a>Observação para desenvolvedores do SharePoint existentes

A API do Microsoft Graph do SharePoint tem algumas diferenças essenciais das APIs CSOM.
Os recurso do [site][] mapeia para `SPWeb`.
O [site][] (`SPWeb`) raiz em um conjunto de sites tem uma faceta [siteCollection](sitecollection.md), que contém informações sobre `SPSite`.
Como as IDs de sites são exclusivas penas em sua coleção de site, abordar um site por ID requer o fornecimento do identificador de coleção de site e identificador de site.

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id},{spweb-id}/
```
Uma URL construída com apenas o nome do host apontará para o site raiz (`SPWeb`) na coleção de sites padrão.

```http
GET https://graph.microsoft.com/beta/sites/{hostname}
```

Uma URL construída apenas com o nome do host e ID de siteCollection (`SPSite`) apontará o site raiz (`SPWeb`) na coleção de sites determinada.

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id}
```

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

[site]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: sitecollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->


