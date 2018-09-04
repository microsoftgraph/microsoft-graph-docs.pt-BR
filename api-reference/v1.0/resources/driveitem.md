---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 60f2d58331f349f9990f78f36f04df055ce90b9e
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23269835"
---
# <a name="driveitem-resource-type"></a>Tipo de recurso DriveItem

O recurso **DriveItem** representa um arquivo, pasta ou outro item armazenado em uma unidade. Todos os objetos do sistema de arquivos no OneDrive e no SharePoint são retornados como recursos **driveItem**.

Há duas maneiras principais de endereçar um recurso **driveItem**:

* Pelo identificador exclusivo de **driveItem** usando `drive/items/{item-id}`
* Usando o caminho do sistema de arquivos `/drive/root:/path/to/file`

Os recursos **DriveItem** têm facetas modeladas como propriedades que fornecem dados sobre as identidades e capacidades de driveItem. Por exemplo:

* As pastas têm uma [**faceta folder**][folder]
* Os arquivos têm uma [**faceta file**][file].
* As imagens têm uma [**faceta image**][image], além de facetas file.
* Imagens obtidas com uma câmera (fotos) têm uma [**faceta photo**][photo] que identifica o item como uma foto e fornece as propriedades de quando foi tirada e com qual dispositivo.

Itens com a faceta **folder** atuam como contêineres de itens e, portanto, têm uma referência `children` apontando para um conjunto de **driveItems** na pasta.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON de um recurso **driveItem**.

O recurso **driveItem** é derivado de [**baseItem**][baseItem] e herda propriedades desse recurso.

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
       "baseType": "microsoft.graph.baseItem",
       "optionalProperties": ["cTag", "children", "folder", "file", "image", "audio", "video",
       "location", "deleted", "specialFolder", "photo", "thumbnails", "searchResult", "remoteItem",
       "shared", "content", "@microsoft.graph.conflictBehavior", "@microsoft.graph.downloadUrl", "@content.sourceUrl",
       "sharepointIds"],
       "keyProperty": "id", "openType": true } -->

```json
{
  "audio": { "@odata.type": "microsoft.graph.audio" },
  "content": { "@odata.type": "Edm.Stream" },
  "cTag": "string (etag)",
  "deleted": { "@odata.type": "microsoft.graph.deleted"},
  "description": "string",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image": { "@odata.type": "microsoft.graph.image" },
  "location": { "@odata.type": "microsoft.graph.geoCoordinates" },
  "package": { "@odata.type": "microsoft.graph.package" },
  "photo": { "@odata.type": "microsoft.graph.photo" },
  "publication": {"@odata.type": "microsoft.graph.publicationFacet"},
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
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "microsoft.graph.driveItemVersion"}],

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

| Propriedade             | Tipo               | Descrição
|:---------------------|:-------------------|:---------------------------------
| audio                | [audio][]          | Metadados de áudio, se o item for um arquivo de áudio. Somente leitura.
| content              | Fluxo             | O fluxo de conteúdo, se o item representar um arquivo.
| createdBy            | [identitySet][]    | Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.
| createdDateTime      | DateTimeOffset     | Data e hora de criação do item. Somente leitura.
| cTag                 | Sequência de caracteres             | Uma eTag para o conteúdo do item. Essa eTag não será alterada se apenas os metadados forem alterados. **Observação** Essa propriedade não será retornada se o item for uma pasta. Somente leitura.
| deleted              | [deleted][]        | Informações sobre o estado excluído do item. Somente leitura.
| description          | Sequência de caracteres             | Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal
| eTag                 | Sequência de caracteres             | eTag para o item inteiro (metadados + conteúdo). Somente leitura.
| file                 | [file][]           | Metadados de arquivo, se o item for um arquivo. Somente leitura.
| fileSystemInfo       | [fileSystemInfo][] | Informações do sistema de arquivos no cliente. Leitura e gravação.
| folder               | [folder][]         | Metadados de pasta, se o item for uma pasta. Somente leitura.
| id                   | Sequência de caracteres             | O identificador exclusivo do item na Unidade. Somente leitura.
| imagem                | [image][]          | Metadados de imagem, se o item for uma imagem. Somente leitura.
| lastModifiedBy       | [identitySet][]    | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.
| lastModifiedDateTime | DateTimeOffset     | Data e hora em que o item foi modificado pela última vez. Somente leitura.
| location             | [geoCoordinates][] | Metadados de localização, se o item tiver dados de localização. Somente leitura.
| name                 | Sequência de caracteres             | O nome do item (nome do arquivo e extensão). Leitura e gravação.
| pacote              | [package][]        | Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.
| parentReference      | [itemReference][]  | Informações do pai, se o item tiver um pai. Leitura e gravação.
| Foto                | [photo][]          | Metadados de foto, se o item for uma foto. Somente leitura.
| publication          | [publicationFacet][] | Fornece informações sobre o estado de publicação ou de check-out de um item, nos locais que oferecem suporte a essas ações. Esta propriedade não retorna por padrão. Somente leitura. |
| remoteItem           | [remoteItem][]     | Dados do item remoto, se o item for compartilhado de uma unidade diferente daquela que está sendo acessada. Somente leitura.
| root                 | [root][]           | Se essa propriedade for não nula, indicará que o driveItem é o principal driveItem na unidade.
| searchResult         | [searchResult][]   | Metadados de pesquisa, se o item for de um resultado de pesquisa. Somente leitura.
| shared               | [shared][]         | Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.
| sharepointIds        | [sharepointIds][]  | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| size                 | Int64              | O tamanho do item em bytes. Somente leitura.
| specialFolder        | [specialFolder][]  | Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.
| video                | [video][]          | Metadados de vídeo, se o item for um vídeo. Somente leitura.
| webDavUrl            | Sequência de caracteres             | URL compatível com WebDAV para o item.
| webUrl               | Sequência de caracteres             | URL que exibe o recurso no navegador. Somente leitura.

**Observação:** As propriedades eTag e cTag funcionam de maneira diferente em contêineres (pastas). O valor de cTag é modificado quando o conteúdo ou os metadados de qualquer descendente da pasta são alterados. O valor de eTag é modificado apenas quando as propriedades da pasta são alteradas, exceto para propriedades derivadas de descendentes (como **childCount** ou **lastModifiedDateTime**).

## <a name="relationships"></a>Relações

| Relação       | Tipo                        | Descrição
|:-------------------|:----------------------------|:--------------------------
| children           | Coleção driveItem        | Conjunto que contêm objetos Item para os filhos imediatos de Item. Somente os itens que representam pastas têm filhos. Somente leitura. Anulável.
| createdByUser      | [user][]                    | A identidade do usuário que criou o item. Somente leitura.
| lastModifiedByUser | [user][]                    | A identidade do usuário que modificou o item pela última vez. Somente leitura.
| listItem           | [listItem][]                | Para as unidades no SharePoint, o item associado de lista da biblioteca de documentos. Somente leitura. Anulável.
| permissions        | Coleção [permission][]   | O conjunto de permissões do item. Somente leitura. Anulável.
| miniaturas         | Coleção [thumbnailSet][] | Coleção contendo objetos [ThumbnailSet][] associados ao item. Para saber mais, confira [obter miniaturas][]. Somente leitura. Anulável.
| versions           | Coleção [driveItemVersion][] | Lista de versões anteriores do item. Para obter mais informações, consulte [obter de versões anteriores][]. Somente leitura. Anulável.
| workbook           | [workbook][]                | Para arquivos de planilhas do Excel, acessa a pasta de trabalho API para trabalhar com o conteúdo da planilha. Anulável.

## <a name="instance-attributes"></a>Atributos de instância

Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.

| Nome da propriedade                     | Tipo   | Descrição
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | sequência de caracteres | O comportamento de resolução de conflitos para ações que criam um novo item. Você pode usar os valores *fail*, *replace* ou *rename*. O padrão para PUT é *replace*. Um item nunca será retornado com essa anotação. Somente gravação.
| @microsoft.graph.downloadUrl      | sequência de caracteres | Uma URL que pode ser usada para baixar conteúdo desse arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.
| @microsoft.graph.sourceUrl        | sequência de caracteres | Quando uma solicitação PUT é emitida, essa anotação de instância pode ser usada para instruir o serviço a baixar o conteúdo da URL e armazená-lo como o arquivo. Somente gravação.

**Observação:** O valor de @microsoft.graph.downloadUrl é uma URL de curta duração e não pode ser armazenado em cache. A URL só estará disponível por um curto período de tempo (1 hora) antes de ser invalidada.

## <a name="methods"></a>Métodos

| Método                                                   | Caminho REST
|:---------------------------------------------------------|:------------------
| [Obter item](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [Listar filhos](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [Listar versões](../api/driveitem_list_versions.md)       | `GET /drive/items/{item-id}/versions`
| [Criar item](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [Atualizar item](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [Carregar conteúdo](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [Baixar conteúdo](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| [Baixar formato de arquivo específico][download-format]         | `GET /drive/items/{item-id}/content?format={format}`
| [Excluir item](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [Mover item](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [Copiar item](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [Pesquisar itens](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [Listar alterações em uma unidade](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [Listar miniaturas](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [Criar um link de compartilhamento](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [Adicionar permissões](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [Listar permissões](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Excluir permissão](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a>Comentários

Em bibliotecas de documentos do OneDrive for Business ou do SharePoint, a propriedade **cTag** não será retornada se **driveItem** for uma faceta [folder][].

[audio]: audio.md
[baseItem]: baseItem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[driveItemVersion]: driveItemVersion.md
[file]: file.md
[fileSystemInfo]: fileSystemInfo.md
[folder]: folder.md
[obter versões anteriores]: ../api/driveitem_list_versions.md
[obter miniaturas]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
[listItem]: listItem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteItem.md
[root]: root.md
[searchResult]: searchResult.md
[compartilhado]: shared.md
[sharepointIds]: sharepointIds.md
[specialFolder]: specialFolder.md
[thumbnailSet]: thumbnailSet.md
[video]: video.md
[workbook]: workbook.md
[user]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
