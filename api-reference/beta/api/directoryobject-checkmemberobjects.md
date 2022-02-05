---
title: 'directoryObject: checkMemberObjects'
description: 'Verifique se há associação em uma lista de grupos, unidades administrativas ou funções de diretório para o usuário, grupo, entidade de serviço, contato organizacional, dispositivo ou objeto de diretório especificado.'
ms.localizationpriority: medium
author: jpettere
ms.prod: users
doc_type: apiPageType
---

# <a name="directoryobject-checkmemberobjects"></a>directoryObject: checkMemberObjects

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Verifique se há associação em uma lista de IDs de grupo, IDs de unidade administrativa ou IDs de função de diretório, para as IDs do [usuário, grupo](../resources/user.md)[,](../resources/group.md) [entidade de serviço](../resources/serviceprincipal.md), contato [](../resources/device.md)[organizacional, dispositivo](../resources/orgcontact.md) ou objeto [de diretório especificado](../resources/directoryobject.md). Esse método é transitivo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="memberships-for-a-directory-object"></a>Associações para um objeto directory

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All |

### <a name="memberships-for-a-user"></a>Associações para um usuário

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read, User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.ReadWrite.All |

### <a name="memberships-for-a-group"></a>Associações para um grupo

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                                              |
| Aplicativo                            | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All                             |

### <a name="memberships-for-a-service-principal"></a>Associações para uma entidade de serviço

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |

### <a name="memberships-for-an-organizational-contact"></a>Associações para um contato organizacional

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All, Directory.ReadWrite.All |

### <a name="memberships-for-a-device"></a>Associações para um dispositivo

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Device.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |


## <a name="http-request"></a>Solicitação HTTP


Associações para um objeto de diretório.
<!-- { "blockType": "ignored" } -->
```http
POST /directoryObjects/{id}/checkMemberObjects
```

Associações para um usuário.
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberObjects
POST /users/{id | userPrincipalName}/checkMemberObjects
```

Associações para um grupo.
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberObjects
```

Associações para uma entidade de serviço.
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberObjects
```

Associações para um contato organizacional.
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberObjects
```

Associações para um dispositivo.
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/checkMemberObjects
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {token} |
| Content-Type  | application/json |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ids|Coleção de cadeias de caracteres|Uma coleção que contém as IDs de objeto dos grupos, funções de diretório, unidades administrativas ou IDs de roleTemplate de funções de diretório, na qual verificar a associação. Até 20 objetos podem ser especificados.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto da coleção String no corpo da resposta.

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
POST https://graph.microsoft.com/beta/me/checkMemberObjects
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

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/user-checkmemberobjects-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/user-checkmemberobjects-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

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
  "description": "directoryObject: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


