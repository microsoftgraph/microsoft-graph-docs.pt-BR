# <a name="create-a-sharing-link-for-a-driveitem"></a>Criar um link de compartilhamento para um DriveItem

Você pode usar a ação **createLink** para compartilhar um [DriveItem](../resources/driveitem.md) por meio de um link de compartilhamento.

A ação **createLink** criará um novo link de compartilhamento se o tipo de link especificado não existir para o aplicativo de chamada. Se um link de compartilhamento do tipo especificado já existir para o aplicativo, o link de compartilhamento existente será retornado.

Recursos de DriveItem herdam permissões de seus ancestrais.

## <a name="prerequisites"></a>Pré-requisitos
Um dos seguintes **escopos** é obrigatório para executar esta API:

  * Files.ReadWrite

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/createLink
POST /me/drive/root:/{item-path}:/createLink
POST /groups/{group-id}/drive/items/{item-id}/createLink
POST /drives/{drive-id}/items/{item-id}/createLink
```

## <a name="request-body"></a>Corpo da solicitação
O corpo da solicitação define o tipo de link de compartilhamento que seu aplicativo está procurando. A solicitação deve ser um objeto JSON com essa propriedade.

| Name      | Tipo   | Descrição                                                                  |
|:----------|:-------|:-----------------------------------------------------------------------------|
| **type**  | string | O tipo de link de compartilhamento a ser criado. Pode ser `view`, `edit` ou `embed`.       |
| **scope** | cadeia de caracteres | O escopo do link a ser criado. Pode ser `anonymous` ou `organization`. Opcional. |

## <a name="link-types"></a>Tipos de link
Os seguintes valores são permitidos para o parâmetro **type**.

| Valor do tipo | Descrição                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | Cria um link somente leitura para o item.                                                        |
| `edit`     | Cria um link de leitura e gravação para o item.                                                       |
| `embed`    | Cria um link inserível para o item. Essa opção só está disponível para uso pessoal do OneDrive. |

## <a name="scope-types"></a>Tipos de escopo
Os seguintes valores são permitidos para o parâmetro **scope**. Esse é um parâmetro opcional. Se o parâmetro **scope** não for especificado, o link mais permissivo disponível será criado.

| Valor do tipo     | Descrição                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | Cria um link para o item que pode ser acessado por qualquer pessoa. Links anônimos podem estar desabilitados pelo administrador de locatários.                 |
| `organization` | Cria um link para o item que pode ser acessado dentro de uma organização. O escopo de link de organização não está disponível para uso pessoal do OneDrive. |

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um único recurso [Permission](../resources/permission.md) no corpo da resposta, que representa a permissão solicitada do link de compartilhamento.

O serviço primeiro examinará as permissões atuais e verificará se já existe uma permissão com o mesmo valor de **type** para o aplicativo de chamada.

A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.

## <a name="example"></a>Exemplo
Eis um exemplo de como chamar esta API.

##### <a name="request"></a>Solicitação
Veja a seguir um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

##### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a>Criando links compartilháveis pela empresa

O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa. Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros do locatário proprietário. Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->
```
POST https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

## <a name="http-response"></a>Resposta HTTP

A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="embeddable-links"></a>Links inseríveis

Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.

**Observação:** Links de inserção apenas têm suporte em [Drives](../resources/drive.md), em que **driveType** é `personal`.

## <a name="remarks"></a>Comentários

* Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.
* Os links ficam visíveis nas permissões de compartilhamento do item e podem ser removidos por um proprietário desse item.
* Os links sempre apontam para a versão atual de um item, a menos que esse item esteja em check-out (apenas no SharePoint).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item: createLink",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Create sharing link"
} -->
