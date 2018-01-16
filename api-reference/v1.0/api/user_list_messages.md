# <a name="list-messages"></a>Listar mensagens

Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).

No momento, essa operação retorna corpos de mensagens somente no formato HTML.


### <a name="get-messages-in-another-users-message-folder"></a>Receber mensagens na pasta de mensagens de outro usuário

Se você tem permissões de aplicativo ou as [permissões](#permissions) delegadas apropriadas de um usuário, é possível receber mensagens da pasta de mensagens de outro usuário. Esta seção se concentra em cenários que envolvem permissões delegadas.

Por exemplo, seu aplicativo adquiriu permissões delegadas do usuário, Diogo. Suponha que outro usuário, Henrique, tenha compartilhado uma pasta de mensagens com Diogo. Você pode receber mensagens nessa pasta compartilhada especificando a ID de usuário do Henrique (ou o nome de entidade de segurança) na consulta de exemplo mostrada abaixo.

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/messages
```

Esse recurso se aplica a todas as operações de mensagens GET com suporte a usuários individuais, como mostra a seção [Solicitação HTTP](#http-request) abaixo. Também se aplica se Henrique delegou sua caixa de correio inteira a Diogo.

Se Henrique não tiver compartilhado a pasta de mensagens dele com Diogo nem delegado a caixa de correio dele a Diogo, a especificação da ID de usuário do Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro. Nesses casos, especificar uma ID de usuário ou um nome de entidade de segurança só funcionará para receber mensagens nas próprias pastas de mensagens do usuário conectado, e a consulta será equivalente a usar o atalho /me:

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
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

Para obter todas as mensagens na caixa de correio do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

Para obter mensagens em uma pasta específica na caixa de correio do usuário:

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Prefer: outlook.body-content-type | string | O formato das propriedades **body** e **uniqueBody** a serem retornadas. Os valores podem ser "text" ou "html". Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML. Opcional. |


## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.

O tamanho de página padrão para essa solicitação é dez mensagens.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "datetime-value",
      "sentDateTime": "datetime-value",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
