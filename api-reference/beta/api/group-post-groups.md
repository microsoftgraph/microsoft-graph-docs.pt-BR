---
title: Criar grupo
description: 'Use esta API para criar um novo grupo, conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: de304cc4faaa6e4b64992ba0d7b2af35e8b5900a
ms.sourcegitcommit: 7d94b581f7c6dc1995efecf6ee21b604c0b80998
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2019
ms.locfileid: "29353066"
---
# <a name="create-group"></a>Criar grupo

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Use esta API para criar um novo [grupo](../resources/group.md) conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:

* Grupo do Office 365 (grupo unificado)
* Grupo dinâmico
* Grupo de segurança

Esta operação retorna, por padrão, apenas um subconjunto das propriedades de cada grupo. Essas propriedades padrão estão listadas na seção [Propriedades](../resources/group.md#properties).

Para obter propriedades _não_ retornadas por padrão, execute uma operação GET e especifique as propriedades em uma opção de consulta `$select` do OData. Veja um [exemplo](group-get.md#request-2).

> **Observação**: para criar uma [equipe](../resources/team.md), primeiro crie um grupo e adicione uma equipe nele, confira [Criar equipe](../api/team-put-teams.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar quando criar um grupo. 

| Propriedade | Tipo | Descrição|
|:---------------|:--------|:----------|
| displayName | string | O nome para exibição no catálogo de endereços do grupo. Obrigatório. |
| mailEnabled | booliano | Defina como **true** para grupos habilitados para email. Defina isto como **true**, se estiver criando um Grupo do Office 365. Defina como **false**, se estiver criando um grupo dinâmico ou de segurança. Obrigatório. |
| mailNickname | string | O alias de email do grupo. Obrigatório. |
| securityEnabled | booliano | Defina como **true** para grupos habilitados para segurança. Defina isto como **true**, se estiver criando um grupo dinâmico ou de segurança. Defina isto como **false**, se estiver criando um Grupo do Office 365. Obrigatório. |
| owners | coleção de cadeias de caracteres | Esta propriedade representa os proprietários do grupo na hora de criação. Opcional. |
| membros | coleção de cadeias de caracteres | Esta propriedade representa os membros do grupo na hora de criação. Opcional. |

Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.

| Tipo de grupo | Propriedade **groupTypes** |
|:--------------|:------------------------|
| Office 365 (também conhecido como grupo unificado)| "Unified" |
| Dinâmica | "DynamicMembership" |
| Segurança | Não defina. |

Como o recurso **group** dá suporte a [extensions](/graph/extensibility-overview), você pode usar a operação `POST` e adicionar propriedades personalizadas com seus próprios dados para o grupo ao criá-lo.

>**Observação:** criar um Grupo do Office 365 programaticamente sem um contexto de usuário e sem especificar os proprietários criará o grupo anonimamente.  Se assim o fizer, o site associado do SharePoint Online só será criado automaticamente, após a execução de outras ações manuais.  

Especifique outras propriedades graváveis conforme necessário para o grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta. A resposta inclui somente as propriedades padrão do grupo.

## <a name="example"></a>Exemplo
#### <a name="request-1"></a>Solicitação 1
A primeira solicitação de exemplo cria um Grupo do Office 365.
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-type: application/json
Content-length: 244

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

#### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade. Todas as propriedades padrão serão retornadas de uma chamada real.
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
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

#### <a name="request-2"></a>Solicitação 2
A segunda solicitação de exemplo cria um Grupo do Office 365 com um proprietário especificado.
<!-- {
  "blockType": "request",
  "name": "create_group_with_owner"
}-->
```http
POST https://graph.microsoft.com/beta/groups
Content-Type: application/json

{
  "description": "Group with designated owner",
  "displayName": "Operations group",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "operations2019",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

 #### <a name="response-2"></a>Resposta 2
Veja a seguir o exemplo de uma resposta bem-sucedida. Ele inclui apenas propriedades padrão. Posteriormente, você pode obter a propriedade de navegação **owners** do grupo para verificar os detalhes do proprietário. 
>**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade. Todas as propriedades padrão serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group_with_owner"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
     "id": "502df398-d59c-469d-944f-34a50e60db3f",
     "deletedDateTime": null,
     "classification": null,
     "createdDateTime": "2018-12-27T22:17:07Z",
     "description": "Group with designated owner",
     "displayName": "Operations group",
     "expirationDateTime": null,
     "groupTypes": [
         "Unified"
     ],
     "mail": "operations2019@contoso.com",
     "mailEnabled": true,
     "mailNickname": "operations2019",
     "membershipRule": null,
     "membershipRuleProcessingState": null,
     "onPremisesLastSyncDateTime": null,
     "onPremisesSecurityIdentifier": null,
     "onPremisesSyncEnabled": null,
     "preferredDataLocation": "CAN",
     "preferredLanguage": null,
     "proxyAddresses": [
         "SMTP:operations2019@contoso.com"
     ],
     "renewedDateTime": "2018-12-27T22:17:07Z",
     "resourceBehaviorOptions": [],
     "resourceProvisioningOptions": [],
     "securityEnabled": false,
     "theme": null,
     "visibility": "Public",
     "onPremisesProvisioningErrors": []
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando extensões do esquema (visualização)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
