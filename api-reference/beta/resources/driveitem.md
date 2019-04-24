---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7ac95379d8e5eeae07e520f40ae9403c47e98f58
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507578"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="3ce07-102">tipo de recurso driveItem</span><span class="sxs-lookup"><span data-stu-id="3ce07-102">driveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ce07-p101">O recurso **DriveItem** representa um arquivo, pasta ou outro item armazenado em uma unidade. Todos os objetos do sistema de arquivos no OneDrive e no SharePoint são retornados como recursos **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="3ce07-105">Há duas maneiras principais de endereçar um recurso **driveItem**:</span><span class="sxs-lookup"><span data-stu-id="3ce07-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="3ce07-106">Pelo identificador exclusivo de **driveItem** usando `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="3ce07-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="3ce07-107">Usando o caminho do sistema de arquivos `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="3ce07-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="3ce07-p102">Os recursos **DriveItem** têm facetas modeladas como propriedades que fornecem dados sobre as identidades e capacidades de driveItem. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="3ce07-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="3ce07-110">As pastas têm uma [**faceta folder**][folder]</span><span class="sxs-lookup"><span data-stu-id="3ce07-110">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="3ce07-111">Os arquivos têm uma [**faceta file**][file].</span><span class="sxs-lookup"><span data-stu-id="3ce07-111">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="3ce07-112">As imagens têm uma [**faceta image**][image], além de facetas file.</span><span class="sxs-lookup"><span data-stu-id="3ce07-112">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="3ce07-113">Imagens obtidas com uma câmera (fotos) têm uma [**faceta photo**][photo] que identifica o item como uma foto e fornece as propriedades de quando foi tirada e com qual dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3ce07-113">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="3ce07-114">Itens com a faceta **folder** atuam como contêineres de itens e, portanto, têm uma referência `children` apontando para um conjunto de **driveItems** na pasta.</span><span class="sxs-lookup"><span data-stu-id="3ce07-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ce07-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ce07-115">JSON representation</span></span>

<span data-ttu-id="3ce07-116">Veja a seguir uma representação JSON de um recurso **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="3ce07-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="3ce07-117">O recurso **driveItem** é derivado de [**baseItem**][baseItem] e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="3ce07-117">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3ce07-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ce07-118">Properties</span></span>

| <span data-ttu-id="3ce07-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ce07-119">Property</span></span>             | <span data-ttu-id="3ce07-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ce07-120">Type</span></span>               | <span data-ttu-id="3ce07-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ce07-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="3ce07-122">audio</span><span class="sxs-lookup"><span data-stu-id="3ce07-122">audio</span></span>                | <span data-ttu-id="3ce07-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-123">[audio][]</span></span>          | <span data-ttu-id="3ce07-p103">Metadados de áudio, se o item for um arquivo de áudio. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="3ce07-126">conteúdo</span><span class="sxs-lookup"><span data-stu-id="3ce07-126">content</span></span>              | <span data-ttu-id="3ce07-127">Fluxo</span><span class="sxs-lookup"><span data-stu-id="3ce07-127">Stream</span></span>             | <span data-ttu-id="3ce07-128">O fluxo de conteúdo, se o item representar um arquivo.</span><span class="sxs-lookup"><span data-stu-id="3ce07-128">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="3ce07-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="3ce07-129">createdBy</span></span>            | <span data-ttu-id="3ce07-130">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-130">[identitySet][]</span></span>    | <span data-ttu-id="3ce07-p104">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="3ce07-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce07-133">createdDateTime</span></span>      | <span data-ttu-id="3ce07-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce07-134">DateTimeOffset</span></span>     | <span data-ttu-id="3ce07-p105">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="3ce07-137">cTag</span><span class="sxs-lookup"><span data-stu-id="3ce07-137">cTag</span></span>                 | <span data-ttu-id="3ce07-138">String</span><span class="sxs-lookup"><span data-stu-id="3ce07-138">String</span></span>             | <span data-ttu-id="3ce07-p106">Uma eTag para o conteúdo do item. Essa eTag não será alterada se apenas os metadados forem alterados. **Observação** Essa propriedade não será retornada se o item for uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="3ce07-143">deleted</span><span class="sxs-lookup"><span data-stu-id="3ce07-143">deleted</span></span>              | <span data-ttu-id="3ce07-144">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-144">[deleted][]</span></span>        | <span data-ttu-id="3ce07-p107">Informações sobre o estado excluído do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="3ce07-147">descrição</span><span class="sxs-lookup"><span data-stu-id="3ce07-147">description</span></span>          | <span data-ttu-id="3ce07-148">String</span><span class="sxs-lookup"><span data-stu-id="3ce07-148">String</span></span>             | <span data-ttu-id="3ce07-p108">Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="3ce07-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="3ce07-152">eTag</span><span class="sxs-lookup"><span data-stu-id="3ce07-152">eTag</span></span>                 | <span data-ttu-id="3ce07-153">String</span><span class="sxs-lookup"><span data-stu-id="3ce07-153">String</span></span>             | <span data-ttu-id="3ce07-p109">eTag para o item inteiro (metadados + conteúdo). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="3ce07-156">file</span><span class="sxs-lookup"><span data-stu-id="3ce07-156">file</span></span>                 | <span data-ttu-id="3ce07-157">[file][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-157">[file][]</span></span>           | <span data-ttu-id="3ce07-p110">Metadados de arquivo, se o item for um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="3ce07-160">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="3ce07-160">fileSystemInfo</span></span>       | <span data-ttu-id="3ce07-161">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-161">[fileSystemInfo][]</span></span> | <span data-ttu-id="3ce07-p111">Informações do sistema de arquivos no cliente. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="3ce07-164">folder</span><span class="sxs-lookup"><span data-stu-id="3ce07-164">folder</span></span>               | <span data-ttu-id="3ce07-165">[folder][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-165">[folder][]</span></span>         | <span data-ttu-id="3ce07-p112">Metadados de pasta, se o item for uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="3ce07-168">id</span><span class="sxs-lookup"><span data-stu-id="3ce07-168">id</span></span>                   | <span data-ttu-id="3ce07-169">String</span><span class="sxs-lookup"><span data-stu-id="3ce07-169">String</span></span>             | <span data-ttu-id="3ce07-p113">O identificador exclusivo do item na Unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="3ce07-172">imagem</span><span class="sxs-lookup"><span data-stu-id="3ce07-172">image</span></span>                | <span data-ttu-id="3ce07-173">[image][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-173">[image][]</span></span>          | <span data-ttu-id="3ce07-p114">Metadados de imagem, se o item for uma imagem. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="3ce07-176">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3ce07-176">lastModifiedBy</span></span>       | <span data-ttu-id="3ce07-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-177">[identitySet][]</span></span>    | <span data-ttu-id="3ce07-p115">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="3ce07-180">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce07-180">lastModifiedDateTime</span></span> | <span data-ttu-id="3ce07-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce07-181">DateTimeOffset</span></span>     | <span data-ttu-id="3ce07-p116">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="3ce07-184">location</span><span class="sxs-lookup"><span data-stu-id="3ce07-184">location</span></span>             | <span data-ttu-id="3ce07-185">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-185">[geoCoordinates][]</span></span> | <span data-ttu-id="3ce07-p117">Metadados de localização, se o item tiver dados de localização. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="3ce07-188">nome</span><span class="sxs-lookup"><span data-stu-id="3ce07-188">name</span></span>                 | <span data-ttu-id="3ce07-189">String</span><span class="sxs-lookup"><span data-stu-id="3ce07-189">String</span></span>             | <span data-ttu-id="3ce07-p118">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="3ce07-192">pacote</span><span class="sxs-lookup"><span data-stu-id="3ce07-192">package</span></span>              | <span data-ttu-id="3ce07-193">[package][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-193">[package][]</span></span>        | <span data-ttu-id="3ce07-p119">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="3ce07-197">parentReference</span><span class="sxs-lookup"><span data-stu-id="3ce07-197">parentReference</span></span>      | <span data-ttu-id="3ce07-198">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-198">[itemReference][]</span></span>  | <span data-ttu-id="3ce07-p120">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="3ce07-201">Foto</span><span class="sxs-lookup"><span data-stu-id="3ce07-201">photo</span></span>                | <span data-ttu-id="3ce07-202">[photo][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-202">[photo][]</span></span>          | <span data-ttu-id="3ce07-p121">Metadados de foto, se o item for uma foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="3ce07-205">publication</span><span class="sxs-lookup"><span data-stu-id="3ce07-205">publication</span></span>          | <span data-ttu-id="3ce07-206">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-206">[publicationFacet][]</span></span> | <span data-ttu-id="3ce07-207">Fornece informações sobre o estado de publicação ou de check-out de um item, nos locais que oferecem suporte a essas ações.</span><span class="sxs-lookup"><span data-stu-id="3ce07-207">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="3ce07-208">Esta propriedade não retorna por padrão.</span><span class="sxs-lookup"><span data-stu-id="3ce07-208">This property is not returned by default.</span></span> <span data-ttu-id="3ce07-209">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-209">Read-only.</span></span> |
| <span data-ttu-id="3ce07-210">remoteItem</span><span class="sxs-lookup"><span data-stu-id="3ce07-210">remoteItem</span></span>           | <span data-ttu-id="3ce07-211">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-211">[remoteItem][]</span></span>     | <span data-ttu-id="3ce07-p123">Dados do item remoto, se o item for compartilhado de uma unidade diferente daquela que está sendo acessada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p123">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="3ce07-214">root</span><span class="sxs-lookup"><span data-stu-id="3ce07-214">root</span></span>                 | <span data-ttu-id="3ce07-215">[root][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-215">[root][]</span></span>           | <span data-ttu-id="3ce07-216">Se essa propriedade for não nula, indicará que o driveItem é o principal driveItem na unidade.</span><span class="sxs-lookup"><span data-stu-id="3ce07-216">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="3ce07-217">searchResult</span><span class="sxs-lookup"><span data-stu-id="3ce07-217">searchResult</span></span>         | <span data-ttu-id="3ce07-218">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-218">[searchResult][]</span></span>   | <span data-ttu-id="3ce07-p124">Metadados de pesquisa, se o item for de um resultado de pesquisa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p124">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="3ce07-221">compartilhado</span><span class="sxs-lookup"><span data-stu-id="3ce07-221">shared</span></span>               | <span data-ttu-id="3ce07-222">[compartilhado][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-222">[shared][]</span></span>         | <span data-ttu-id="3ce07-p125">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p125">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="3ce07-225">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="3ce07-225">sharepointIds</span></span>        | <span data-ttu-id="3ce07-226">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-226">[sharepointIds][]</span></span>  | <span data-ttu-id="3ce07-p126">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p126">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="3ce07-229">size</span><span class="sxs-lookup"><span data-stu-id="3ce07-229">size</span></span>                 | <span data-ttu-id="3ce07-230">Int64</span><span class="sxs-lookup"><span data-stu-id="3ce07-230">Int64</span></span>              | <span data-ttu-id="3ce07-p127">O tamanho do item em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p127">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="3ce07-233">specialFolder</span><span class="sxs-lookup"><span data-stu-id="3ce07-233">specialFolder</span></span>        | <span data-ttu-id="3ce07-234">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-234">[specialFolder][]</span></span>  | <span data-ttu-id="3ce07-p128">Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p128">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="3ce07-237">video</span><span class="sxs-lookup"><span data-stu-id="3ce07-237">video</span></span>                | <span data-ttu-id="3ce07-238">[video][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-238">[video][]</span></span>          | <span data-ttu-id="3ce07-p129">Metadados de vídeo, se o item for um vídeo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p129">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="3ce07-241">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="3ce07-241">webDavUrl</span></span>            | <span data-ttu-id="3ce07-242">String</span><span class="sxs-lookup"><span data-stu-id="3ce07-242">String</span></span>             | <span data-ttu-id="3ce07-243">URL compatível com WebDAV para o item.</span><span class="sxs-lookup"><span data-stu-id="3ce07-243">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="3ce07-244">webUrl</span><span class="sxs-lookup"><span data-stu-id="3ce07-244">webUrl</span></span>               | <span data-ttu-id="3ce07-245">String</span><span class="sxs-lookup"><span data-stu-id="3ce07-245">String</span></span>             | <span data-ttu-id="3ce07-p130">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p130">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="3ce07-p131">**Observação:** As propriedades eTag e cTag funcionam de maneira diferente em contêineres (pastas). O valor de cTag é modificado quando o conteúdo ou os metadados de qualquer descendente da pasta são alterados. O valor de eTag é modificado apenas quando as propriedades da pasta são alteradas, exceto para propriedades derivadas de descendentes (como **childCount** ou **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="3ce07-p131">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="3ce07-251">Relações</span><span class="sxs-lookup"><span data-stu-id="3ce07-251">Relationships</span></span>

| <span data-ttu-id="3ce07-252">Relação</span><span class="sxs-lookup"><span data-stu-id="3ce07-252">Relationship</span></span>       | <span data-ttu-id="3ce07-253">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ce07-253">Type</span></span>                        | <span data-ttu-id="3ce07-254">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ce07-254">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="3ce07-255">activities</span><span class="sxs-lookup"><span data-stu-id="3ce07-255">activities</span></span>         | <span data-ttu-id="3ce07-256">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-256">[itemActivity][] collection</span></span> | <span data-ttu-id="3ce07-257">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="3ce07-257">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="3ce07-258">analytics</span><span class="sxs-lookup"><span data-stu-id="3ce07-258">analytics</span></span>          | <span data-ttu-id="3ce07-259">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="3ce07-259">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="3ce07-260">Análise sobre as atividades de exibição que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="3ce07-260">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="3ce07-261">filhos</span><span class="sxs-lookup"><span data-stu-id="3ce07-261">children</span></span>           | <span data-ttu-id="3ce07-262">coleção driveItem</span><span class="sxs-lookup"><span data-stu-id="3ce07-262">driveItem collection</span></span>        | <span data-ttu-id="3ce07-p132">Coleção que contêm objetos Item para os filhos imediatos do Item. Somente os itens que representam pastas têm filhos. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p132">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="3ce07-267">createdByUser</span><span class="sxs-lookup"><span data-stu-id="3ce07-267">createdByUser</span></span>      | <span data-ttu-id="3ce07-268">[user][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-268">[user][]</span></span>                    | <span data-ttu-id="3ce07-269">A identidade do usuário que criou o item.</span><span class="sxs-lookup"><span data-stu-id="3ce07-269">Identity of the user who created the item.</span></span> <span data-ttu-id="3ce07-270">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-270">Read-only.</span></span>
| <span data-ttu-id="3ce07-271">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="3ce07-271">lastModifiedByUser</span></span> | <span data-ttu-id="3ce07-272">[user][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-272">[user][]</span></span>                    | <span data-ttu-id="3ce07-273">A identidade do usuário que modificou o item pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3ce07-273">Identity of the user who last modified the item.</span></span> <span data-ttu-id="3ce07-274">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-274">Read-only.</span></span>
| <span data-ttu-id="3ce07-275">listItem</span><span class="sxs-lookup"><span data-stu-id="3ce07-275">listItem</span></span>           | <span data-ttu-id="3ce07-276">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-276">[listItem][]</span></span>                | <span data-ttu-id="3ce07-277">Para unidades no SharePoint, o item da lista da biblioteca de documentos associado.</span><span class="sxs-lookup"><span data-stu-id="3ce07-277">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="3ce07-278">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-278">Read-only.</span></span> <span data-ttu-id="3ce07-279">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3ce07-279">Nullable.</span></span>
| <span data-ttu-id="3ce07-280">permissões</span><span class="sxs-lookup"><span data-stu-id="3ce07-280">permissions</span></span>        | <span data-ttu-id="3ce07-281">Coleção [permission][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-281">[permission][] collection</span></span>   | <span data-ttu-id="3ce07-p136">O conjunto de permissões do item. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p136">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="3ce07-285">assinaturas</span><span class="sxs-lookup"><span data-stu-id="3ce07-285">subscriptions</span></span>      | <span data-ttu-id="3ce07-286">conjunto de [assinaturas][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-286">[subscription][] collection</span></span> | <span data-ttu-id="3ce07-287">O conjunto de assinaturas no item.</span><span class="sxs-lookup"><span data-stu-id="3ce07-287">The set of subscriptions on the item.</span></span> <span data-ttu-id="3ce07-288">Compatível somente na raiz de uma unidade.</span><span class="sxs-lookup"><span data-stu-id="3ce07-288">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="3ce07-289">miniaturas</span><span class="sxs-lookup"><span data-stu-id="3ce07-289">thumbnails</span></span>         | <span data-ttu-id="3ce07-290">Coleção [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-290">[thumbnailSet][] collection</span></span> | <span data-ttu-id="3ce07-p138">Coleção contendo objetos [ThumbnailSet][] associados ao item. Para saber mais, confira [obtendo miniaturas][]. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p138">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="3ce07-295">versões</span><span class="sxs-lookup"><span data-stu-id="3ce07-295">versions</span></span>           | <span data-ttu-id="3ce07-296">coleção [driveItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="3ce07-296">[driveItemVersion][] collection</span></span> | <span data-ttu-id="3ce07-297">A lista de todas as versões anteriores do item.</span><span class="sxs-lookup"><span data-stu-id="3ce07-297">The list of previous versions of the item.</span></span> <span data-ttu-id="3ce07-298">Para saber mais, confira as informações sobre a [obtenção de versões anteriores][].</span><span class="sxs-lookup"><span data-stu-id="3ce07-298">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="3ce07-299">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-299">Read-only.</span></span> <span data-ttu-id="3ce07-300">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3ce07-300">Nullable.</span></span>
| <span data-ttu-id="3ce07-301">pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="3ce07-301">workbook</span></span>           | <span data-ttu-id="3ce07-302">[pasta de trabalho][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-302">[workbook][]</span></span>                | <span data-ttu-id="3ce07-303">Para arquivos que são planilhas do Excel, acessa a API de pasta da trabalho para trabalhar com o conteúdo da planilha.</span><span class="sxs-lookup"><span data-stu-id="3ce07-303">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="3ce07-304">Anulável.</span><span class="sxs-lookup"><span data-stu-id="3ce07-304">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="3ce07-305">Atributos de instância</span><span class="sxs-lookup"><span data-stu-id="3ce07-305">Instance Attributes</span></span>

<span data-ttu-id="3ce07-p141">Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p141">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="3ce07-308">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3ce07-308">Property name</span></span>                     | <span data-ttu-id="3ce07-309">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ce07-309">Type</span></span>   | <span data-ttu-id="3ce07-310">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ce07-310">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="3ce07-311">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="3ce07-311">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="3ce07-312">string</span><span class="sxs-lookup"><span data-stu-id="3ce07-312">string</span></span> | <span data-ttu-id="3ce07-p142">O comportamento de resolução de conflitos para ações que criam um novo item. Você pode usar os valores *fail*, *replace* ou *rename*. O padrão para PUT é *replace*. Um item nunca será retornado com essa anotação. Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p142">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="3ce07-318">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="3ce07-318">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="3ce07-319">string</span><span class="sxs-lookup"><span data-stu-id="3ce07-319">string</span></span> | <span data-ttu-id="3ce07-p143">Uma URL que pode ser usada para baixar conteúdo desse arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p143">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="3ce07-323">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="3ce07-323">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="3ce07-324">string</span><span class="sxs-lookup"><span data-stu-id="3ce07-324">string</span></span> | <span data-ttu-id="3ce07-p144">Quando uma solicitação PUT é emitida, essa anotação de instância pode ser usada para instruir o serviço a baixar o conteúdo da URL e armazená-lo como o arquivo. Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="3ce07-p144">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="3ce07-327">**Observação:** O valor de @microsoft.graph.downloadUrl é uma URL de curta duração e não pode ser armazenado em cache.</span><span class="sxs-lookup"><span data-stu-id="3ce07-327">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="3ce07-328">A URL só estará disponível por um curto período de tempo (1 hora) antes de ser invalidada.</span><span class="sxs-lookup"><span data-stu-id="3ce07-328">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="3ce07-329">A remoção das permissões de arquivo de um usuário pode não invalidar a URL imediatamente.</span><span class="sxs-lookup"><span data-stu-id="3ce07-329">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="3ce07-330">Métodos</span><span class="sxs-lookup"><span data-stu-id="3ce07-330">Methods</span></span>

| <span data-ttu-id="3ce07-331">Método</span><span class="sxs-lookup"><span data-stu-id="3ce07-331">Method</span></span>                                                   | <span data-ttu-id="3ce07-332">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="3ce07-332">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="3ce07-333">Obter item</span><span class="sxs-lookup"><span data-stu-id="3ce07-333">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="3ce07-334">Listar atividades</span><span class="sxs-lookup"><span data-stu-id="3ce07-334">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="3ce07-335">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-335">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="3ce07-336">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="3ce07-336">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="3ce07-337">Listar filhos</span><span class="sxs-lookup"><span data-stu-id="3ce07-337">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="3ce07-338">Listar versões</span><span class="sxs-lookup"><span data-stu-id="3ce07-338">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="3ce07-339">Criar item</span><span class="sxs-lookup"><span data-stu-id="3ce07-339">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="3ce07-340">Atualizar item</span><span class="sxs-lookup"><span data-stu-id="3ce07-340">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="3ce07-341">Carregar conteúdo</span><span class="sxs-lookup"><span data-stu-id="3ce07-341">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="3ce07-342">Baixar conteúdo</span><span class="sxs-lookup"><span data-stu-id="3ce07-342">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="3ce07-343">[Baixar formato de arquivo específico][download-format]</span><span class="sxs-lookup"><span data-stu-id="3ce07-343">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="3ce07-344">Excluir item</span><span class="sxs-lookup"><span data-stu-id="3ce07-344">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="3ce07-345">Mover item</span><span class="sxs-lookup"><span data-stu-id="3ce07-345">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="3ce07-346">Copiar item</span><span class="sxs-lookup"><span data-stu-id="3ce07-346">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="3ce07-347">Pesquisar itens</span><span class="sxs-lookup"><span data-stu-id="3ce07-347">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="3ce07-348">Listar alterações em uma unidade</span><span class="sxs-lookup"><span data-stu-id="3ce07-348">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="3ce07-349">Listar miniaturas</span><span class="sxs-lookup"><span data-stu-id="3ce07-349">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="3ce07-350">Criar link de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="3ce07-350">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="3ce07-351">Adicionar permissões</span><span class="sxs-lookup"><span data-stu-id="3ce07-351">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="3ce07-352">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="3ce07-352">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="3ce07-353">Excluir permissão</span><span class="sxs-lookup"><span data-stu-id="3ce07-353">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="3ce07-354">[Obter canal WebSocket][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="3ce07-354">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="3ce07-355">[Item de visualização][item-preview]</span><span class="sxs-lookup"><span data-stu-id="3ce07-355">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="3ce07-358">Comentários</span><span class="sxs-lookup"><span data-stu-id="3ce07-358">Remarks</span></span>

<span data-ttu-id="3ce07-359">Em bibliotecas de documentos do OneDrive for Business ou do SharePoint, a propriedade **cTag** não será retornada se **driveItem** for uma faceta [folder][].</span><span class="sxs-lookup"><span data-stu-id="3ce07-359">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[obter versões anteriores]: ../api/driveitem-list-versions.md
[getting previous versions]: ../api/driveitem-list-versions.md
[obtendo miniaturas]: ../api/driveitem-list-thumbnails.md
[getting thumbnails]: ../api/driveitem-list-thumbnails.md
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
[shared]: shared.md
[sharepointIds]: sharepointids.md
[specialFolder]: specialfolder.md
[assinatura]: subscription.md
[subscription]: subscription.md
[thumbnailSet]: thumbnailset.md
[vídeo]: video.md
[video]: video.md
[pasta de trabalho]: workbook.md
[workbook]: workbook.md
[Usuário]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[user]: https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/users
[publicationFacet]: publicationfacet.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": {
    "Resources/Item": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/driveitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
