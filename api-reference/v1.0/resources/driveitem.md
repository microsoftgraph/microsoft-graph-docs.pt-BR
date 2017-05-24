# <a name="driveitem-resource-type"></a>Tipo de recurso DriveItem

O recurso **DriveItem** representa um arquivo, pasta ou outro item armazenado em uma unidade. Todos os objetos do sistema de arquivos no OneDrive e no SharePoint são retornados como recursos **driveItem**.

Há duas maneiras principais de endereçar um recurso **driveItem**:

* Pelo identificador exclusivo de **driveItem** usando `drive/items/{item-id}`
* Usando o caminho do sistema de arquivos `/drive/root:/path/to/file`

Os recursos **DriveItem** têm facetas modeladas como propriedades que fornecem dados sobre as identidades e capacidades de driveItem. Por exemplo:

* As pastas têm uma [**faceta folder**](folder.md)
* Os arquivos têm uma [**faceta file**](file.md).
* As imagens têm uma [**faceta image**](image.md) além das facetas file.
* Imagens obtidas com uma câmera (fotos) se comportam como uma [**faceta photo**](photo.md) que identifica o item como uma foto e fornece as propriedades de quando a foto foi tirada e com qual dispositivo.

Itens com a faceta **folder** atuam como contêineres de itens e, portanto, têm uma referência `children` apontando para um conjunto de **driveItems** na pasta.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **driveItem**.

O recurso **driveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "children", "createdByUser", "lastModifiedByUser", "permissions", "thumbnails"],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItem"
}-->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "cTag": "string",
  "deleted": { "@odata.type": "microsoft.graph.deleted" },
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "remoteItem": { "@odata.type": "microsoft.graph.remoteItem" },
  "root": { "@odata.type": "microsoft.graph.root" },
  "searchResult": { "@odata.type": "microsoft.graph.searchResult" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "string",

  /* relationships */
  "content": { "@odata.type": "Edm.Stream" },
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],

  /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "eTag": "string",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": {"@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "string",

  /* instance annotations */
  "@microsoft.graph.conflictBehavior": "string",
  "@microsoft.graph.downloadUrl": "url",
  "@microsoft.graph.sourceUrl": "url"
}

```

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                | Descrição                                                                                                                                                               |
| :------------------- | :---------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| audio                | [audio](audio.md)                   | Metadados de áudio, se o item for um arquivo de áudio. Somente leitura.                                                                                                                  |
| createdBy            | [identitySet](identityset.md)       | Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.                                                                                          |
| createdDateTime      | DateTimeOffset                      | Data e hora de criação do item. Somente leitura.                                                                                                                                |
| cTag                 | String                              | Uma eTag para o conteúdo do item. Essa eTag não será alterada se apenas os metadados forem alterados. **Observação** Essa propriedade não será retornada se o item for uma pasta. Somente leitura. |
| deleted              | [deleted](deleted.md)               | Informações sobre o estado excluído do item. Somente leitura.                                                                                                               |
| description          | String                              | Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal                                                                                    |
| eTag                 | String                              | eTag para o item inteiro (metadados + conteúdo). Somente leitura.                                                                                                                 |
| file                 | [file](file.md)                     | Metadados de arquivo, se o item for um arquivo. Somente leitura.                                                                                                                          |
| fileSystemInfo       | [fileSystemInfo](filesysteminfo.md) | Informações do sistema de arquivos no cliente. Leitura e gravação.                                                                                                                            |
| folder               | [folder](folder.md)                 | Metadados de pasta, se o item for uma pasta. Somente leitura.                                                                                                                      |
| id                   | String                              | O identificador exclusivo do item na Unidade. Somente leitura.                                                                                                            |
| imagem                | [image](image.md)                   | Metadados de imagem, se o item for uma imagem. Somente leitura.                                                                                                                       |
| lastModifiedBy       | [identitySet](identityset.md)       | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.                                                                                    |
| lastModifiedDateTime | DateTimeOffset                      | Data e hora em que o item foi modificado pela última vez. Somente leitura.                                                                                                                      |
| location             | [geoCoordinates](geoCoordinates.md) | Metadados de localização, se o item tiver dados de localização. Somente leitura.                                                                                                              |
| nome                 | String                              | O nome do item (nome do arquivo e extensão). Leitura e gravação.                                                                                                                |
| pacote              | [package](package.md)               | Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.         |
| parentReference      | [itemReference](itemreference.md)   | Informações do pai, se o item tiver um pai. Leitura e gravação.                                                                                                                 |
| Foto                | [photo](photo.md)                   | Metadados de foto, se o item for uma foto. Somente leitura.                                                                                                                        |
| remoteItem           | [remoteItem](remoteitem.md)         | Dados do item remoto, se o item for compartilhado de uma unidade diferente daquela que está sendo acessada. Somente leitura.                                                                        |
| root                 | [root](root.md)                     | Se essa propriedade for não nula, indicará que o driveItem é o principal driveItem na unidade.                                                                     |
| searchResult         | [searchResult](searchresult.md)     | Metadados de pesquisa, se o item for de um resultado de pesquisa. Somente leitura.                                                                                                          |
| compartilhado               | [shared](shared.md)                 | Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.                                               |
| sharepointIds        | [sharepointIds](sharepointids.md)   | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.                                                                                                  |
| size                 | Int64                               | O tamanho do item em bytes. Somente leitura.                                                                                                                                     |
| specialFolder        | [specialFolder](specialfolder.md)   | Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.                                                                             |
| video                | [video](video.md)                   | Metadados de vídeo, se o item for um vídeo. Somente leitura.                                                                                                                        |
| webDavUrl            | String                              | URL compatível com WebDAV para o item.                                                                                                                                       |
| webUrl               | String                              | URL que exibe o recurso no navegador. Somente leitura.                                                                                                                 |

**Observação:** As propriedades eTag e cTag funcionam de maneira diferente em contêineres (pastas). O valor de cTag é modificado quando o conteúdo ou os metadados de qualquer descendente da pasta são alterados. O valor de eTag é modificado apenas quando as propriedades da pasta são alteradas, exceto para propriedades derivadas de descendentes (como **childCount** ou **lastModifiedDateTime**).

## <a name="relationships"></a>Relações

| Relação       | Tipo                                       | Descrição                                                                                                                                                                       |
| :----------------- | :----------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| content            | Fluxo                                     | O fluxo de conteúdo, se o item representar um arquivo.                                                                                                                                |
| children           | Coleção [driveitem](driveitem.md)       | Coleção que contêm objetos Item para os filhos imediatos do Item. Somente os itens que representam pastas têm filhos. Somente leitura. Anulável.                                        |
| createdByUser      | [user](user.md)                            | Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.                                                                                                  |
| lastModifiedByUser | [user](user.md)                            | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.                                                                                            |
| permissões        | Coleção [permission](permission.md)     | O conjunto de permissões do item. Somente leitura. Anulável.                                                                                                                         |
| miniaturas         | Coleção [thumbnailSet](thumbnailset.md) | Coleção contendo objetos [ThumbnailSet](thumbnailSet.md) associados ao item. Para saber mais, confira [obtendo miniaturas](../api/thumbnailset_get.md). Somente leitura. Anulável. |


## <a name="instance-attributes"></a>Atributos de instância

Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.

| Nome da propriedade                     | Tipo   | Descrição                                                                                                                                                         |
|:----------------------------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| @microsoft.graph.conflictBehavior | string | O comportamento de resolução de conflitos para ações que criam um novo item. Você pode usar os valores *fail*, *replace* ou *rename*. O padrão para PUT é *replace*. Um item nunca será retornado com essa anotação. Somente gravação.                               |
| @microsoft.graph.downloadUrl      | string | Uma URL que pode ser usada para baixar conteúdo desse arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.                                                    |
| @microsoft.graph.sourceUrl        | string | Quando uma solicitação PUT é emitida, essa anotação de instância pode ser usada para instruir o serviço a baixar o conteúdo da URL e armazená-lo como o arquivo. Somente gravação. |

**Observação:** O valor de @microsoft.graph.downloadUrl é uma URL de curta duração e não pode ser armazenado em cache. A URL só estará disponível por um curto período de tempo (1 hora) antes de ser invalidada.


## <a name="methods"></a>Métodos

| Método                                                 | Caminho REST
|:-------------------------------------------------------|:--------------------
| [Obter item](../api/item_get.md)                         | `GET /drive/items/{item-id}`
| [Listar filhos](../api/item_list_children.md)          | `GET /drive/items/{item-id}/children`
| [Criar item](../api/item_post_children.md)            | `POST /drive/items/{item-id}/children`
| [Atualizar item](../api/item_update.md)                   | `PATCH /drive/items/{item-id}`
| [Carregar conteúdo](../api/item_uploadcontent.md)         | `PUT /drive/items/{item-id}/content`
| [Baixar conteúdo](../api/item_downloadcontent.md)     | `GET /drive/items/{item-id}/content`
| [Excluir item](../api/item_delete.md)                   | `DELETE /drive/items/{item-id}`
| [Mover item](../api/item_move.md)                       | `PATCH /drive/items/{item-id}`
| [Copiar item](../api/item_copy.md)                       | `POST /drive/items/{item-id}/copy`
| [Pesquisar itens](../api/item_search.md)                  | `GET /drive/items/{item-id}/search(q='text')`
| [Listar alterações em uma unidade](../api/item_delta.md)        | `GET /drive/root/delta`
| [Listar miniaturas](../api/item_list_thumbnails.md)      | `GET /drive/items/{item-id}/thumbnails`  |
| [Criar link de compartilhamento](../api/item_createlink.md)       | `POST /drive/items/{item-id}/createLink` |
| [Adicionar permissões](../api/item_invite.md)               | `POST /drive/items/{item-id}/invite`     |
| [Listar permissões](../api/item_list_permissions.md)    | `GET /drive/items/{item-id}/permissions` |
| [Excluir permissão](../api/permission_delete.md)       | `DELETE /drive/items/{item-id}/permissions/{perm-id}` |


## <a name="remarks"></a>Comentários

Em bibliotecas de documentos do OneDrive for Business ou do SharePoint, a propriedade **cTag** não será retornada se o **driveItem** for uma faceta [folder](folder.md).

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "item resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
