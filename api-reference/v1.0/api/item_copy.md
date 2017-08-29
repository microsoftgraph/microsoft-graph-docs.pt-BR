# <a name="copy-a-driveitem"></a>Copiar um DriveItem

Cria uma cópia de um [driveItem](../resources/driveitem.md) (incluindo todos os filhos) em um novo pai ou com um novo nome.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
```
POST /me/drive/items/{item-id}/copy
POST /me/drive/root:/{path}:/copy
POST /groups/{group-id}/drive/items/{item-id}/copy
```

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.


| Nome            | Valor                                          | Descrição                                                                                                 |
|:----------------|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------|
| parentReference | [ItemReference](../resources/itemreference.md) | Opcional. Referência ao item pai em que a cópia será criada.                                         |
| name            | string                                         | Opcional. O novo nome para a cópia. Se isso não for fornecido, será usado o mesmo nome que o original.    |

**Observação:** _parentReference_ deve incluir um `id` ou `path` mas não ambos. Se ambos forem incluídos, precisarão fazer referência ao mesmo item ou ocorrerá um erro.

## <a name="example"></a>Exemplo

<!-- { "blockType": "request", "name": "copy-item", "scopes": "files.readwrite" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "contoso plan.docx"
}
```

## <a name="response"></a>Resposta

Retorna detalhes sobre como monitorar o progresso da cópia após aceitar a solicitação.

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 202 Accepted
```

## <a name="remarks"></a>Comentários

Em muitos casos, a ação de copiar é executada de forma assíncrona. A resposta da API só indicará que a operação de cópia foi aceita ou rejeitada, por exemplo, porque o nome de arquivo de destino já está sendo utilizado.

**Observação:** A API não fornece um método para saber se a cópia foi bem-sucedida.

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Copy"
} -->
