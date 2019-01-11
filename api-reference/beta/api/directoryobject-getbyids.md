---
title: Obter objetos directory a partir de uma lista de ids
description: Selecione ' opção de consulta não está disponível para esta operação.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 4c63ea85113ec54dec8e5d818c3add1005aebb19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888057"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a>Obter objetos directory a partir de uma lista de ids

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Retorna os objetos directory especificados a partir de uma lista de ids  OBSERVAÇÃO: Os objetos de diretório retornados são os objetos completos que contêm **todas** as propriedades. A opção `$select` não está disponível para todos os tipos de arquivo.

Alguns usos comuns dessa função são:

* Resolver ids retornadas por funções (que retornam coleções de ids) como [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) ou [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta) para seus objetos de diretório de suporte.
* Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro   | Tipo |Descrição|
|:---------------|:--------|:----------|
|ids|Coleção de cadeias de caracteres| Uma coleção de ids para a qual retornar objetos. Você pode especificar até 1000 ids. |
|tipos|Coleção de cadeias de caracteres| Uma coleção dos tipos de recursos que especifica o conjunto de conjuntos de recursos para pesquisar. Se não especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), que contém todos os tipos de recursos definidos no diretório. Qualquer objeto que derive da [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) pode ser especificado na coleção; Por exemplo: [usuário](/graph/api/resources/user?view=graph-rest-beta), [grupo](/graph/api/resources/group?view=graph-rest-beta), [dispositivo](/graph/api/resources/device?view=graph-rest-beta)e assim por diante. Para pesquisar referências a um parceiro de [Provedor de soluções de nuvem](https://partner.microsoft.com/en-us/cloud-solution-provider) organização especificar [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta). Se não especificado, o padrão é [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), que contém todos os tipos de recursos definidos no diretório, exceto para referências a uma organização parceira de [Provedor de soluções de nuvem](https://partner.microsoft.com/en-us/cloud-solution-provider) . Os valores não diferenciam maiusculas de minúsculas.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a>Resposta

Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
