---
title: Listar membros
description: Use essa API para obter a lista de membros (usuários, grupos e dispositivos) em uma unidade administrativa.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6a3e591e164f92557c1661a3f3c3318508d054e7
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878628"
---
# <a name="list-members"></a>Listar membros

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use essa API para obter a lista de membros (usuários, grupos e dispositivos) em uma unidade administrativa.

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
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método (quando usado sem `$ref`) dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, `$search`incluindo , `$count`e `$filter`. O OData cast também está habilitado, por exemplo, você pode lançar para obter apenas os usuários que são membros da unidade administrativa. 

`$search` tem suporte apenas nas **propriedades displayName** **e description** . Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho      |Valor|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| ConsistencyLevel  | eventualmente. Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries). |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e uma [coleção de objetos](../resources/user.md) de usuário, [grupo](../resources/group.md) [ou dispositivo](../resources/device.md) no corpo da resposta. Adicionar `$ref` ao final da solicitação retorna uma coleção de `@odata.id` URLs somente dos membros.

## <a name="examples"></a>Exemplos
### <a name="example-1-list-member-objects"></a>Exemplo 1: Listar objetos membros

#### <a name="request"></a>Solicitação
A solicitação a seguir lista os membros da unidade administrativa, retornando uma coleção de usuários e/ou grupos.

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta. 
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
 
```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-list-member-references"></a>Exemplo 2: Listar referências de membro

#### <a name="request"></a>Solicitação

A solicitação a seguir lista as referências de membro da unidade administrativa, retornando uma coleção `@odata.id` de referências aos membros.

```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
 
```http
HTTP/1.1 200 OK
Content-type: application/json

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


