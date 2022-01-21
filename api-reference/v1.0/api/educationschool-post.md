---
title: Criar educationSchool
description: Crie um novo objeto educationSchool.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d5f192b1a25c223c5742a8ba355d32d10cf4c057
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136243"
---
# <a name="create-educationschool"></a>Criar educationSchool

Namespace: microsoft.graph

Crie um novo [objeto educationSchool.](../resources/educationschool.md)

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
POST /education/schools
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
| :------------ | :-------------------------- |
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto educationSchool.](../resources/educationschool.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [a educationSchool](../resources/educationschool.md).

| Propriedade             | Tipo                                               | Descrição                                                                                                                                                          |
| :------------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| displayName          | Cadeia de caracteres                                             | Nome de exibição da escola. Herdado de [educationOrganization](../resources/educationorganization.md).                                                           |
| description          | Cadeia de caracteres                                             | Descrição da escola. Herdado de [educationOrganization](../resources/educationorganization.md).                                                            |
| externalSource       | educationExternalSource                            | Fonte de onde essa organização foi criada. Herdado de [educationOrganization](../resources/educationorganization.md). Os valores possíveis são: `sis` , 'manual. |
| externalSourceDetail | Cadeia de caracteres                                             | O nome da fonte externa de onde esses recursos foram gerados.                                                                                                   |
| principalEmail       | Cadeia de caracteres                                             | Endereço de email da entidade de segurança.                                                                                                                                      |
| principalName        | Cadeia de caracteres                                             | Nome da entidade de segurança.                                                                                                                                               |
| externalPrincipalId  | Cadeia de caracteres                                             | ID da entidade de segurança no sistema de sincronização.                                                                                                                                   |
| highestGrade         | Cadeia de caracteres                                             | Ensino de nível mais alto.                                                                                                                                                |
| lowestGrade          | Cadeia de caracteres                                             | Ensino de nível mais baixo.                                                                                                                                                 |
| schoolNumber         | Cadeia de caracteres                                             | Número da escola.                                                                                                                                                       |
| externalId           | Cadeia de caracteres                                             | ID da escola no sistema de sincronização.                                                                                                                                      |
| phone                | Cadeia de caracteres                                             | Número de telefone da escola.                                                                                                                                              |
| fax                  | Cadeia de caracteres                                             | Número de fax da escola.                                                                                                                                                |
| createdBy            | [identitySet](../resources/identityset.md)         | Entidade que criou a escola.                                                                                                                                       |
| address              | [physicalAddress](../resources/physicaladdress.md) | Endereço da escola.                                                                                                                                               |

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `201 Created` e um objeto [educationSchool](../resources/educationschool.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationschool_from_"
}
-->

```http
POST https://graph.microsoft.com/v1.0/education/schools
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationschool-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationschool-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationschool-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationschool-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-educationschool-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-educationschool-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```
