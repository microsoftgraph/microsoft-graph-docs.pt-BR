---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 526001ad9a6c52c5b031c1734466772861f1c67e
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="e82a1-102">Tipo de recurso DriveItem</span><span class="sxs-lookup"><span data-stu-id="e82a1-102">DriveItem resource type</span></span>

<span data-ttu-id="e82a1-p101">O recurso **DriveItem** representa um arquivo, pasta ou outro item armazenado em uma unidade. Todos os objetos do sistema de arquivos no OneDrive e no SharePoint são retornados como recursos **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="e82a1-105">Há duas maneiras principais de endereçar um recurso **driveItem**:</span><span class="sxs-lookup"><span data-stu-id="e82a1-105">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="e82a1-106">Pelo identificador exclusivo de **driveItem** usando `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="e82a1-106">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="e82a1-107">Usando o caminho do sistema de arquivos `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="e82a1-107">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="e82a1-p102">Os recursos **DriveItem** têm facetas modeladas como propriedades que fornecem dados sobre as identidades e capacidades de driveItem. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e82a1-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="e82a1-110">As pastas têm uma [**faceta folder**][folder]</span><span class="sxs-lookup"><span data-stu-id="e82a1-110">Folders have a [**folder facet**]</span></span>
* <span data-ttu-id="e82a1-111">Os arquivos têm uma [**faceta file**][file].</span><span class="sxs-lookup"><span data-stu-id="e82a1-111">Files have a [**file facet**].</span></span>
* <span data-ttu-id="e82a1-112">As imagens têm uma [**faceta image**][image], além de facetas file.</span><span class="sxs-lookup"><span data-stu-id="e82a1-112">Images have an [**image facet**] in addition to their file facet.</span></span>
* <span data-ttu-id="e82a1-113">Imagens obtidas com uma câmera (fotos) têm uma [**faceta photo**][photo] que identifica o item como uma foto e fornece as propriedades de quando foi tirada e com qual dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e82a1-113">Images taken with a camera (photos) have a [**photo facet**] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="e82a1-114">Itens com a faceta **folder** atuam como contêineres de itens e, portanto, têm uma referência `children` apontando para um conjunto de **driveItems** na pasta.</span><span class="sxs-lookup"><span data-stu-id="e82a1-114">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e82a1-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e82a1-115">JSON representation</span></span>

<span data-ttu-id="e82a1-116">Veja a seguir uma representação JSON de um recurso **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="e82a1-116">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="e82a1-117">O recurso **driveItem** é derivado de [**baseItem**][baseItem] e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="e82a1-117">The **driveItem** resource is derived from [**baseItem**] and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.driveItem", "@type.aka": "oneDrive.item",
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

## <a name="properties"></a><span data-ttu-id="e82a1-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e82a1-118">Properties</span></span>

| <span data-ttu-id="e82a1-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e82a1-119">Property</span></span>             | <span data-ttu-id="e82a1-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e82a1-120">Type</span></span>               | <span data-ttu-id="e82a1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e82a1-121">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="e82a1-122">audio</span><span class="sxs-lookup"><span data-stu-id="e82a1-122">audio</span></span>                | <span data-ttu-id="e82a1-123">[audio][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-123">[audio][]</span></span>          | <span data-ttu-id="e82a1-p103">Metadados de áudio, se o item for um arquivo de áudio. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="e82a1-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="e82a1-126">createdBy</span></span>            | <span data-ttu-id="e82a1-127">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-127">[identitySet][]</span></span>    | <span data-ttu-id="e82a1-p104">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="e82a1-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e82a1-130">createdDateTime</span></span>      | <span data-ttu-id="e82a1-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e82a1-131">DateTimeOffset</span></span>     | <span data-ttu-id="e82a1-p105">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="e82a1-134">cTag</span><span class="sxs-lookup"><span data-stu-id="e82a1-134">cTag</span></span>                 | <span data-ttu-id="e82a1-135">String</span><span class="sxs-lookup"><span data-stu-id="e82a1-135">String</span></span>             | <span data-ttu-id="e82a1-p106">Uma eTag para o conteúdo do item. Essa eTag não será alterada se apenas os metadados forem alterados. **Observação** Essa propriedade não será retornada se o item for uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="e82a1-140">deleted</span><span class="sxs-lookup"><span data-stu-id="e82a1-140">deleted</span></span>              | <span data-ttu-id="e82a1-141">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-141">[deleted][]</span></span>        | <span data-ttu-id="e82a1-p107">Informações sobre o estado excluído do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="e82a1-144">descrição</span><span class="sxs-lookup"><span data-stu-id="e82a1-144">description</span></span>          | <span data-ttu-id="e82a1-145">String</span><span class="sxs-lookup"><span data-stu-id="e82a1-145">String</span></span>             | <span data-ttu-id="e82a1-p108">Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="e82a1-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="e82a1-149">eTag</span><span class="sxs-lookup"><span data-stu-id="e82a1-149">eTag</span></span>                 | <span data-ttu-id="e82a1-150">String</span><span class="sxs-lookup"><span data-stu-id="e82a1-150">String</span></span>             | <span data-ttu-id="e82a1-p109">eTag para o item inteiro (metadados + conteúdo). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="e82a1-153">file</span><span class="sxs-lookup"><span data-stu-id="e82a1-153">file</span></span>                 | <span data-ttu-id="e82a1-154">[file][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-154">[file][]</span></span>           | <span data-ttu-id="e82a1-p110">Metadados de arquivo, se o item for um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="e82a1-157">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="e82a1-157">fileSystemInfo</span></span>       | <span data-ttu-id="e82a1-158">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-158">[fileSystemInfo][]</span></span> | <span data-ttu-id="e82a1-p111">Informações do sistema de arquivos no cliente. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="e82a1-161">folder</span><span class="sxs-lookup"><span data-stu-id="e82a1-161">folder</span></span>               | <span data-ttu-id="e82a1-162">[folder][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-162">[folder][]</span></span>         | <span data-ttu-id="e82a1-p112">Metadados de pasta, se o item for uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="e82a1-165">id</span><span class="sxs-lookup"><span data-stu-id="e82a1-165">id</span></span>                   | <span data-ttu-id="e82a1-166">String</span><span class="sxs-lookup"><span data-stu-id="e82a1-166">String</span></span>             | <span data-ttu-id="e82a1-p113">O identificador exclusivo do item na Unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="e82a1-169">image</span><span class="sxs-lookup"><span data-stu-id="e82a1-169">image</span></span>                | <span data-ttu-id="e82a1-170">[image][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-170">[image][]</span></span>          | <span data-ttu-id="e82a1-p114">Metadados de imagem, se o item for uma imagem. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="e82a1-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="e82a1-173">lastModifiedBy</span></span>       | <span data-ttu-id="e82a1-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-174">[identitySet][]</span></span>    | <span data-ttu-id="e82a1-p115">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="e82a1-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e82a1-177">lastModifiedDateTime</span></span> | <span data-ttu-id="e82a1-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e82a1-178">DateTimeOffset</span></span>     | <span data-ttu-id="e82a1-p116">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e82a1-181">location</span><span class="sxs-lookup"><span data-stu-id="e82a1-181">location</span></span>             | <span data-ttu-id="e82a1-182">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-182">[geoCoordinates][]</span></span> | <span data-ttu-id="e82a1-p117">Metadados de localização, se o item tiver dados de localização. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="e82a1-185">nome</span><span class="sxs-lookup"><span data-stu-id="e82a1-185">name</span></span>                 | <span data-ttu-id="e82a1-186">String</span><span class="sxs-lookup"><span data-stu-id="e82a1-186">String</span></span>             | <span data-ttu-id="e82a1-p118">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="e82a1-189">pacote</span><span class="sxs-lookup"><span data-stu-id="e82a1-189">package</span></span>              | <span data-ttu-id="e82a1-190">[package][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-190">[package][]</span></span>        | <span data-ttu-id="e82a1-p119">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="e82a1-194">parentReference</span><span class="sxs-lookup"><span data-stu-id="e82a1-194">parentReference</span></span>      | <span data-ttu-id="e82a1-195">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-195">[itemReference][]</span></span>  | <span data-ttu-id="e82a1-p120">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="e82a1-198">Foto</span><span class="sxs-lookup"><span data-stu-id="e82a1-198">photo</span></span>                | <span data-ttu-id="e82a1-199">[photo][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-199">[photo][]</span></span>          | <span data-ttu-id="e82a1-p121">Metadados de foto, se o item for uma foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p121">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="e82a1-202">remoteItem</span><span class="sxs-lookup"><span data-stu-id="e82a1-202">remoteItem</span></span>           | <span data-ttu-id="e82a1-203">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-203">[remoteItem][]</span></span>     | <span data-ttu-id="e82a1-p122">Dados do item remoto, se o item for compartilhado de uma unidade diferente daquela que está sendo acessada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p122">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="e82a1-206">root</span><span class="sxs-lookup"><span data-stu-id="e82a1-206">root</span></span>                 | <span data-ttu-id="e82a1-207">[root][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-207">[root][]</span></span>           | <span data-ttu-id="e82a1-208">Se essa propriedade for não nula, indicará que o driveItem é o principal driveItem na unidade.</span><span class="sxs-lookup"><span data-stu-id="e82a1-208">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="e82a1-209">searchResult</span><span class="sxs-lookup"><span data-stu-id="e82a1-209">searchResult</span></span>         | <span data-ttu-id="e82a1-210">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-210">[searchResult][]</span></span>   | <span data-ttu-id="e82a1-p123">Metadados de pesquisa, se o item for de um resultado de pesquisa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p123">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="e82a1-213">compartilhado</span><span class="sxs-lookup"><span data-stu-id="e82a1-213">shared</span></span>               | <span data-ttu-id="e82a1-214">[shared][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-214">[shared][]</span></span>         | <span data-ttu-id="e82a1-p124">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p124">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="e82a1-217">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="e82a1-217">sharepointIds</span></span>        | <span data-ttu-id="e82a1-218">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-218">[sharepointIds][]</span></span>  | <span data-ttu-id="e82a1-p125">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p125">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="e82a1-221">size</span><span class="sxs-lookup"><span data-stu-id="e82a1-221">size</span></span>                 | <span data-ttu-id="e82a1-222">Int64</span><span class="sxs-lookup"><span data-stu-id="e82a1-222">Int64</span></span>              | <span data-ttu-id="e82a1-p126">O tamanho do item em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p126">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="e82a1-225">specialFolder</span><span class="sxs-lookup"><span data-stu-id="e82a1-225">specialFolder</span></span>        | <span data-ttu-id="e82a1-226">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-226">[specialFolder][]</span></span>  | <span data-ttu-id="e82a1-p127">Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p127">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="e82a1-229">video</span><span class="sxs-lookup"><span data-stu-id="e82a1-229">video</span></span>                | <span data-ttu-id="e82a1-230">[video][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-230">[video][]</span></span>          | <span data-ttu-id="e82a1-p128">Metadados de vídeo, se o item for um vídeo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p128">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="e82a1-233">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="e82a1-233">webDavUrl</span></span>            | <span data-ttu-id="e82a1-234">String</span><span class="sxs-lookup"><span data-stu-id="e82a1-234">String</span></span>             | <span data-ttu-id="e82a1-235">URL compatível com WebDAV para o item.</span><span class="sxs-lookup"><span data-stu-id="e82a1-235">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="e82a1-236">webUrl</span><span class="sxs-lookup"><span data-stu-id="e82a1-236">webUrl</span></span>               | <span data-ttu-id="e82a1-237">String</span><span class="sxs-lookup"><span data-stu-id="e82a1-237">String</span></span>             | <span data-ttu-id="e82a1-p129">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p129">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="e82a1-p130">**Observação:** As propriedades eTag e cTag funcionam de maneira diferente em contêineres (pastas). O valor de cTag é modificado quando o conteúdo ou os metadados de qualquer descendente da pasta são alterados. O valor de eTag é modificado apenas quando as propriedades da pasta são alteradas, exceto para propriedades derivadas de descendentes (como **childCount** ou **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="e82a1-p130">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="e82a1-243">Relações</span><span class="sxs-lookup"><span data-stu-id="e82a1-243">Relationships</span></span>

| <span data-ttu-id="e82a1-244">Relação</span><span class="sxs-lookup"><span data-stu-id="e82a1-244">Relationship</span></span>       | <span data-ttu-id="e82a1-245">Tipo</span><span class="sxs-lookup"><span data-stu-id="e82a1-245">Type</span></span>                        | <span data-ttu-id="e82a1-246">Descrição</span><span class="sxs-lookup"><span data-stu-id="e82a1-246">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="e82a1-247">content</span><span class="sxs-lookup"><span data-stu-id="e82a1-247">content</span></span>            | <span data-ttu-id="e82a1-248">Fluxo</span><span class="sxs-lookup"><span data-stu-id="e82a1-248">Stream</span></span>                      | <span data-ttu-id="e82a1-249">O fluxo de conteúdo, se o item representar um arquivo.</span><span class="sxs-lookup"><span data-stu-id="e82a1-249">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="e82a1-250">children</span><span class="sxs-lookup"><span data-stu-id="e82a1-250">children</span></span>           | <span data-ttu-id="e82a1-251">Conjunto driveitem</span><span class="sxs-lookup"><span data-stu-id="e82a1-251">driveitem collection</span></span>        | <span data-ttu-id="e82a1-p131">Coleção que contêm objetos Item para os filhos imediatos do Item. Somente os itens que representam pastas têm filhos. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p131">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="e82a1-256">createdByUser</span><span class="sxs-lookup"><span data-stu-id="e82a1-256">createdByUser</span></span>      | <span data-ttu-id="e82a1-257">[user][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-257">[user][]</span></span>                    | <span data-ttu-id="e82a1-258">A identidade do usuário que criou o item.</span><span class="sxs-lookup"><span data-stu-id="e82a1-258">Identity of the user, device, or application which created the item. Read-only.</span></span> <span data-ttu-id="e82a1-259">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-259">Read-only.</span></span>
| <span data-ttu-id="e82a1-260">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="e82a1-260">lastModifiedByUser</span></span> | <span data-ttu-id="e82a1-261">[user][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-261">[user][]</span></span>                    | <span data-ttu-id="e82a1-262">A identidade do usuário que modificou o item pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e82a1-262">Identity of the user, device, and application which last modified the item. Read-only.</span></span> <span data-ttu-id="e82a1-263">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-263">Read-only.</span></span>
| <span data-ttu-id="e82a1-264">permissions</span><span class="sxs-lookup"><span data-stu-id="e82a1-264">permissions</span></span>        | <span data-ttu-id="e82a1-265">Coleção [permission][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-265">[permission][] collection</span></span>   | <span data-ttu-id="e82a1-p134">O conjunto de permissões do item. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p134">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="e82a1-269">miniaturas</span><span class="sxs-lookup"><span data-stu-id="e82a1-269">thumbnails</span></span>         | <span data-ttu-id="e82a1-270">Coleção [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="e82a1-270">[thumbnailSet][] collection</span></span> | <span data-ttu-id="e82a1-p135">Coleção contendo objetos [ThumbnailSet][] associados ao item. Para saber mais, confira [obtendo miniaturas][]. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p135">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="e82a1-275">Atributos de instância</span><span class="sxs-lookup"><span data-stu-id="e82a1-275">Instance Attributes</span></span>

<span data-ttu-id="e82a1-p136">Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p136">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="e82a1-278">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e82a1-278">Property name</span></span>                     | <span data-ttu-id="e82a1-279">Tipo</span><span class="sxs-lookup"><span data-stu-id="e82a1-279">Type</span></span>   | <span data-ttu-id="e82a1-280">Descrição</span><span class="sxs-lookup"><span data-stu-id="e82a1-280">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="e82a1-281">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="e82a1-281">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="e82a1-282">string</span><span class="sxs-lookup"><span data-stu-id="e82a1-282">string</span></span> | <span data-ttu-id="e82a1-p137">O comportamento de resolução de conflitos para ações que criam um novo item. Você pode usar os valores *fail*, *replace* ou *rename*. O padrão para PUT é *replace*. Um item nunca será retornado com essa anotação. Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p137">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="e82a1-288">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="e82a1-288">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="e82a1-289">string</span><span class="sxs-lookup"><span data-stu-id="e82a1-289">string</span></span> | <span data-ttu-id="e82a1-p138">Uma URL que pode ser usada para baixar conteúdo desse arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p138">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="e82a1-293">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="e82a1-293">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="e82a1-294">string</span><span class="sxs-lookup"><span data-stu-id="e82a1-294">string</span></span> | <span data-ttu-id="e82a1-p139">Quando uma solicitação PUT é emitida, essa anotação de instância pode ser usada para instruir o serviço a baixar o conteúdo da URL e armazená-lo como o arquivo. Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p139">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="e82a1-p140">**Observação:** O valor de @microsoft.graph.downloadUrl é uma URL de curta duração e não pode ser armazenado em cache. A URL só estará disponível por um curto período de tempo (1 hora) antes de ser invalidada.</span><span class="sxs-lookup"><span data-stu-id="e82a1-p140">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached. The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>

## <a name="methods"></a><span data-ttu-id="e82a1-299">Métodos</span><span class="sxs-lookup"><span data-stu-id="e82a1-299">Methods</span></span>

| <span data-ttu-id="e82a1-300">Método</span><span class="sxs-lookup"><span data-stu-id="e82a1-300">Method</span></span>                                                   | <span data-ttu-id="e82a1-301">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="e82a1-301">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="e82a1-302">Obter item</span><span class="sxs-lookup"><span data-stu-id="e82a1-302">Get item</span></span>](../api/driveitem_get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="e82a1-303">Listar filhos</span><span class="sxs-lookup"><span data-stu-id="e82a1-303">List children</span></span>](../api/driveitem_list_children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="e82a1-304">Criar item</span><span class="sxs-lookup"><span data-stu-id="e82a1-304">Create item</span></span>](../api/driveitem_post_children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="e82a1-305">Atualizar item</span><span class="sxs-lookup"><span data-stu-id="e82a1-305">Update item</span></span>](../api/driveitem_update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="e82a1-306">Carregar conteúdo</span><span class="sxs-lookup"><span data-stu-id="e82a1-306">Upload content</span></span>](../api/driveitem_put_content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="e82a1-307">Baixar conteúdo</span><span class="sxs-lookup"><span data-stu-id="e82a1-307">Download content</span></span>](../api/driveitem_get_content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="e82a1-308">[Baixar formato de arquivo específico][download-format]</span><span class="sxs-lookup"><span data-stu-id="e82a1-308">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="e82a1-309">Excluir item</span><span class="sxs-lookup"><span data-stu-id="e82a1-309">Delete item</span></span>](../api/driveitem_delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="e82a1-310">Mover item</span><span class="sxs-lookup"><span data-stu-id="e82a1-310">Move item</span></span>](../api/driveitem_move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="e82a1-311">Copiar item</span><span class="sxs-lookup"><span data-stu-id="e82a1-311">Copy item</span></span>](../api/driveitem_copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="e82a1-312">Pesquisar itens</span><span class="sxs-lookup"><span data-stu-id="e82a1-312">Search items</span></span>](../api/driveitem_search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="e82a1-313">Listar alterações em uma unidade</span><span class="sxs-lookup"><span data-stu-id="e82a1-313">List changes in a drive</span></span>](../api/driveitem_delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="e82a1-314">Listar miniaturas</span><span class="sxs-lookup"><span data-stu-id="e82a1-314">List thumbnails</span></span>](../api/driveitem_list_thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="e82a1-315">Criar link de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="e82a1-315">Create sharing link</span></span>](../api/driveitem_createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="e82a1-316">Adicionar permissões</span><span class="sxs-lookup"><span data-stu-id="e82a1-316">Add permissions</span></span>](../api/driveitem_invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="e82a1-317">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="e82a1-317">List permissions</span></span>](../api/driveitem_list_permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="e82a1-318">Excluir permissão</span><span class="sxs-lookup"><span data-stu-id="e82a1-318">Delete permission</span></span>](../api/permission_delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`


## <a name="remarks"></a><span data-ttu-id="e82a1-319">Comentários</span><span class="sxs-lookup"><span data-stu-id="e82a1-319">Remarks</span></span>

<span data-ttu-id="e82a1-320">Em bibliotecas de documentos do OneDrive for Business ou do SharePoint, a propriedade **cTag** não será retornada se **driveItem** for uma faceta [folder][].</span><span class="sxs-lookup"><span data-stu-id="e82a1-320">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseItem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem_get_content_format.md
[file]: file.md
[fileSystemInfo]: fileSystemInfo.md
[folder]: folder.md
[getting thumbnails]: ../api/driveitem_list_thumbnails.md
[identitySet]: identitySet.md
[image]: image.md
[itemReference]: itemReference.md
[geoCoordinates]: geoCoordinates.md
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
[user]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/users

<!-- {
  "type": "#page.annotation",
  "description": "Item is the main data model in the OneDrive API. Everything is an item.",
  "keywords": "item,facet,resource",
  "section": "documentation",
  "tocPath": "Items",
  "tocBookmarks": { "Resources/Item": "#" }
} -->
