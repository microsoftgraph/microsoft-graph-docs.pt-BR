---
title: 'directoryObject: checkMemberGroups'
description: 'Verifique se há associação em uma lista especificada de grupos e retorne dessa lista os grupos dos quais o usuário, grupo, entidade de serviço especificado, contato organizacional, dispositivo ou objeto de diretório é um membro.'
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
---

# <a name="directoryobject-checkmembergroups"></a>directoryObject: checkMemberGroups

Namespace: microsoft.graph

Verifique se há associação em uma lista especificada de IDs de grupo e retorne dessa lista esses grupos (identificados por IDs) dos quais o [usuário, grupo](../resources/user.md)[, entidade](../resources/group.md) de serviço [especificado, contato](../resources/serviceprincipal.md) [organizacional, dispositivo](../resources/orgcontact.md) ou objeto de [](../resources/directoryobject.md) diretório é um membro. [](../resources/device.md) Esta função é transitiva.

Você pode fazer check-up de no máximo 20 grupos por solicitação. Essa função dá suporte a todos os grupos provisionados no Azure AD. Como Microsoft 365 grupos não podem conter outros grupos, a associação em um Microsoft 365 grupo é sempre direta.

## <a name="permissions"></a>Permissões

### <a name="group-memberships-for-a-directory-object"></a>Associações de grupo para um objeto directory

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadBasic.All e GroupMember.Read.All, User.Read.All e GroupMember.Read.All, User.ReadBasic.All e Group.Read.All, User.Read.All e Group.Read.All, Directory.Read.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.Read.All e GroupMember.Read.All, User.Read.All e Group.Read.All, Directory.Read.All |

### <a name="group-memberships-for-a-user"></a>Associações de grupo para um usuário

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadBasic.All e GroupMember.Read.All, User.Read.All e GroupMember.Read.All, User.ReadBasic.All e Group.Read.All, User.Read.All e Group.Read.All, Directory.Read.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.Read.All e GroupMember.Read.All, User.Read.All e Group.Read.All, Directory.Read.All |

### <a name="group-memberships-for-a-group"></a>Associações de grupo para um grupo

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All, Directory. AccessAsUser. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                                              |
| Aplicativo                            | GroupMember. Read. All, Group. Read. All, Directory. Read. All, Group. ReadWrite. All, Directory. ReadWrite. All                             |

### <a name="group-memberships-for-a-service-principal"></a>Associações de grupo para uma entidade de serviço

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All |

### <a name="group-memberships-for-an-organizational-contact"></a>Associações de grupo para um contato organizacional

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Directory.Read.All, Directory.ReadWrite.All |

### <a name="group-memberships-for-a-device"></a>Associações de grupo para um dispositivo

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Device.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

<!--

Use the follow scenario guidance to help determine which permission types to use:

| Scenario | Permissions to use |
|:-|:-|
| To get group memberships for the signed-in user | Use one of the following sets of permissions: <br/> <li> **User.Read** and **GroupMember.Read.All** <li>**User.Read** and **Group.Read.All** |
| To get group memberships for any user | Use one of the following sets of permissions: <br/> <li> **User.ReadBasic.All** and **GroupMember.Read.All** <li>**User.Read.All** and **GroupMember.Read.All** <li>**User.ReadBasic.All** and **Group.Read.All** <li>**User.Read.All** and **Group.Read.All** |
| To get group memberships for a group | Use either the **GroupMember.Read.All** or **Group.Read.All** permission. |
| To get group memberships for a directory object | Use the **Directory.Read.All** permission. |

<!-- These tables will replace the data in lines 22-36 to help with the tooling that parses permissions tables.
+ Current data is copy-pasted from incorrect files/file names
+ To validate these permissions against lines 32-36
-->

## <a name="http-request"></a>Solicitação HTTP

Associações de grupo para um objeto de diretório (usuário, grupo, entidade de serviço ou contato organizacional).
<!-- { "blockType": "ignored" } -->
```http
POST /directoryObjects/{id}/checkMemberGroups
```

Associações de grupo para o usuário de entrada ou outros usuários.
<!-- { "blockType": "ignored" } -->
```http
POST /me/checkMemberGroups
POST /users/{id | userPrincipalName}/checkMemberGroups
```

Associações de grupo para um grupo.
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/checkMemberGroups
```

Associações de grupo para uma entidade de serviço.
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/checkMemberGroups
```

Associações de grupo para um contato organizacional.
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups
```

Associações de grupo para um dispositivo.
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/checkMemberGroups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|groupIds|Coleção de cadeias de caracteres|Uma coleção que contém as IDs de objetos dos grupos em que se deve verificar a associação. Até 20 grupos podem ser especificados.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-check-group-memberships-for-a-directory-object"></a>Exemplo 1: Verificar associações de grupo para um objeto de diretório

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e/checkMemberGroups
Content-type: application/json

{
    "groupIds": [
        "f448435d-3ca7-4073-8152-a1fd73c0fd09",
        "bd7c6263-4dd5-4ae8-8c96-556e1c0bece6",
        "93670da6-d731-4366-94b5-abed40b6016b",
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-checkmembergroups-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryobject-checkmembergroups-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "f448435d-3ca7-4073-8152-a1fd73c0fd09",
        "93670da6-d731-4366-94b5-abed40b6016b",
        "f5484ab1-4d4d-41ec-a9b8-754b3957bfc7",
        "c9103f26-f3cf-4004-a611-2a14e81b8f79"
    ]
}
```

### <a name="example-2-check-group-memberships-for-the-signed-in-user"></a>Exemplo 2: Verificar associações de grupo para o usuário associado

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_checkmembergroups_me"
}-->
```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json

{
  "groupIds": [
        "fee2c45b-915a-4a64b130f4eb9e75525e",
        "4fe90ae065a-478b9400e0a0e1cbd540"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-checkmembergroups-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-checkmembergroups-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-checkmembergroups-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-checkmembergroups-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-checkmembergroups-me-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryobject-checkmembergroups-me-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

A seguir, um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
  "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

