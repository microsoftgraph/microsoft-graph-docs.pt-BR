---
title: Criar educationClass
description: Crie um novo objeto educationClass.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 71dcda18e56b6dfd53fa35943e6da246b5b8d68f
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232148"
---
# <a name="create-educationclass"></a>Criar educationClass

Namespace: microsoft.graph

Crie um novo [objeto educationClass.](../resources/educationclass.md)

> [!NOTE]
> Isso também criará um grupo universal. Quando você usa essa API para criar uma classe, ela adicionará propriedades especiais ao grupo, que adicionará recursos como atribuições e tratamento especial no Microsoft Teams quando as equipes são criadas usando o grupo. Observe que essa API cria apenas o grupo universal e não cria uma equipe. Microsoft Teams fornece uma interface de usuário para que os professores criem equipes para suas próprias classes usando os grupos criados por essa API.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Sem suporte.                              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /education/classes
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto educationClass.](../resources/educationclass.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [educationClass](../resources/educationclass.md).

| Propriedade             | Tipo                                           | Descrição                                                        |
| :------------------- | :--------------------------------------------- | :----------------------------------------------------------------- |
| id                   | String                                         | Identificador de objeto. Herdado da [entidade](../resources/entity.md) |
| displayName          | String                                         | Nome da aula.                                                 |
| mailNickname         | String                                         | Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.    |
| descrição          | String                                         | Descrição da aula.                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | Entidade que criou a aula                                       |
| classCode            | Cadeia de caracteres                                         | Código de aula usada pela escola para identificar a aula.               |
| externalName         | Cadeia de caracteres                                         | Nome da aula no sistema de sincronização.                           |
| externalId           | Cadeia de caracteres                                         | ID da aula no sistema de sincronização.                           |
| externalSource       | educationExternalSource                        | Como essa aula foi criada. Os valores possíveis são: `sis` , `manual`   |
| externalSourceDetail | String                                         | O nome da fonte externa de onde esses recursos foram gerados. |
| grade                | Cadeia de caracteres                                         | Nível de nota da classe.                                          |
| term                 | [educationTerm](../resources/educationterm.md) | Termos dessa aula.                                               |

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-Type: application/json
Content-length: 533

{
  "@odata.type": "#microsoft.graph.educationClass",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```

### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```
