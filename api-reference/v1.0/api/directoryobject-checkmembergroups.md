---
title: 'directoryObject: checkMemberGroups'
description: Verifique se há associação em uma lista especificada de grupos e retorne dessa lista os grupos dos quais o usuário, grupo, entidade de serviço, contato organizacional ou objeto de diretório especificado é um membro.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1efadd27c8e3a9cd2100734fc5b2d781fd451542
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2021
ms.locfileid: "61125055"
---
# <a name="directoryobject-checkmembergroups"></a>directoryObject: checkMemberGroups

Namespace: microsoft.graph

Verifique se há associação em uma lista especificada de grupos e retorne dessa lista os grupos dos quais o usuário [especificado](../resources/user.md) [,](../resources/group.md)grupo, entidade de [serviço,](../resources/serviceprincipal.md)contato [organizacional](../resources/orgcontact.md)ou objeto [de](../resources/directoryobject.md) diretório é um membro. Esta função é transitiva.

Você pode fazer check-up de no máximo 20 grupos por solicitação. Essa função dá suporte a todos os grupos provisionados no Azure AD. Como Microsoft 365 grupos não podem conter outros grupos, a associação em um Microsoft 365 grupo é sempre direta.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadBasic.All, User.Read.All, Directory.Read.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.Read.All, Directory.Read.All |

A tabela a seguir lista os tipos de permissão a usar para cenários diferentes.

| Cenário | Permissões |
|:-|:-|
| Para obter associações de grupo para o usuário de entrada | Use um dos seguintes conjuntos de permissões: <br/> <li> **User.Read** e **GroupMember.Read.All** <li>**User.Read** e **Group.Read.All** |
| Para obter associações de grupo para qualquer usuário | Use um dos seguintes conjuntos de permissões: <br/> <li> **User.ReadBasic.All** e **GroupMember.Read.All** <li>**User.Read.All** e **GroupMember.Read.All** <li>**User.ReadBasic.All** e **Group.Read.All** <li>**User.Read.All** e **Group.Read.All** |
| Para obter associações de grupo para um grupo | Use a **permissão GroupMember.Read.All** **ou Group.Read.All.** |
| Para obter associações de grupo para uma entidade de serviço | Use um dos seguintes conjuntos de permissões <br/> <li>**Application.ReadWrite.All** e **GroupMember.Read.All** <li>**Application.ReadWrite.All** e **Group.Read.All** |
| Para obter associações de grupo para um objeto directory | Use a **permissão Directory.Read.All.** |

<!-- These tables will replace the data in lines 22-36 to help with the tooling that parses permissions tables.
+ Current data is copy-pasted from incorrect files/file names
+ To validate these permissions against lines 32-36

### Group memberships for a directory object

| Permission type                        | Permissions (from least to most privileged)           |
|:---------------------------------------|:------------------------------------------------------|
| Delegated (work or school account)     | User.ReadBasic.All, User.Read.All, Directory.Read.All |
| Delegated (personal Microsoft account) | Not supported.                                        |
| Application                            | User.Read.All, Directory.Read.All                     |

### Group memberships for a user

| Permission type | Permissions (from least to most privileged) |
|:-|:-|
| Delegated (work or school account) | User.ReadBasic.All, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application | User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All |

### Group memberships for a group

| Permission type | Permissions (from least to most privileged) |
|:-|:-|
| Delegated (work or school account) | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegated (personal Microsoft account) | Not supported. |
| Application | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All |

### Group memberships for a service principal

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |

### Group memberships for an organizational contact

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All   |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Directory.Read.All, Directory.ReadWrite.All |

-->

## <a name="http-request"></a>Solicitação HTTP

Associações de grupo para um objeto de diretório (usuário, grupo, entidade de serviço ou contato organizacional).
<!-- { "blockType": "ignored" } -->
```http
POST /directoryObjects/{id}/checkMemberGroups
```

Associações de grupo para o usuário de entrada ou outros usuários.
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
```

Associações de grupo para um grupo.
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberGroups
```

Associações de grupo para uma entidade de serviço.
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups
```

Associações de grupo para um contato organizacional.
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|groupIds|Coleção de cadeias de caracteres|Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-check-group-memberships-for-a-directory-object"></a>Exemplo 1: Verificar associações de grupo para um objeto de diretório

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e/checkMemberGroups
Content-type: application/json

{
    "groupIds": [
        "f448435d-3ca7-4073-8152-a1fd73c0fd09",
        "bd7c6263-4dd5-4ae8-8c96-556e1c0bece6",
        "93670da6-d731-4366-94b5-abed40b6016b",
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    ]
}
```

#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "f448435d-3ca7-4073-8152-a1fd73c0fd09",
        "93670da6-d731-4366-94b5-abed40b6016b",
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    ]
}
```

### <a name="example-2-check-group-memberships-for-the-signed-in-user"></a>Exemplo 2: Verificar associações de grupo para o usuário associado

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups_me"
}-->
```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```

#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

