---
title: 'directoryObject: getMemberGroups'
description: Retorna todos os grupos dos quais o usuário, grupo ou objeto de diretório especificado é membro. Esta função é transitiva.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9ccb8db35f8aadf89859afc130377287f4bcce1b
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123555"
---
# <a name="directoryobject-getmembergroups"></a>directoryObject: getMemberGroups

Namespace: microsoft.graph

Retorne todos os grupos dos qual o usuário [especificado,](../resources/user.md) [grupo,](../resources/group.md)entidade de [serviço,](../resources/serviceprincipal.md)contato [organizacional](../resources/orgcontact.md)ou objeto [de diretório](../resources/directoryobject.md) é membro. Esta função é transitiva.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadBasic.All e GroupMember.Read.All, User.Read.All e GroupMember.Read.All, User.ReadBasic.All e Group.Read.All, User.Read.All e Group.Read.All, Directory.Read.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.Read.All e GroupMember.Read.All, User.Read.All e Group.Read.All, Directory.Read.All |

Use as diretrizes de cenário a seguir para ajudar a determinar quais tipos de permissão usar:

| Cenário | Permissões a usar |
|:-|:-|
| Para obter associações de grupo para o usuário de entrada | Use um dos seguintes conjuntos de permissões: <br/> <li> **User.Read** e **GroupMember.Read.All** <li>**User.Read** e **Group.Read.All** |
| Para obter associações de grupo para qualquer usuário | Use um dos seguintes conjuntos de permissões: <br/> <li> **User.ReadBasic.All** e **GroupMember.Read.All** <li>**User.Read.All** e **GroupMember.Read.All** <li>**User.ReadBasic.All** e **Group.Read.All** <li>**User.Read.All** e **Group.Read.All** |
| Para obter associações de grupo para um grupo | Use a **permissão GroupMember.Read.All** **ou Group.Read.All.** |
| Para obter associações de grupo para um objeto directory | Use a **permissão Directory.Read.All.** |

<!-- These tables will replace the data in lines 22-36 to help with the tooling that parses permissions tables.
+ Current data is copy-pasted from incorrect files/file names
+ To validate these permissions against lines 32-36

### Group memberships for a directory object

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All |

### Group memberships for a user

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | User.ReadBasic.All and GroupMember.Read.All, User.Read.All and GroupMember.Read.All, User.ReadBasic.All and Group.Read.All, User.Read.All and Group.Read.All, Directory.Read.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | User.Read.All and GroupMember.Read.All, User.Read.All and Group.Read.All, Directory.Read.All |

### Group memberships for a group

| Permission type                        | Permissions (from least to most privileged)                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| Delegated (work or school account)     | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegated (personal Microsoft account) | Not supported.                                                                              |
| Application                            | GroupMember.Read.All, Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All                             |

### Group memberships for a service principal

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |

### Group memberships for an organizational contact

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegated (personal Microsoft account) | Not supported.    |
|Application | Directory.Read.All, Directory.ReadWrite.All |

-->

## <a name="http-request"></a>Solicitação HTTP

Associações de grupo para um objeto de diretório (usuário, grupo, entidade de serviço ou contato organizacional).
<!-- { "blockType": "ignored" } -->
```http
POST /directoryObjects/{id}/getMemberGroups
```

Associações de grupo para o usuário de entrada ou outros usuários.
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
```

Associações de grupo para um grupo.
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberGroups
```

Associações de grupo para uma entidade de serviço.
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups
```

Associações de grupo para um contato organizacional.
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-Type   | application/json  |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|securityEnabledOnly|Booliano| `true` para especificar que apenas grupos de segurança dos quais a entidade é membro devem ser retornados; para especificar que todos os grupos e funções de diretório das quais `false` a entidade é membro devem ser retornados. `true` pode ser especificado apenas para usuários ou entidades de serviço retornarem grupos habilitados para segurança. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-check-group-memberships-for-a-directory-object"></a>Exemplo 1: Verificar associações de grupo para um objeto de diretório

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/0049d944-a805-4680-9f54-3ab292090309/getMemberGroups
Content-type: application/json

{
    "securityEnabledOnly": false
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
        "a8daa1fb-d24c-47d0-9e9e-c99e83394e3e"
    ]
}
```

### <a name="example-2-check-group-memberships-for-the-signed-in-user"></a>Exemplo 2: Verificar associações de grupo para o usuário associado

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups_me"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

#### <a name="response"></a>Resposta

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
        "6239671a-0db6-4e8b-9d2f-f280efb5a181",
        "2e2f1227-1586-45ae-bf51-fccc1de72625",
        "1dae9306-be75-4c3c-99ec-0316a4342c84",
        "0e2d1bbb-76f8-4140-bda7-2a858b74507e",
        "0049d944-a805-4680-9f54-3ab292090309",
        "a8daa1fb-d24c-47d0-9e9e-c99e83394e3e",
        "6f204729-1b8f-4067-bcc9-98fb6c069ffd",
        "59afd38d-441a-4358-b074-8b9b1e7de52f",
        "64ed3df3-53c7-4d4d-ac5c-5c8dd4dafe33",
        "8b676bab-4b1e-419e-a253-7f5aca97d739",
        "be4ef325-9fa8-40d7-b375-4758853ddf52",
        "f5987b5a-61f6-4c31-9fa2-7bfb845c8d2a"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

