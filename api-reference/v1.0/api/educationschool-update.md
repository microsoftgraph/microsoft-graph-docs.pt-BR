---
title: Atualizar educationSchool
description: Atualize as propriedades de um objeto educationSchool.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 70502ab3ad21d6d71d9560c95e2cdef1fc5c5f98
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117652"
---
# <a name="update-educationschool"></a>Atualizar educationSchool

Namespace: microsoft.graph

Atualize as propriedades de um [objeto educationSchool.](../resources/educationschool.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | Sem suporte.                              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor                     |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json          |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto educationSchool.](../resources/educationschool.md)

A tabela a seguir mostra as propriedades que são necessárias ao atualizar [o educationSchool](../resources/educationschool.md).

| Propriedade             | Tipo                                               | Descrição                                                                                                                                                           |
| :------------------- | :------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| displayName          | Cadeia de caracteres                                             | Nome de exibição da escola. Herdado de [educationOrganization](../resources/educationorganization.md).                                                            |
| description          | Cadeia de caracteres                                             | Descrição da escola. Herdado de [educationOrganization](../resources/educationorganization.md).                                                             |
| externalSource       | educationExternalSource                            | Fonte de onde essa organização foi criada. Herdado de [educationOrganization](../resources/educationorganization.md). Os valores possíveis são: `sis` e `manual`. |
| externalSourceDetail | Cadeia de caracteres                                             | O nome da fonte externa de onde esses recursos foram gerados.                                                                                                    |
| principalEmail       | Cadeia de caracteres                                             | Endereço de email da entidade de segurança.                                                                                                                                       |
| principalName        | Cadeia de caracteres                                             | Nome da entidade de segurança.                                                                                                                                                |
| externalPrincipalId  | Cadeia de caracteres                                             | ID da entidade de segurança no sistema de sincronização.                                                                                                                                    |
| highestGrade         | Cadeia de caracteres                                             | Ensino de nível mais alto.                                                                                                                                                 |
| lowestGrade          | Cadeia de caracteres                                             | Ensino de nível mais baixo.                                                                                                                                                  |
| schoolNumber         | Cadeia de caracteres                                             | Número da escola.                                                                                                                                                        |
| externalId           | Cadeia de caracteres                                             | ID da escola no sistema de sincronização.                                                                                                                                       |
| phone                | Cadeia de caracteres                                             | Número de telefone da escola.                                                                                                                                               |
| fax                  | Cadeia de caracteres                                             | Número de fax da escola.                                                                                                                                                 |
| createdBy            | [identitySet](../resources/identityset.md)         | Entidade que criou a escola.                                                                                                                                        |
| address              | [physicalAddress](../resources/physicaladdress.md) | Endereço da escola.                                                                                                                                                |

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [educationSchool](../resources/educationschool.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-educationschool-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-educationschool-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
