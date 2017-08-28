# <a name="get-directory-objects-from-a-list-of-ids"></a>Obter objetos directory a partir de uma lista de ids

Retorna os objetos directory especificados a partir de uma lista de ids  OBSERVAÇÃO: Os objetos de diretório retornados são os objetos completos que contêm **todas** as propriedades. A opção `$select` não está disponível para todos os tipos de arquivo.

Alguns usos comuns dessa função são:

* Resolver ids retornadas por funções (que retornam coleções de ids) como [getMemberObjects](directoryobject_getmemberobjects.md) ou [getMemberGroups](directoryobject_getmembergroups.md) para seus objetos de diretório de suporte.
* Resolver ids que persistem em um repositório externo pelo aplicativo para seus objetos de diretório de suporte.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | 
|:--------------------|:---------------------------------------------------------| 
|Delegado (conta corporativa ou de estudante) | Directory.Read.All, Directory.AccessAsUser.All    | 
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | 
|Aplicativo | Directory.Read.All | 

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getById
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro   | Tipo |Descrição|
|:---------------|:--------|:----------|
|ids|Coleção de cadeias de caracteres| Uma coleção de ids para a qual retornar objetos. Você pode especificar até 1000 ids. |
|tipos|Coleção de cadeias de caracteres| Uma coleção de tipos de recursos que especifica o conjunto de coleções de recursos para pesquisar. Se não estiver especificado, o padrão será [directoryObject](../resources/directoryobject.md), que contém todos os tipos de recursos definidos no diretório. Qualquer objeto derivado de `directoryObject` pode ser especificado na coleção. Por exemplo: [usuário](../resources/user.md), [grupo](../resources/group.md), [dispositivo](../resources/device.md) e assim por diante. Os valores não diferenciam maiúsculas de minúsculas.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200, OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a>Resposta

Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
