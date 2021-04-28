---
title: Listar membros
description: Use essa API para obter a lista de membros (usuário e grupo) em uma unidade administrativa.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f65e2f2b8509e5718146a2b99893e35e1bea6327
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054207"
---
# <a name="list-members"></a>Listar membros

Namespace: microsoft.graph

Use essa API para obter a lista de membros (usuário e grupo) em uma unidade administrativa.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All |

> Observação: para listar os membros de uma associação oculta em uma unidade administrativa, a permissão Member.Read.Hidden é necessária.

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>Solicitação HTTP

```http
GET /directory/administrativeUnits/{id}/members
GET /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` de usuário [](../resources/user.md) e/ou grupo no corpo da resposta. [](../resources/group.md)  Em vez disso, se você colocar no final da solicitação, a resposta conterá uma coleção de `$ref` `@odata.id` links/URLs para os membros.

## <a name="examples"></a>Exemplos
##### <a name="list-member-objects"></a>Listar objetos membros
A solicitação a seguir lista os membros da unidade administrativa, retornando uma coleção de usuários e/ou grupos.

```http
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members
```

Veja a seguir um exemplo da resposta. Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.
 
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

##### <a name="list-member-references"></a>Listar referências de membro
A solicitação a seguir lista as referências de membro da unidade administrativa, retornando uma coleção de `@odata.id` referências aos membros.
```
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
```
Veja a seguir um exemplo da resposta. Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
