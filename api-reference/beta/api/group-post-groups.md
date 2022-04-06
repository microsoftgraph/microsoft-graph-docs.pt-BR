---
title: Criar grupo
description: Criar um novo grupo ou grupo de segurança do Microsoft 365.
author: psaffaie
ms.localizationpriority: high
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 346c19c28e9e30b196c87b9fdca48d50e9e7bd01
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587137"
---
# <a name="create-group"></a>Criar grupo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [group](../resources/group.md) as specified in the request body. You can create one of the following groups:

- Grupo do Microsoft 365 (grupo unificado)
- Grupo de segurança

Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo. Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties). Para obter propriedades _não_ retornadas por padrão, execute uma [operação GET](group-get.md) e especifique as propriedades em uma opção de consulta `$select` do OData.

**Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                |
| :------------------------------------- | :--------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Group.ReadWrite.All, Directory.ReadWrite.All               |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                             |
| Aplicativo                            | Group.Create, Group.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /groups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição               |
| :------------ | :------------------------ |
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto de [grupo](../resources/group.md).

A tabela a seguir mostra as propriedades necessárias ao criar o [grupo](../resources/group.md). Especifique outras propriedades graváveis conforme necessário para o seu grupo.

| Propriedade        | Tipo    | Descrição                                                                                                                                                                                                                                                                                                                                |
| :-------------- | :------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| displayName     | string  | O nome a ser exibido no catálogo de endereços do grupo. O comprimento máximo é de 256 caracteres. Requeridos.                                                                                                                                                                                                                                         |
| mailEnabled     | booliano | Definir como `true` para grupos habilitados para e-mail. Obrigatório.                                                                                                                                                                                                                                                                                           |
| mailNickname    | string  | O alias de email do grupo, exclusivo para grupos do Microsoft 365 na organização. O comprimento máximo é de 64 caracteres. Essa propriedade pode conter apenas caracteres no [conjunto de caracteres ASCII de 0 a 127](/office/vba/language/reference/user-interface-help/character-set-0127), exceto o seguinte: ` @ () \ [] " ; : . <> , SPACE`. Obrigatório. |
| securityEnabled | booliano | Definido como `true` para grupos habilitados para segurança, incluindo Microsoft 365 grupos. Obrigatório. **Observação:** os grupos criados usando o portal do Microsoft Azure sempre terão **securityEnabled** definido inicialmente como `true`.                                                                                                                                    |

> [!IMPORTANT]
>
> - Criar um grupo usando a permissão de aplicativo **Group.Create** sem especificar proprietários criará o grupo anonimamente e o grupo não será modificável. Adicione proprietários ao grupo ao criá-lo para especificar os proprietários que podem modificar o grupo.
>
> - Ao criar um grupo do Microsoft 365 programaticamente com um contexto somente de aplicativo e sem especificar os proprietários, o grupo será criado anonimamente. Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.
>
> - As propriedades a seguir não podem ser definidas na solicitação POST inicial e devem ser definidas em uma solicitação PATCH subsequente: **allowExternalSenders**, **autoSubscribeNewMembers**, **hideFromAddressLists**, **hideFromOutlookClients**, **isSubscribedByMail**, **unseenCount**.

Como o recurso de **grupo** dá suporte a [extensões](/graph/extensibility-overview), você pode adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.

### <a name="grouptypes-options"></a>Opções de groupTypes

Use a propriedade **groupTypes** para controlar o tipo de grupo e sua associação, conforme mostrad.

| Tipo de grupo                     | Associação atribuída | Associação dinâmica                |
| :-------------------------------- | :------------------ | :-------------------------------- |
| Microsoft 365 (também conhecido como grupo unificado) | `["Unified"]`       | `["Unified","DynamicMembership"]` |
| Dinâmica                           | `[]` (_null_)       | `["DynamicMembership"]`           |

## <a name="response"></a>Resposta

Se bem-sucedido, esse método retorna um código de resposta `201 Created` e um objeto [group](../resources/group.md) no corpo da resposta. A resposta inclui somente as propriedades padrão do grupo.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-microsoft-365-group"></a>Exemplo 1: Criar um grupo do Microsoft 365

O exemplo a seguir cria um grupo do Microsoft 365. Como os proprietários não foram especificados, o usuário que fez a chamada é adicionado automaticamente como proprietário do grupo.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_group"
}-->

```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json

{
  "description": "Self help community for golf",
  "displayName": "Golf Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "golfassist",
  "securityEnabled": false
}
```

# <a name="c"></a>[C#](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/create-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/create-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/create-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/create-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)

[!INCLUDE [sample-code](../includes/snippets/go/create-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)

[!INCLUDE [sample-code](../includes/snippets/powershell/create-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta. O valor da propriedade **preferredDataLocation** foi herdado da localização de dados preferencial do criador do grupo.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
     "id": "45b7d2e7-b882-4a80-ba97-10b7a63b8fa4",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-22T02:21:05Z",
     "description": "Self help community for golf",
     "displayName": "Golf Assist",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
   "isAssignableToRole": null,
     "mail": "golfassist@contoso.com",
     "mailEnabled": true,
     "mailNickname": "golfassist",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:golfassist@contoso.onmicrosoft.com"
     ],
     "renewedDateTime": "2018-12-22T02:21:05Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
   "securityIdentifier": "S-1-12-1-1753967289-1089268234-832641959-555555555",
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

### <a name="example-2-create-a-security-group-with-an-owner-and-members"></a>Exemplo 2: criar um grupo de segurança com um proprietário e membros

O exemplo a seguir cria um grupo de segurança com um proprietário e membros especificados. Observe que, no máximo, 20 relações, como proprietários e membros, podem ser adicionadas como parte da criação do grupo. Posteriormente, você pode adicionar mais membros, usando a API [adicionar membro](/graph/api/group-post-members?view=graph-rest-beta&preserve-view=true) ou o envio em lotes JSON.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "create_prepopulated_group"
}-->

```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner and members",
  "displayName": "Operations group",
  "groupTypes": [
  ],
  "mailEnabled": false,
  "mailNickname": "operations2019",
  "securityEnabled": true,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  "members@odata.bind": [
    "https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
}
```

#### <a name="response"></a>Resposta

Veja a seguir o exemplo de uma resposta bem-sucedida. Ele inclui apenas propriedades padrão. Posteriormente, você pode acessar as propriedades de navegação de grupo **proprietários** ou **membros** para verificar o proprietário ou membros. O valor da propriedade **preferredDataLocation** foi herdado da localização de dados preferencial do criador do grupo.

> **Observação:** O objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_prepopulated_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/1226170d-83d5-49b8-99ab-d1ab3d91333e/Microsoft.DirectoryServices.Group",
    "id": "1226170d-83d5-49b8-99ab-d1ab3d91333e",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2021-09-21T07:14:44Z",
    "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
    "organizationId": "84841066-274d-4ec0-a5c1-276be684bdd3",
    "description": "Group with designated owner and members",
    "displayName": "Operations group",
    "expirationDateTime": null,
    "groupTypes": [],
    "infoCatalogs": [],
    "isAssignableToRole": null,
    "isManagementRestricted": null,
    "mail": null,
    "mailEnabled": false,
    "mailNickname": "operations2019",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
    "onPremisesDomainName": null,
    "onPremisesLastSyncDateTime": null,
    "onPremisesNetBiosName": null,
    "onPremisesSamAccountName": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": null,
    "preferredLanguage": null,
    "proxyAddresses": [],
    "renewedDateTime": "2021-09-21T07:14:44Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-304486157-1236829141-2882644889-1043566909",
    "theme": null,
    "visibility": null,
    "writebackConfiguration": {
        "isEnabled": null,
        "onPremisesGroupType": null
    },
    "onPremisesProvisioningErrors": []
}
```

### <a name="example-3-create-a-microsoft-365-group-that-can-be-assigned-to-an-azure-ad-role"></a>Exemplo 3: Criar um grupo do Microsoft 365 que pode ser atribuído a uma função do Azure AD

#### <a name="request"></a>Solicitação

Este é um exemplo da solicitação. O usuário ou aplicativo de chamada precisam receber a permissão _RoleManagement.ReadWrite.Directory_ para definir a propriedade **isAssignableToRole** ou atualizar sua afiliação a esses grupos.

**OBSERVAÇÃO:** Um grupo com a propriedade **isAssignableToRole** definida como `true` não pode ser do tipo associação dinâmica. Para mais informações, consulte [Usando um grupo para gerenciar as atribuições de funções do Azure AD](https://go.microsoft.com/fwlink/?linkid=2103037).

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_role_enabled_group"
}-->

```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
    "description": "Group assignable to a role",
    "displayName": "Role assignable group",
    "groupTypes": [
        "Unified"
    ],
    "isAssignableToRole": true,
    "mailEnabled": true,
    "securityEnabled": true,
    "mailNickname": "contosohelpdeskadministrators",
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/99e44b05-c10b-4e95-a523-e2732bbaba1e"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0",
        "https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e"
    ]
}
```

# <a name="c"></a>[C#](#tab/csharp)

[!INCLUDE [sample-code](../includes/snippets/csharp/create-role-enabled-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)

[!INCLUDE [sample-code](../includes/snippets/javascript/create-role-enabled-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)

[!INCLUDE [sample-code](../includes/snippets/objc/create-role-enabled-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)

[!INCLUDE [sample-code](../includes/snippets/java/create-role-enabled-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)

[!INCLUDE [sample-code](../includes/snippets/go/create-role-enabled-group-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)

[!INCLUDE [sample-code](../includes/snippets/powershell/create-role-enabled-group-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

Este é um exemplo de resposta. O valor da propriedade **preferredDataLocation** foi herdado da localização de dados preferencial do criador do grupo.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_role_enabled_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/84841066-274d-4ec0-a5c1-276be684bdd3/directoryObjects/1afc3ca3-b14d-43af-9c70-8ae3a5065454/Microsoft.DirectoryServices.Group",
    "id": "1afc3ca3-b14d-43af-9c70-8ae3a5065454",
    "deletedDateTime": null,
    "classification": null,
    "createdDateTime": "2021-09-21T07:16:21Z",
    "createdByAppId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
    "organizationId": "84841066-274d-4ec0-a5c1-276be684bdd3",
    "description": "Group assignable to a role",
    "displayName": "Role assignable group",
    "expirationDateTime": null,
    "groupTypes": [
        "Unified"
    ],
    "infoCatalogs": [],
    "isAssignableToRole": true,
    "isManagementRestricted": null,
    "mail": "contosohelpdeskadministrators@Contoso.com",
    "mailEnabled": true,
    "mailNickname": "contosohelpdeskadministrators",
    "membershipRule": null,
    "membershipRuleProcessingState": null,
    "onPremisesDomainName": null,
    "onPremisesLastSyncDateTime": null,
    "onPremisesNetBiosName": null,
    "onPremisesSamAccountName": null,
    "onPremisesSecurityIdentifier": null,
    "onPremisesSyncEnabled": null,
    "preferredDataLocation": "EU",
    "preferredLanguage": null,
    "proxyAddresses": [
        "SMTP:contosohelpdeskadministrators@Contoso.com"
    ],
    "renewedDateTime": "2021-09-21T07:16:21Z",
    "resourceBehaviorOptions": [],
    "resourceProvisioningOptions": [],
    "securityEnabled": true,
    "securityIdentifier": "S-1-12-1-452738211-1135587661-3817500828-1414792869",
    "theme": null,
    "visibility": "Private",
    "writebackConfiguration": {
        "isEnabled": null,
        "onPremisesGroupType": null
    },
    "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando extensões do esquema (visualização)](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
