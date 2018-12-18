---
title: Listar membros
description: Use essa API para obter os membros da lista (de usuário e de grupo) em uma unidade administrativa.
author: lleonard-msft
ms.openlocfilehash: d373c8353928d8e8d5d8b398aa09e62d457ba665
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311659"
---
# <a name="list-members"></a>Listar membros

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Use essa API para obter os membros da lista (de usuário e de grupo) em uma unidade administrativa.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All, Directory.ReadWrite.All |

> Observação: Para listar os membros de uma associação oculta em uma unidade administrativa, a permissão de Member.Read.Hidden é obrigatório.

## <a name="http-request"></a>Solicitação HTTP

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [usuário](../resources/user.md) e/ou [grupo](../resources/group.md) no corpo da resposta.  Em vez disso, se você colocar `$ref` ao final da solicitação, a resposta conterá uma coleção de `@odata.id` links/URLs aos membros.

## <a name="examples"></a>Exemplos
##### <a name="list-member-objects"></a>Objetos de membros da lista
A seguinte solicitação listará os membros da unidade administrativa, retornando uma coleção de usuários e/ou em grupos.

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a>Referências de membro de lista
A seguinte solicitação listará as referências de membro da unidade administrativa, retornando uma coleção de `@odata.id` referências aos membros.
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
