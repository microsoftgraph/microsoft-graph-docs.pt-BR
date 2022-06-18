---
title: Adicionar um membro
description: Use essa API para adicionar um membro (usuário, grupo ou dispositivo) a uma unidade administrativa.
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 76ce28e022d171ccd50486527e2ac0c0cfe5df58
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160549"
---
# <a name="add-a-member"></a>Adicionar um membro

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use essa API para adicionar um membro (usuário, grupo ou dispositivo) a uma unidade administrativa ou para criar um novo grupo dentro de uma unidade administrativa. Todos [os tipos de](/graph/api/resources/groups-overview) grupo podem ser criados em uma unidade administrativa.

**Nota:** Atualmente, só é possível adicionar um membro por vez a uma unidade administrativa."

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="permissions-to-add-an-existing-user-group-or-device"></a>Permissões para adicionar um usuário, grupo ou dispositivo existente
|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | AdministrativeUnit.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | AdministrativeUnit.ReadWrite.All |

Para adicionar um usuário, grupo ou dispositivo a uma unidade administrativa, a entidade de chamada deve receber uma das seguintes Azure AD [funções](/azure/active-directory/roles/permissions-reference):

* Administrador de Função Com Privilégios
* Administrador Global

### <a name="permissions-to-create-a-new-group"></a>Permissões para criar um novo grupo
|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Application | Directory.ReadWrite.All |

Para criar um novo grupo em uma unidade administrativa, a entidade de chamada deve receber uma das seguintes Azure AD [funções](/azure/active-directory/roles/permissions-reference):

* Administrador de Função Com Privilégios
* Administrador Global
* Administrador de Grupos

## <a name="http-request"></a>Solicitação HTTP

A solicitação a seguir adiciona um usuário, grupo ou dispositivo existente à unidade administrativa.
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```

A solicitação a seguir cria um novo grupo dentro da unidade administrativa.
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-type  | application/json. Obrigatório. |

### <a name="adding-an-existing-user-or-group"></a>Adicionando um usuário ou grupo existente
No corpo da solicitação, forneça o `id` de um [usuário](../resources/user.md),  [grupo](../resources/group.md), [dispositivo](../resources/device.md) ou [directoryObject](../resources/directoryobject.md) a ser adicionado.

### <a name="creating-a-new-group"></a>Criando um novo grupo
A tabela a seguir mostra as propriedades do recurso [de](../resources/group.md) grupo a serem especificadas quando você cria um grupo na unidade administrativa. 

| Propriedade | Tipo | Descrição|
|:---------------|:--------|:----------|
| displayName | string | O nome para exibição no catálogo de endereços do grupo. Necessário. |
| description | string | Uma descrição para o grupo. Opcional. |
| isAssignableToRole | Booliano | Definir para **true** para habilitar o grupo a ser atribuído uma função do Azure AD. Somente o Administrador com Função Privilegiada e o Administrador Global podem definir o valor dessa propriedade. Opcional. |
| mailEnabled | booliano | Defina como **true** para grupos habilitados para email. Obrigatório. |
| mailNickname | string | O alias de email do grupo. Esses caracteres não podem ser usados no mailNickName: `@()\[]";:.<>,SPACE`. Obrigatório. |
| securityEnabled | booliano | Defina como **true** para grupos habilitados para segurança, incluindo grupos do Microsoft 365. Obrigatório. |
| owners | Coleção [directoryObject](../resources/directoryobject.md) | Esta propriedade representa os proprietários do grupo na hora de criação. Opcional. |
| membros | Coleção [directoryObject](../resources/directoryobject.md) | Esta propriedade representa os membros do grupo na hora de criação. Opcional. |
|visibility|Cadeia de caracteres|Especifica a visibilidade de um grupo do Microsoft 365. Os valores possíveis são: `Private`, `Public`, `HiddenMembership` ou vazio (que é interpretado como `Public`).|

## <a name="response"></a>Resposta

Se tiver êxito, adicionar um objeto existente (usando `$ref`) retornará o `204 No Content` código de resposta. Não retorna nada no corpo da resposta. 

Ao criar um novo grupo (sem `$ref`), esse método retorna `201 Created` um código de resposta e um objeto [de](../resources/group.md) grupo no corpo da resposta. A resposta inclui somente as propriedades padrão do grupo.

## <a name="examples"></a>Exemplos
### <a name="example-1-add-an-existing-user-or-group"></a>Exemplo 1: Adicionar um usuário ou grupo existente
O seguinte adicionará um usuário ou grupo existente à unidade administrativa.

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeunits_members_ref"
} -->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-ref-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-ref-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-ref-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-ref-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-administrativeunits-members-ref-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/post-administrativeunits-members-ref-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



No corpo da solicitação, forneça o `id` [usuário, grupo](../resources/user.md)[](../resources/group.md) [ou objeto de](../resources/device.md) dispositivo que você deseja adicionar.

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
 
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "post_administrativeunits_members_ref"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-create-a-new-group"></a>Exemplo 2: Criar um novo grupo
O exemplo a seguir cria um novo grupo na unidade administrativa.

#### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_administrativeunits_members"
} -->
``` http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#Microsoft.Graph.Group",
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
[!INCLUDE [sample-code](../includes/snippets/csharp/post-administrativeunits-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-administrativeunits-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-administrativeunits-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-administrativeunits-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/post-administrativeunits-members-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



No corpo da solicitação, forneça as propriedades do objeto [de](../resources/group.md) grupo que você deseja adicionar.

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "post_administrativeunits_members"
} -->
``` http
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
