---
title: Criar educationClass
description: Crie um novo objeto educationClass.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bc70af54d18593ec7cef8cd90eae52a90f39b99b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115075"
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
| id                   | Cadeia de caracteres                                         | Identificador de objeto. Herdado da [entidade](../resources/entity.md) |
| displayName          | Cadeia de caracteres                                         | Nome da aula.                                                 |
| mailNickname         | String                                         | Nome de email para enviar email a todos os membros, se essa propriedade estiver habilitada.    |
| description          | Cadeia de caracteres                                         | Descrição da aula.                                          |
| createdBy            | [identitySet](../resources/identityset.md)     | Entidade que criou a aula                                       |
| classCode            | Cadeia de caracteres                                         | Código de aula usada pela escola para identificar a aula.               |
| externalName         | Cadeia de caracteres                                         | Nome da aula no sistema de sincronização.                           |
| externalId           | Cadeia de caracteres                                         | ID da aula no sistema de sincronização.                           |
| externalSource       | educationExternalSource                        | Como essa aula foi criada. Os valores possíveis são: `sis` , `manual`   |
| externalSourceDetail | Cadeia de caracteres                                         | O nome da fonte externa de onde esses recursos foram gerados. |
| grade                | Cadeia de caracteres                                         | Nível de nota da classe.                                          |
| term                 | [educationTerm](../resources/educationterm.md) | Termos dessa aula.                                               |

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationClass](../resources/educationclass.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-Type: application/json

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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-educationclass-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-educationclass-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
