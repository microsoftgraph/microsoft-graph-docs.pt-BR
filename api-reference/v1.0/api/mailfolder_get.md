# <a name="get-mailfolder"></a>Obter mailFolder

Recupere as propriedades e os relacionamentos de um objeto da pasta de mensagens.


### <a name="get-another-users-message-folder"></a>Receber a pasta de mensagens de outro usuário

Se você tem permissões de aplicativo ou as [permissões](#permissions) delegadas apropriadas de um usuário, é possível receber a pasta de mensagens de outro usuário. Esta seção se concentra em cenários que envolvem permissões delegadas.

Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo. Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de mensagens com Diogo. Você pode obter essa pasta compartilhada especificando a ID de usuário de Henrique (ou nome de entidade de segurança) na consulta de exemplo mostrada abaixo.

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/mailFolders/{id}
```

Esse recurso se aplica a todas as operações de pastas de mensagens GET para usuários individuais, conforme descrito na seção [Solicitação HTTP](#http-request) abaixo. Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.

Se Henrique não tiver compartilhado a pasta de mensagens dele com Diogo nem delegado a caixa de correio dele a Diogo, a especificação da ID de usuário do Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro. Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para receber a pasta de mensagens do usuário conectado, e a consulta será equivalente a usar o atalho /me:

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
```

Esse recurso só está disponível nas operações GET de:

- Pastas de contatos, calendários e pastas de mensagens compartilhados 
- Contatos, eventos e mensagens em pastas compartilhadas
- Os recursos acima em caixas de correio delegadas

Esse recurso não está disponível em outras operações para contatos, eventos, mensagens e respectivas pastas.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.Read, Mail.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Mail.Read, Mail.ReadWrite    |
|Aplicativo | Mail.Read, Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailFolder](../resources/mailfolder.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
