---
title: Criar externalGroupMember
description: Criar um novo objeto externalGroupMember.
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: b6c1d278fed4d32ac61afb7989c27d16e3fb275c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954619"
---
# <a name="create-externalgroupmember"></a>Criar externalGroupMember

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um novo objeto [externalGroupMember](../resources/externalgroupmember.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (de privilégios máximos a mínimos) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte                               |
| Delegado (conta pessoal da Microsoft) | Sem suporte                               |
| Aplicativo                            | ExternalItem.ReadWrite.All                  |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /external/connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
|:--------------|:----------------------------|
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [externalGroupMember](../resources/externalgroupmember.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [externalGroupMember](../resources/externalgroupmember.md).

| Propriedade       | Tipo                    | Descrição                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| id             | String                  | O exclusivo `id` do membro. Seria o objectId em caso de usuários ou grupos do Azure Active Directory e o externalGroupId no caso de grupos externos.                                    |
| tipo           | externalGroupMemberType | O tipo de membro adicionado ao grupo externo. Os valores possíveis são: `user` ou `group` quando IdentityName é `azureActiveDirectory` e apenas `group` quando IdentityName é `external` . |
| identificação da identidade | identitySourceType      | A origem de identidade à qual o membro pertence. Os valores possíveis são: `azureActiveDirectory` e `external`.                                                                                         |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [externalGroupMember](../resources/externalgroupmember.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a>Exemplo 1: adicionar um usuário do Azure Active Directory como membro

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroupmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroupmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroupmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroupmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a>Exemplo 2: adicionar um grupo do Azure Active Directory como membro

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group",
  "identitySource": "azureActiveDirectory"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a>Exemplo 3: adicionar outro grupo externo como membro

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_externalgroupmember_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "1431b9c38ee647f6a",
  "type": "group",
  "identitySource": "external"
}
```

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalGroupMember"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "14m1b9c38qe647f6a",
  "type": "group",
  "identitySource": "external"
}
```
