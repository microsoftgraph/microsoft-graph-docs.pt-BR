# <a name="list-contacts"></a>Listar contatos

Obter uma coleção de contatos da pasta Contatos padrão do usuário conectado.


### <a name="get-contacts-in-another-users-contact-folder"></a>Obter contatos na pasta de contatos de outro usuário

Se você tiver permissões de aplicativo ou se você tiver as [permissões](#permissions) delegadas apropriadas de um usuário, será possível obter os contatos da pasta de contatos de outro usuário. Esta seção se concentra em cenários que envolvem permissões delegadas.

Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo. Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de contatos com Diogo. Você pode obter os contatos nessa pasta compartilhada especificando a ID de usuário de Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

Esse recurso se aplica a todas as operações de contatos GET com suporte para usuários individuais, conforme listado na seção [solicitação HTTP](#http-request) abaixo. Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.

Se Henrique não tiver compartilhado sua pasta de contatos com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro. Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para obter contatos nas próprias pastas de contatos do usuário conectado, e a consulta será equivalente a usar o atalho /me:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
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
|Delegado (conta corporativa ou de estudante) | Contacts.Read, Contacts.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Contacts.Read, Contacts.ReadWrite    |
|Aplicativo | Contacts.Read, Contacts.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP

Para obter todos os contatos na caixa de correio do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

Para obter os contatos em uma pasta específica na caixa de correio do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.

Por exemplo, você pode usar o parâmetro de consulta `$filter` para filtrar os contatos com base no domínio dos endereços de email deles:

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type   | application/json  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Contact](../resources/contact.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
