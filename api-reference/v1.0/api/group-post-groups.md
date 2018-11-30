---
title: Criar grupo
description: 'Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:'
ms.openlocfilehash: 63cb04ad1b7bd8bfbe0798b53f28b5b16e0b795f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004599"
---
# <a name="create-group"></a>Criar grupo
Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:

* Grupo do Office 365 (grupo unificado)
* Grupo dinâmico
* Grupo de segurança

> **Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.

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
A tabela a seguir mostra as propriedades do [grupo de](../resources/group.md) recurso para especificar quando você cria um grupo. 

| Propriedade | Tipo | Descrição|
|:---------------|:--------|:----------|
| displayName | string | O nome de exibição no catálogo de endereços do grupo. Obrigatório. |
| mailEnabled | booliano | Defina como **true** para grupos habilitados para email. Defina como **true** se criando um grupo do Office 365. Defina como **false** se criando dinâmico ou grupo de segurança. Obrigatório. |
| mailNickname | string | O alias de email do grupo. Obrigatório. |
| securityEnabled | booliano | Defina como **true** para grupos de segurança. Defina isso como **true** se a criação de um grupo de segurança ou dinâmico. Defina como **false** se criando um grupo do Office 365. Obrigatório. |
| owners | coleção de cadeias de caracteres | Essa propriedade representa os proprietários do grupo no momento da criação. Opcional. |
| membros | coleção de cadeias de caracteres | Essa propriedade representa os membros do grupo no momento da criação. Opcional. |


Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.

### <a name="grouptypes-options"></a>Opções de groupTypes

| Tipo de grupo | Propriedade **groupTypes** |
|:--------------|:------------------------|
| Office 365 (também conhecido como grupo unificado)| "Unified" |
| Dinâmica | "DynamicMembership" |
| Segurança | Não defina. |


>**Observação:** criar um grupo do Office 365 programaticamente sem um contexto do usuário e sem a especificação de proprietários criará o grupo anônimo.  Isso pode resultar no site do SharePoint Online associado não está sendo criado automaticamente até que ainda mais a ação manual é realizada.  

Especifique outras propriedades graváveis conforme necessário para o seu grupo. Confira mais informações nas propriedades do recurso [group](../resources/group.md).

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.

## <a name="example"></a>Exemplo
#### <a name="request-1"></a>Solicitação 1
A primeira solicitação de exemplo cria um grupo do Office 365.
<!-- {
  "blockType": "request",
  "name": "create_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="response-1"></a>Resposta 1
Este é um exemplo de resposta.
>**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

#### <a name="request-2"></a>Solicitação 2
A segunda solicitação de exemplo cria um grupo do Office 365 com proprietários especificados.
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a>Resposta 2
O exemplo a seguir é um exemplo da resposta bem-sucedida.
>**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
    "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
