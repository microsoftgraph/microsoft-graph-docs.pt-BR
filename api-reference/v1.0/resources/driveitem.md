---
author: JeremyKelley
ms.author: JeremyKelley
title: tipo de recurso driveItem
description: Item é o principal modelo de dados na API do OneDrive. Tudo é um item.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 2d80c6cf2b121f606938e533a6428e2d85d54033
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968790"
---
# <a name="driveitem-resource-type"></a>tipo de recurso driveItem

O recurso **DriveItem** representa um arquivo, pasta ou outro item armazenado em uma unidade. Todos os objetos do sistema de arquivos no OneDrive e no SharePoint são retornados como recursos **driveItem**.

Há duas maneiras principais de endereçar um recurso **driveItem**:

* Pelo identificador exclusivo de **driveItem** usando `drive/items/{item-id}`
* Usando o caminho do sistema de arquivos `/drive/root:/path/to/file`

Os recursos de **driveItem** têm facetas modeladas como propriedades que fornecem dados sobre as identidades e recursos do driveItem.
Por exemplo:

* As pastas têm uma [**faceta folder**][folder]
* Os arquivos têm uma [**faceta file**][file].
* As imagens têm uma [**faceta image**][image], além de facetas file.
* Imagens obtidas com uma câmera (fotos) têm uma [**faceta photo**][photo] que identifica o item como uma foto e fornece as propriedades de quando foi tirada e com qual dispositivo.

Itens com a faceta **folder** atuam como contêineres de itens e, portanto, têm uma referência `children` apontando para um conjunto de **driveItems** na pasta.

>**Observação:** No OneDrive for Business ou nas bibliotecas de documentos do SharePoint, a propriedade **cTag** não é retornada se o **driveItem** tiver uma faceta de [pasta][].

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo               | Descrição
|:---------------------|:-------------------|:---------------------------------
| audio                | [audio][]          | Metadados de áudio, se o item for um arquivo de áudio. Somente leitura.
| conteúdo              | Fluxo             | O fluxo de conteúdo, se o item representar um arquivo.
| createdBy            | [identitySet][]    | Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.
| createdDateTime      | DateTimeOffset     | Data e hora de criação do item. Somente leitura.
| cTag                 | String             | Uma eTag para o conteúdo do item. Essa eTag não será alterada se apenas os metadados forem alterados. **Observação** Essa propriedade não será retornada se o item for uma pasta. Somente leitura.
| deleted              | [deleted][]        | Informações sobre o estado excluído do item. Somente leitura.
| descrição          | String             | Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal
| eTag                 | String             | eTag para o item inteiro (metadados + conteúdo). Somente leitura.
| file                 | [file][]           | Metadados de arquivo, se o item for um arquivo. Somente leitura.
| fileSystemInfo       | [fileSystemInfo][] | Informações do sistema de arquivos no cliente. Leitura e gravação.
| folder               | [folder][]         | Metadados de pasta, se o item for uma pasta. Somente leitura.
| id                   | String             | O identificador exclusivo do item na Unidade. Somente leitura.
| imagem                | [image][]          | Metadados de imagem, se o item for uma imagem. Somente leitura.
| lastModifiedBy       | [identitySet][]    | Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.
| lastModifiedDateTime | DateTimeOffset     | Data e hora em que o item foi modificado pela última vez. Somente leitura.
| location             | [geoCoordinates][] | Metadados de localização, se o item tiver dados de localização. Somente leitura.
| nome                 | String             | O nome do item (nome do arquivo e extensão). Leitura e gravação.
| pacote              | [package][]        | Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.
| parentReference      | [itemReference][]  | Informações do pai, se o item tiver um pai. Leitura e gravação.
| Foto                | [photo][]          | Metadados de foto, se o item for uma foto. Somente leitura.
| publication          | [publicationFacet][] | Fornece informações sobre o estado de publicação ou de check-out de um item, nos locais que oferecem suporte a essas ações. Esta propriedade não retorna por padrão. Somente leitura. |
| remoteItem           | [remoteItem][]     | Dados do item remoto, se o item for compartilhado de uma unidade diferente daquela que está sendo acessada. Somente leitura.
| root                 | [root][]           | Se essa propriedade for não nula, indicará que o driveItem é o principal driveItem na unidade.
| searchResult         | [searchResult][]   | Metadados de pesquisa, se o item for de um resultado de pesquisa. Somente leitura.
| compartilhado               | [compartilhado][]         | Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.
| sharepointIds        | [sharepointIds][]  | Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.
| size                 | Int64              | O tamanho do item em bytes. Somente leitura.
| specialFolder        | [specialFolder][]  | Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.
| video                | [video][]          | Metadados de vídeo, se o item for um vídeo. Somente leitura.
| webDavUrl            | String             | URL compatível com WebDAV para o item.
| webUrl               | String             | URL que exibe o recurso no navegador. Somente leitura.

**Observação:** As propriedades eTag e cTag funcionam de maneira diferente em contêineres (pastas). O valor de cTag é modificado quando o conteúdo ou os metadados de qualquer descendente da pasta são alterados. O valor de eTag é modificado apenas quando as propriedades da pasta são alteradas, exceto para propriedades derivadas de descendentes (como **childCount** ou **lastModifiedDateTime**).

## <a name="relationships"></a>Relações

| Relação       | Tipo                        | Descrição
|:-------------------|:----------------------------|:--------------------------
| activities         | Conjunto [itemActivity][] | A lista de atividades recentes que ocorreram neste item.
| análise          | recurso [itemAnalytics][]  | Análise sobre as atividades de visualização que ocorreram neste item.
| children           | coleção driveItem        | Coleção que contêm objetos Item para os filhos imediatos do Item. Somente os itens que representam pastas têm filhos. Somente leitura. Anulável.
| createdByUser      | [user][]                    | A identidade do usuário que criou o item. Somente leitura.
| lastModifiedByUser | [user][]                    | A identidade do usuário que modificou o item pela última vez. Somente leitura.
| listItem           | [listItem][]                | Para unidades no SharePoint, o item da lista da biblioteca de documentos associado. Somente leitura. Anulável.
| permissões        | Coleção [permission][]   | O conjunto de permissões do item. Somente leitura. Anulável.
| assinaturas      | conjunto de [assinaturas][] | O conjunto de assinaturas no item. Compatível somente na raiz de uma unidade.
| miniaturas         | Coleção [thumbnailSet][] | Coleção contendo objetos [ThumbnailSet][] associados ao item. Para saber mais, confira [obtendo miniaturas][]. Somente leitura. Anulável.
| versões           | coleção [driveItemVersion][]  | A lista de todas as versões anteriores do item. Para saber mais, confira as informações sobre a [obtenção de versões anteriores][]. Somente leitura. Anulável.
| pasta de trabalho           | [pasta de trabalho][]                | Para arquivos que são planilhas do Excel, acessa a API de pasta da trabalho para trabalhar com o conteúdo da planilha. Anulável.

## <a name="instance-attributes"></a>Atributos de instância

Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.

| Nome da propriedade                     | Tipo   | Descrição
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.conflictBehavior | string | O comportamento de resolução de conflitos para ações que criam um novo item. Você pode usar os valores *fail*, *replace* ou *rename*. O padrão para PUT é *replace*. Um item nunca será retornado com essa anotação. Somente gravação.
| @microsoft.graph.downloadUrl      | string | Uma URL que pode ser usada para baixar conteúdo desse arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.
| @microsoft.graph.sourceUrl        | string | Quando uma solicitação PUT é emitida, essa anotação de instância pode ser usada para instruir o serviço a baixar o conteúdo da URL e armazená-lo como o arquivo. Somente gravação.

**Observação:** O valor de @microsoft.graph.downloadUrl é uma URL de curta duração e não pode ser armazenado em cache.
A URL só estará disponível por um curto período de tempo (1 hora) antes de ser invalidada.
A remoção das permissões de arquivo de um usuário pode não invalidar a URL imediatamente.

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
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": {"@odata.type": "microsoft.graph.itemAnalytics"},
  "children": [{ "@odata.type": "microsoft.graph.driveItem" }],
  "createdByUser": { "@odata.type": "microsoft.graph.user" },
  "lastModifiedByUser": { "@odata.type": "microsoft.graph.user" },
  "permissions": [ {"@odata.type": "microsoft.graph.permission"} ],
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],
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

## <a name="methods"></a>Métodos

| Método                                                   | Tipo de retorno | Descrição
|:---------------------------------------------------------|:------------|:------------
| [Obter item](../api/driveitem-get.md)                      | driveItem |Recupere os metadados de um DriveItem em uma unidade.
| [Obter análises][]                                        | [itemAnalytics][] | Obter análises para este recurso. 
| [Obter atividades por intervalo][]                           | [itemActivityStat][] | Obter uma coleção de itemActivityStats dentro do intervalo de tempo especificado.
| [Listar filhos](../api/driveitem-list-children.md)       | coleção de driveItem | Retornar uma coleção de DriveItems no relacionamento filho de um DriveItem.
| [Listar versões](../api/driveitem-list-versions.md)       | coleção de [DriveItemVersion][] | Recupera as versões de um arquivo na unidade do usuário atual.
| [Criar item](../api/driveitem-post-children.md)         | driveItem | Cria um driveItem na unidade especificada.
| [Atualizar item](../api/driveitem-update.md)                | driveItem | Atualiza um driveItem na unidade.
| [Carregar conteúdo](../api/driveitem-put-content.md)        | driveItem | Carrega conteúdo para o driveItem.
| [Baixar conteúdo](../api/driveitem-get-content.md)      | URL de download | Baixa o conteúdo de um driveItem.
| [Baixar formato de arquivo específico][download-format]         | URL de download | Baixa o conteúdo de um driveItem com um formato específico.
| [Excluir item](../api/driveitem-delete.md)                | Sem Conteúdo | Exclui um driveItem.
| [Mover item](../api/driveitem-move.md)                    | driveItem | Move um DriveItem para um novo item pai.
| [Copiar item](../api/driveitem-copy.md)                    | detalhes sobre como [monitorar o progresso](/graph/long-running-actions-overview) da cópia | Cria uma cópia de um driveItem (incluindo qualquer filho).
| [Pesquisar itens](../api/driveitem-search.md)               | coleção de driveItem | Pesquise a hierarquia de itens para itens que correspondam a uma consulta.
| [Listar alterações em uma unidade](../api/driveitem-delta.md)     | link delta | Listar quaisquer alterações na unidade.
| [Listar miniaturas](../api/driveitem-list-thumbnails.md)   | coleção de driveItem | Listar driveItems com suas miniaturas. 
| [Criar link de compartilhamento](../api/driveitem-createlink.md)    | link de compartilhamento | Criar um link para compartilhar o driveItem.
| [Adicionar permissões](../api/driveitem-invite.md)            | coleção de [permissão][] | Envia um convite de compartilhamento a um usuário.
| [Listar permissões](../api/driveitem-list-permissions.md) | coleção de [permissão][] | Recupera a coleção de permissões em um driveItem.
| [Excluir permissão](../api/permission-delete.md)         | Sem Conteúdo | Remove a permissão do driveItem.
| [Obter canal WebSocket][getWebSocket]                    | [assinatura][] | Recebe notificações de alteração quase em tempo real para uma unidade usando o socket.io.
| [Item de visualização][item-preview]                             | objeto json | Obtenha URLs incorporáveis de curta duração para um item de modo a renderizar uma visualização temporária.

[item-preview]: ../api/driveitem-preview.md
[Obter análises]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivitystat-getactivitybyinterval.md

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[obter versões anteriores]: ../api/driveitem-list-versions.md
[obtendo miniaturas]: ../api/driveitem-list-thumbnails.md
[getWebSocket]: ../api/driveitem-subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
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
[assinatura]: subscription.md
[thumbnailSet]: thumbnailset.md
[vídeo]: video.md
[pasta de trabalho]: workbook.md
[Usuário]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

[DriveItemVersion]: driveitemversion.md
[permissão]: permission.md
[assinatura]: subscription.md
[itemActivityStat]: itemactivitystat.md

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
