---
title: 'user: checkMemberObjects'
description: Verifique se há associação em uma lista de funções de grupo ou diretório para o objeto de usuário especificado.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 4f27a53030e1c01b3efb1967f9f0620033e36f28
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722388"
---
# <a name="user-checkmemberobjects"></a>user: checkMemberObjects

Namespace: microsoft.graph

Verifique se há associação em uma lista de funções de grupo ou diretório para o objeto de usuário especificado. Esse método é transitivo.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | User.ReadBasic.All, User.Read.All, User.ReadWrite.All<br><br>Além disso:<br><br><ul><li>Se verificar a associação em grupos: Group.Read.All, Group.ReadWrite.All</li><li>Se verificar a associação em unidades administrativas: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</li><li>Se verificar se há associação em funções de diretório: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</li></ul>Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All  |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | User.ReadBasic.All, User.Read.All, User.ReadWrite.All<br>E:<ul><li>Se verificar a associação em grupos: Group.Read.All, Group.ReadWrite.All</li><li>Se verificar a associação em unidades administrativas: AdministrativeUnit.Read.All, AdministrativeUnit.ReadWrite.All</li><li>Se verificar se há associação em funções de diretório: RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</li></ul>Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ids|Coleção de cadeias de caracteres|Uma coleção que contém as IDs de objeto dos grupos, funções de diretório ou IDs de roleTemplate de funções de diretório, na qual verificar a associação. Você pode especificar até 20 objetos.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um novo objeto da coleção `200 OK` String no corpo da resposta.

## <a name="examples"></a>Exemplos

Veja a seguir um exemplo de como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-checkmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-checkmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-checkmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-checkmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

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
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

