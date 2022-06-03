---
title: Listar membros
description: Use essa API para obter a lista de membros (usuários, grupos ou dispositivos) em uma unidade administrativa.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4de66a36c8399a233b5dabdd65041415c2abfe42
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884294"
---
# <a name="list-members"></a>Listar membros

Namespace: microsoft.graph

Use essa API para obter a lista de membros (usuários, grupos ou dispositivos) em uma unidade administrativa.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Application | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All |

> Observação: para listar os membros de uma associação oculta em uma unidade administrativa, a permissão Member.Read.Hidden é necessária.

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>Solicitação HTTP

```http
GET /directory/administrativeUnits/{id}/members
GET /directory/administrativeUnits/{id}/members/$ref
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método (quando usado sem`$ref`) dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, `$search`incluindo , `$count`e .`$filter` A conversão de OData também está habilitada, por exemplo, você pode converter para obter apenas os usuários que são membros da unidade administrativa. 

`$search` tem suporte apenas nas propriedades **displayName** **e description** . Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| ConsistencyLevel  | eventualmente. Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`. Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries). |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `200 OK` de resposta e uma [coleção de objetos](../resources/user.md) de [](../resources/device.md) usuário, [grupo](../resources/group.md) ou dispositivo no corpo da resposta. Adicionar `$ref` ao final da solicitação retorna uma coleção de apenas `@odata.id` URLs dos membros.

## <a name="examples"></a>Exemplos

### <a name="example-1-list-member-objects"></a>Exemplo 1: listar objetos membro

#### <a name="request"></a>Solicitação
A solicitação a seguir listará os membros da unidade administrativa, retornando uma coleção de usuários, grupos e dispositivos.

<!-- {
  "blockType": "request",
  "name": "list_administrativeunit_members"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/c5729e7c-988e-417b-b287-14f5bd4711d8/members
```

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
        {
            "@odata.type": "#microsoft.graph.device",
            "id": "7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac",
            "accountEnabled": true,
            "deviceId": "6fa60d52-01e7-4b18-8055-4759461fc16b",
            "displayName": "Test Windows device",
            "operatingSystem": "Windows"
        },
        {
            "@odata.type": "#microsoft.graph.device",
            "id": "c530e1f6-7b4c-4313-840e-cf1a99ec3b38",
            "accountEnabled": false,
            "deviceId": "4c299165-6e8f-4b45-a5ba-c5d250a707ff",
            "displayName": "Test Linux device",
            "operatingSystem": "linux"
        }
    ]
}
```

### <a name="example-2-list-member-references"></a>Exemplo 2: listar referências de membro

#### <a name="request"></a>Solicitação
A solicitação a seguir listará as referências de membro da unidade administrativa, retornando uma coleção `@odata.id` de referências aos membros.

<!-- {
  "blockType": "request",
  "name": "list_administrativeunit_member_refs"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
```

#### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

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
