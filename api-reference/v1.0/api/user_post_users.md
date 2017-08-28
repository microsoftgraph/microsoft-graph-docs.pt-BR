# <a name="create-user"></a>Criar Usuário

Use essa API para criar um novo Usuário. O corpo da solicitação contém o usuário a ser criado. No mínimo, você deve especificar as propriedades necessárias para o usuário. Opcionalmente, você pode especificar outras propriedades graváveis.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | 
|:--------------------|:---------------------------------------------------------| 
|Delegado (conta corporativa ou de estudante) | User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    | 
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | 
|Aplicativo | User.ReadWrite.All, Directory.ReadWrite.All | 

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.

| Parâmetro | Tipo | Descrição|
|:---------------|:--------|:----------|
|accountEnabled |booliano |true se a conta estiver habilitada; caso contrário, false.|
|displayName |string |Nome de exibição no catálogo de endereços do usuário.|
|onPremisesImmutableId |string |Só precisa ser especificado ao criar uma nova conta de usuário se você está usando um domínio federado para propriedade userPrincipalName (UPN) do usuário.|
|mailNickname |string |O alias de email do usuário.|
|passwordProfile|[PasswordProfile](../resources/passwordprofile.md) |O perfil de senha do usuário.|
|userPrincipalName |string |Nome UPN (usuario@contoso.com).|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [user](../resources/user.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
No corpo da solicitação, forneça uma representação JSON do objeto [user](../resources/user.md).
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
