---
title: 'directoryObject: getMemberGroups'
description: 'Retorne todos os grupos dos qual o usuário, grupo, entidade de serviço, contato organizacional, dispositivo ou objeto de diretório especificado é membro. Esta função é transitiva.'
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
---

# <a name="directoryobject-getmembergroups"></a>directoryObject: getMemberGroups

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retorne todas as IDs de grupo dos grupos dos qual o [usuário, grupo](../resources/user.md)[,](../resources/group.md) [entidade de serviço](../resources/serviceprincipal.md) [especificado, contato](../resources/orgcontact.md) [organizacional, dispositivo](../resources/device.md) ou [objeto de diretório é](../resources/directoryobject.md) membro. Esta função é transitiva.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

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
The following table lists the permission types to use for different scenarios.

| Scenario | Permissions |
|:-|:-|
| To get group memberships for the signed-in user | Use one of the following sets of permissions: <br/> <li> **User.Read** and **GroupMember.Read.All** <li>**User.Read** and **Group.Read.All** |
| To get group memberships for any user | Use one of the following sets of permissions: <br/> <li> **User.ReadBasic.All** and **GroupMember.Read.All** <li>**User.Read.All** and **GroupMember.Read.All** <li>**User.ReadBasic.All** and **Group.Read.All** <li>**User.Read.All** and **Group.Read.All** |
| To get group memberships for a group | Use either the **GroupMember.Read.All** or **Group.Read.All** permission. |
| To get group memberships for a service principal | Use one of the following sets of permissions <br/> <li>**Application.ReadWrite.All** and **GroupMember.Read.All** <li>**Application.ReadWrite.All** and **Group.Read.All** |
| To get group memberships for a directory object | Use the **Directory.Read.All** permission. |
-->

## <a name="http-request"></a>Solicitação HTTP

Associações de grupo para um objeto de diretório (usuário, grupo, entidade de serviço ou contato organizacional).
<!-- { "blockType": "ignored" } -->
```http
POST /directoryObjects/{id}/getMemberGroups
```

Associações de grupo para o usuário de entrada ou outros usuários.
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
```

Associações de grupo para um grupo.
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberGroups
```

Associações de grupo para uma entidade de serviço.
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups
```

Associações de grupo para um contato organizacional.
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberGroups
```

Associações de grupo para um dispositivo.
<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/getMemberGroups
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
|securityEnabledOnly|Booliano| `true` para especificar que apenas grupos de segurança dos quais a entidade é membro devem ser retornados; `false` para especificar que todos os grupos e funções de diretório das quais a entidade é membro devem ser retornados. `true` pode ser especificado apenas para usuários ou entidades de serviço retornarem grupos habilitados para segurança. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-check-group-memberships-for-a-directory-object"></a>Exemplo 1: Verificar associações de grupo para um objeto de diretório

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/directoryObjects/0049d944-a805-4680-9f54-3ab292090309/getMemberGroups
Content-type: application/json

{
    "securityEnabledOnly": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-getmembergroups-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryobject-getmembergroups-powershell-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "a8daa1fb-d24c-47d0-9e9e-c99e83394e3e"
    ]
}
```

### <a name="example-2-check-group-memberships-for-the-signed-in-user"></a>Exemplo 2: Verificar associações de grupo para o usuário associado

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups_me"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-me-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-me-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-me-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-me-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/directoryobject-getmembergroups-me-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/directoryobject-getmembergroups-me-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "6239671a-0db6-4e8b-9d2f-f280efb5a181",
        "2e2f1227-1586-45ae-bf51-fccc1de72625",
        "f5987b5a-61f6-4c31-9fa2-7bfb845c8d2a"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


