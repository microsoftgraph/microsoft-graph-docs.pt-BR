---
title: 'educationUser: delta'
description: Obter usuários recém-criados ou atualizados sem precisar executar uma leitura completa de todo o conjunto de usuários.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eddf1656a9f1366276b89fd5b101768b45e2cca1
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232120"
---
# <a name="educationuser-delta"></a>educationUser: delta

Namespace: microsoft.graph

Get newly created or [updated educationUser](../resources/educationuser.md) without having to perform a full read of the entire collection. Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | EduRoster.ReadBasic                         |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | EduRoster.Read.All, EduRoster.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/users/delta
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código de resposta e uma coleção `200 OK` [educationUser](../resources/educationuser.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/users/delta
```

### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationUser)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationUser)",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/users/delta?$skiptoken=VwhMSQw1l1O5v2F1ZPm...",
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "String (identifier)",
      "primaryRole": "String",
      "middleName": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "residenceAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "mailingAddress": {
        "@odata.type": "microsoft.graph.physicalAddress"
      },
      "student": {
        "@odata.type": "microsoft.graph.educationStudent"
      },
      "teacher": {
        "@odata.type": "microsoft.graph.educationTeacher"
      },
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "accountEnabled": "Boolean",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan"
        }
      ],
      "businessPhones": [
        "String"
      ],
      "department": "String",
      "displayName": "String",
      "givenName": "String",
      "mail": "String",
      "mailNickname": "String",
      "mobilePhone": "String",
      "passwordPolicies": "String",
      "passwordProfile": {
        "@odata.type": "microsoft.graph.passwordProfile"
      },
      "officeLocation": "String",
      "preferredLanguage": "String",
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "refreshTokensValidFromDateTime": "String (timestamp)",
      "showInAddressList": "Boolean",
      "surname": "String",
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      }
    }
  ]
}
```
