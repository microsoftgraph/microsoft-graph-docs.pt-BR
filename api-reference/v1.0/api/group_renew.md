# <a name="group-renew"></a>group: renew

Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).
 

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.ReadWrite.All ou Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte |
|Aplicativo | Group.ReadWrite.All ou Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /groups/<id>/renew
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:---------------|:----------|
| Autorização  | Portador {token} |


## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/<id>/renew
```

##### <a name="response"></a>Resposta
Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->