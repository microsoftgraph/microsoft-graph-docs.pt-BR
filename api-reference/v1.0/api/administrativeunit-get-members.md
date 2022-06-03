---
title: Obter um membro
description: Use essa API para obter um membro específico (usuário, grupo ou dispositivo) em uma unidade administrativa.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5919b75724f10d16dbdca5669e511d9a24b67503
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884222"
---
# <a name="get-a-member"></a>Obter um membro

Namespace: microsoft.graph

Use essa API para obter um membro específico (usuário, grupo ou dispositivo) em uma unidade administrativa.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All    |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Application | AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

```http
GET /directory/administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta [e um usuário](../resources/user.md), [grupo](../resources/group.md) ou objeto [de](../resources/device.md) dispositivo no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "get_administrativeunit_members"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/c5729e7c-988e-417b-b287-14f5bd4711d8/members/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.device",
    "id": "7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac",
    "accountEnabled": true,
    "createdDateTime": "2022-04-20T08:53:50Z",
    "deviceId": "6fa60d52-01e7-4b18-8055-4759461fc16b",
    "displayName": "Test device",
    "operatingSystem": "Windows"
}
```
