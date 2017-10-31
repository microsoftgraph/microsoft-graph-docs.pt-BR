# <a name="working-with-users-in-microsoft-graph"></a>Trabalhando com usuários no Microsoft Graph

Você pode usar o Microsoft Graph para criar experiências envolventes do aplicativo com base nos usuários, em suas relações com outros usuários e em grupos e seus emails, calendário e arquivos.

Você pode acessar [usuários](user.md) pelo Microsoft Graph de duas maneiras:

- Por sua ID, `/users/{id | userPrincipalName}` 
- Usando o alias `/me` para o usuário conectado, que é igual a `/users/{signed-in user's id}`

## <a name="authorization"></a>Autorização

Uma das seguintes [permissões](https://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes) é necessária para acessar operações de usuário. As três primeiras permissões podem ser concedidas a um aplicativo por um usuário. O restante só pode ser concedido a um aplicativo pelo administrador.

- User.ReadBasic.All
- User.Read
- User.ReadWrite
- User.Read.All
- User.ReadWrite.All
- Directory.Read.All
- Directory.ReadWrite.All
- Directory.AccessAsUser.All

## <a name="common-properties"></a>Propriedades comuns

O item a seguir representa o conjunto padrão de propriedades que serão retornadas ao se obter um usuário ou listar usuários. Este é um subconjunto de todas as propriedades disponíveis. Para obter mais propriedades do usuário, use o parâmetro de consulta `$select`. 

|Propriedade |Descrição |
|:----------|:-------------|
|id | O identificador exclusivo do usuário.|
|businessPhones | Os números de telefone do usuário.|
|displayName | O nome exibido no catálogo de endereços do usuário.|
|givenName| O nome do usuário. |
|jobTitle | O cargo do usuário.|
|email| O endereço de email do usuário. |
|mobilePhone | O número de telefone celular do usuário.|
|officeLocation | O local do escritório físico do usuário.|
|preferredLanguage | O idioma preferencial do usuário.|
|surname| O sobrenome do usuário. |
|userPrincipalName| O nome UPN do usuário. |

<br/>

Para obter detalhes e uma lista de todas as propriedades, confira o objeto [user](user.md).

## <a name="common-operations"></a>Operações comuns

> **Observação:** Algumas destas operações exigem permissões adicionais.

| Path    | Descrição |
|:---------|:-------------|
|[`/users`](../api/user_list.md) | Lista os usuários na organização. |
|[`/users/{id}`](../api/user_get.md) | Obtém um usuário específico pela id. |
|[`/users/{id}/photo/$value`](../api/profilephoto_get.md)| Obtém a foto de perfil do usuário. |
|[`/users/{id}/manager`](../api/user_list_manager.md) | Obtém o gerente do usuário. |
|[`/users/{id}/messages`](../api/user_list_messages.md)| Lista as mensagens de email do usuário em sua caixa de entrada principal. |
|[`/users/{id}/events`](../api/user_list_events.md) | Lista os eventos futuros do usuário em seu calendário. |
|[`/users/{id}/drive`](../api/drive_get.md)| Obtém o repositório de arquivos do OneDrive do usuário. |
|[`/users/{id}/memberOf`](../api/user_list_memberof.md)| Lista os grupos dos quais o usuário é membro. |
