# <a name="delete-open-extension"></a>Excluir extensão aberta

Exclua uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) da instância especificada de um recurso. 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é necessária para chamar essa API, dependendo do recurso do qual você está excluindo a extensão. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|**Recurso com suporte**|**Permissão**|**Recurso com suporte**|**Permissão** |
|:-----|:-----|:-----|:-----|
| [dispositivo](../resources/device.md) | Device.ReadWrite.All | [evento](../resources/event.md) | Calendars.ReadWrite |
| [grupo](../resources/group.md) | Group.ReadWrite.All | [evento de grupo](../resources/event.md) | Group.ReadWrite.All |
| [postagem de grupo](../resources/post.md) | Group.ReadWrite.All | [mensagem](../resources/message.md) | Mail.ReadWrite |
| [organização](../resources/organization.md) | Directory.AccessAsUser.All | [contato pessoal](../resources/contact.md) | Contacts.ReadWrite |
| [usuário](../resources/user.md) | Directory.AccessAsUser.All | | |

## <a name="http-request"></a>Solicitação HTTP
Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `DELETE` nessa instância de extensão.

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

>**Observação:** a sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso para excluir uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à exclusão de extensões abertas delas de maneira semelhante.

## <a name="parameters"></a>Parâmetros
|**Parâmetro**|**Tipo**|**Descrição**|
|:-----|:-----|:-----|
|_Parâmetros de URL_|
|id|string|Um identificador exclusivo para uma instância na coleção correspondente. Obrigatório.|
|extensionId|string|Pode ser um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.|

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Valor |
|:---------------|:----------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O primeiro exemplo referencia uma extensão por seu nome e exclui a extensão da mensagem especificada.
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

O segundo exemplo exclui uma extensão no evento de grupo especificado.

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->