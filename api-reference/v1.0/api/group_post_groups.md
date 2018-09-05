# <a name="create-group"></a>Criar grupo
Use esta API para criar um novo grupo conforme especificado no corpo da solicitação. Você pode criar um dos três tipos de grupos:

* Grupo do Office 365 (grupo unificado)
* Grupo dinâmico
* Grupo de segurança

> **Observação**: embora o Microsoft Teams tenha como base grupos do Office 365, não é possível criar uma equipe por meio desta API atualmente. Você pode usar outras APIs de grupos para gerenciar uma equipe que foi criada na interface do usuário do Microsoft Teams.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

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
| Autorização  | sequência de caracteres  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
A tabela a seguir mostra as propriedades do recurso [group](../resources/group.md) que você deve especificar ao criar um grupo. 

| Propriedade | Tipo | Descrição|
|:---------------|:--------|:----------|
| displayName | sequência de caracteres | O nome de exibição no catálogo de endereços do grupo. Obrigatório. |
| mailEnabled | booleano | Defina como **true** para grupos habilitados para email. Defina como **true** se estiver criando um grupo no Office 365. Defina como **false** se estiver criando um grupo dinâmico ou de segurança. Obrigatório. |
| mailNickname | sequência de caracteres | O alias de email do grupo. Obrigatório. |
| securityEnabled | booleano | Defina como **true** para grupos habilitados para segurança. Defina como **true** se estiver criando um grupo dinâmico ou de segurança. Defina como **false** se estiver criando um grupo no Office 365. Obrigatório. |
| owners | coleção de sequência de caracteres | Essa propriedade representa os proprietários do grupo no momento da criação. Opcional. |
| members | coleção de sequência de caracteres | Essa propriedade representa os membros do grupo no momento da criação. Opcional. |


Especifique a propriedade **groupTypes** se estiver criando um grupo do Office 365 ou um grupo dinâmico, conforme descrito a seguir.

### <a name="grouptypes-options"></a>opções de groupTypes

| Tipo de grupo | Propriedade **groupTypes** |
|:--------------|:------------------------|
| Office 365 (também conhecido como grupo unificado)| "Unified" |
| Dinâmico | "DynamicMembership" |
| Segurança | Não defina. |


>**Observação:** Criar um grupo do Office 365 via programação sem um contexto de usuário e sem a especificação de proprietários criará o grupo de forma anônima.  Dessa forma, o site associado do SharePoint Online poderá não ser criado automaticamente até que uma ação manual seja realizada.  

Especifique outras propriedades graváveis para o seu grupo conforme necessário. Para obter mais informações, confira as propriedades do recurso [group](../resources/group.md).

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [group](../resources/group.md) no corpo da resposta.

## <a name="example"></a>Exemplo
#### <a name="request-1"></a>Solicitação 1
O primeiro exemplo de solicitação cria um grupo do Office 365.
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
>**Observação:** o objeto response mostrado aqui pode ser encurtado para melhor legibilidade. Todas as propriedades serão retornadas em uma chamada real.
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
O segundo exemplo de solicitação cria um grupo do Office 365 com proprietários especificados.
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
Este é um exemplo de uma resposta bem-sucedida.
>**Observação:** o objeto response mostrado aqui pode ser encurtado para melhor legibilidade. Todas as propriedades serão retornadas em uma chamada real.
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
