---
title: Listar usuários
description: Recupere uma lista de objetos user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7529097f5d22443b95123cc7a2f578f0521b8ca4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563893"
---
# <a name="list-users"></a>Listar usuários

Recuperar uma lista de objetos user.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.

Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_). 

Para retornar um conjunto de propriedades alternativo, você deve especificar o conjunto desejado das propriedades [user](../resources/user.md) usando o parâmetro de consulta OData `$select`. Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`

> Observação: Determinadas propriedades não podem ser retornadas dentro de uma coleção de usuário. As seguintes propriedades só terão suporte na [recuperação de um único usuário](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                      |
|:--------------|:---------------------------|
| Autorização | {token} do portador (obrigatório)  |
| Content-Type  | application/json           |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-standard-users-request"></a>Exemplo 1: Solicitação de usuários padrão

Por padrão, somente um conjunto limitado de propriedades é retornado (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_). Este exemplo ilustra a solicitação padrão e a resposta. 

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-users-request-using-select"></a>Exemplo 2: Solicitação de usuários usando $select

Se precisar de um conjunto de propriedades diferente, você poderá usar o parâmetro de consulta OData `$select`. Por exemplo, para retornar _displayName_, _givenName_ e _postalCode_, você pode adicionar o seguinte à consulta `$select=displayName,givenName,postalCode`

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a>Resposta

Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
