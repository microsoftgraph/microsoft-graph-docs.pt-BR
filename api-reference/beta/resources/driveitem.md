---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.openlocfilehash: 255b9de7ad565228da093a9a40d23c3360df28b2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882261"
---
# <a name="driveitem-resource-type"></a>tipo de recurso de driveItem

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "content": { "@odata.type": "Edm.Stream" },
  "children": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "thumbnails": [ {"@odata.type": "microsoft.graph.thumbnailSet"}],
  "versions": [ {"@odata.type": "Collection(microsoft.graph.driveItemVersion)"}],

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
| createdBy            | [identitySet][]    | Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.
| createdDateTime      | DateTimeOffset     | Data e hora de criação do item. Somente leitura.
| cTag                 | String             | Uma eTag para o conteúdo do item. Essa eTag não será alterada se apenas os metadados forem alterados. **Observação** Essa propriedade não será retornada se o item for uma pasta. Somente leitura.
| deleted              | [deleted][]        | Informações sobre o estado excluído do item. Somente leitura.
| description          | String             | Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal
| eTag                 | String             | eTag para o item inteiro (metadados + conteúdo). Somente leitura.
| file                 | [file][]           | Metadados de arquivo, se o item for um arquivo. Somente leitura.
| fileSystemInfo       | [fileSystemInfo][] | Informações do sistema de arquivos no cliente. Leitura e gravação.
| folder               | [folder][]         | Metadados de pasta, se o item for uma pasta. Somente leitura.
| id                   | String             | O identificador exclusivo do item na Unidade. Somente leitura.
| image                | [image][]          | Metadados de imagem, se o item for uma imagem. Somente leitura.
| lastModifiedBy       | [identitySet][]    | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.
| lastModifiedDateTime | DateTimeOffset     | Data e hora em que o item foi modificado pela última vez. Somente leitura.
| location             | [geoCoordinates][] | Metadados de localização, se o item tiver dados de localização. Somente leitura.
| name                 | String             | O nome do item (nome do arquivo e extensão). Leitura e gravação.
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
| webDavUrl            | String             | URL compatível com WebDAV para o item.
| webUrl               | String             | URL que exibe o recurso no navegador. Somente leitura.

**Observação:** As propriedades eTag e cTag funcionam de maneira diferente em contêineres (pastas). O valor de cTag é modificado quando o conteúdo ou os metadados de qualquer descendente da pasta são alterados. O valor de eTag é modificado apenas quando as propriedades da pasta são alteradas, exceto para propriedades derivadas de descendentes (como **childCount** ou **lastModifiedDateTime**).

## <a name="relationships"></a>Relações

| Relação       | Tipo                            | Descrição
|:-------------------|:--------------------------------|:--------------------------
| activities         | Conjunto [itemActivity][]     | A lista de atividades recentes que ocorreram neste item.
| análise          | recurso de [itemAnalytics][]      | Análise sobre as atividades de modo de exibição que foram realizada neste item.
| content            | Fluxo                          | O fluxo de conteúdo, se o item representar um arquivo.
| children           | Conjunto driveitem            | Conjunto que contêm objetos Item para os filhos imediatos de Item. Somente os itens que representam pastas têm filhos. Somente leitura. Anulável.
| listItem           | [listItem][]                    | Para as unidades no SharePoint, o item de lista da biblioteca de documento associado. Somente leitura. Anulável.
| permissions        | Coleção [permission][]       | O conjunto de permissões do item. Somente leitura. Anulável.
| miniaturas         | Coleção [thumbnailSet][]     | Coleção contendo objetos [ThumbnailSet][] associados ao item. Para saber mais, confira [obtendo miniaturas][]. Somente leitura. Anulável.
| versions           | coleção [driveItemVersion][] | Lista de versões anteriores do item. Para obter mais informações, consulte a [obtenção de versões anteriores][]. Somente leitura. Anulável.

## <a name="instance-attributes"></a>Atributos de instância

Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.

| Nome da propriedade                     | Tipo   | Descrição
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | string | O comportamento de resolução de conflitos para ações que criam um novo item. Você pode usar os valores *fail*, *replace* ou *rename*. O padrão para PUT é *replace*. Um item nunca será retornado com essa anotação. Somente gravação.
| @microsoft.graph.downloadUrl      | string | Uma URL que pode ser usada para baixar conteúdo desse arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.
| @microsoft.graph.sourceUrl        | string | Quando uma solicitação PUT é emitida, essa anotação de instância pode ser usada para instruir o serviço a baixar o conteúdo da URL e armazená-lo como o arquivo. Somente gravação.

**Observação:** O valor de @microsoft.graph.downloadUrl é uma URL de curta duração e não pode ser armazenados em cache.
A URL só estará disponível por um curto período de tempo (1 hora) antes de ele será invalidado. Remover permissões de arquivo para um usuário não pode invalidar a URL imediatamente.

## <a name="methods"></a>Métodos

| Método                                                   | Caminho REST
|:---------------------------------------------------------|:------------------
| [Obter item](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [Listar atividades](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| [Obtenha a análise][]                                        | `GET /drive/items/{item-id}/analytics`
| [Fazer atividades pelo intervalo][]                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [Listar filhos](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [Listar versões](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [Criar item](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [Atualizar item](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [Carregar conteúdo](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [Baixar conteúdo](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| [Baixar formato de arquivo específico][download-format]         | `GET /drive/items/{item-id}/content?format={format}`
| [Excluir item](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [Mover item](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [Copiar item](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [Pesquisar itens](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [Listar alterações em uma unidade](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [Listar miniaturas](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [Criar um link de compartilhamento](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [Adicionar permissões](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [Listar permissões](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [Excluir permissão](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| [Obtenha o canal WebSocket][getWebSocket]                    | `GET /drive/root/subscriptions/socketIo`
| [Item de visualização][item-preview]                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[Obtenha a análise]: ../api/itemanalytics-get.md
[Fazer atividades pelo intervalo]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a>Comentários

Em bibliotecas de documentos do OneDrive for Business ou do SharePoint, a propriedade **cTag** não será retornada se **driveItem** for uma faceta [folder][].

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[obtenção de versões anteriores]: ../api/driveitem-list-versions.md
[obtendo miniaturas]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
[listItem]: listitem.md
[package]: package.md
[permission]: permission.md
[photo]: photo.md
[remoteItem]: remoteitem.md
[root]: root.md
[searchResult]: searchresult.md
[compartilhado]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[thumbnailSet]: thumbnailset.md
[video]: video.md
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
