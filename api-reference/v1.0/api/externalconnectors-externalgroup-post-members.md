---
title: Criar identidade
description: Crie um novo membro como um recurso de identidade em um externalGroup.
author: sacampbe
localization_priority: Normal
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 42ac3ef6dd3aa12d1116c09694c74957c34077e3
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697484"
---
# <a name="create-identity"></a>Criar identidade
Namespace: microsoft.graph.externalConnectors



Criar um [recurso](../resources/externalconnectors-identity.md) de identidade para um novo membro em [um externalGroup](../resources/externalconnectors-externalgroup.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Sem suporte                               |
| Delegado (conta pessoal da Microsoft) | Sem suporte                               |
| Aplicativo                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All                  |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /connections/{connectionsId}/groups/{externalGroupId}/members
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
|:--------------|:----------------------------|
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do **objeto identity.**

Você pode especificar as seguintes propriedades ao criar um recurso **de** identidade para um membro em **um externalGroup**.

| Propriedade       | Tipo                    | Descrição                                              |
|:---------------|:------------------------|:---------------------------------------------------------|
| id             | Cadeia de caracteres                  | O exclusivo `id` do membro. Seria **objectId no** caso de Azure Active Directory ou grupos e **externalGroupId** no caso de grupos externos. Obrigatório.                                    |
| type           | microsoft.graph.externalConnectors.identityType | O tipo de membro adicionado ao grupo externo. Os valores possíveis são: `user` , `group` , `externalGroup` . Obrigatório. |


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto **identity** no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-an-azure-active-directory-user-as-a-member"></a>Exemplo 1: Adicionar um usuário Azure Active Directory como membro

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_aad_user_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user"
}
```

<!-- markdownlint-disable MD024 -->
#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e811976d-83df-4cbd-8b9b-5215b18aa874",
  "type": "user"
}
```

### <a name="example-2-add-an-azure-active-directory-group-as-a-member"></a>Exemplo 2: Adicionar um grupo Azure Active Directory como membro

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_aad_group_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group"
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e5477431-1038-484e-bf69-1dfedb97a110",
  "type": "group"
}
```

### <a name="example-3-add-another-external-group-as-a-member"></a>Exemplo 3: Adicionar outro grupo externo como membro

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_external_group_identity_from_group"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups/31bea3d537902000/members
Content-Type: application/json

{
  "id": "1431b9c38ee647f6a",
  "type": "externalGroup",
}
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.identity"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "14m1b9c38qe647f6a",
  "type": "externalGroup"
}
```
