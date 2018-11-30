---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: DriveItem
ms.openlocfilehash: 1344d9a82459704354fc20a07c329949c4f5fc23
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039010"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="5e095-102">tipo de recurso de driveItem</span><span class="sxs-lookup"><span data-stu-id="5e095-102">driveItem resource type</span></span>

> <span data-ttu-id="5e095-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5e095-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e095-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5e095-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e095-p102">O recurso **DriveItem** representa um arquivo, pasta ou outro item armazenado em uma unidade. Todos os objetos do sistema de arquivos no OneDrive e no SharePoint são retornados como recursos **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="5e095-p102">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="5e095-107">Há duas maneiras principais de endereçar um recurso **driveItem**:</span><span class="sxs-lookup"><span data-stu-id="5e095-107">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="5e095-108">Pelo identificador exclusivo de **driveItem** usando `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="5e095-108">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="5e095-109">Usando o caminho do sistema de arquivos `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="5e095-109">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="5e095-p103">Os recursos **DriveItem** têm facetas modeladas como propriedades que fornecem dados sobre as identidades e capacidades de driveItem. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="5e095-p103">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="5e095-112">As pastas têm uma [**faceta folder**][folder]</span><span class="sxs-lookup"><span data-stu-id="5e095-112">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="5e095-113">Os arquivos têm uma [**faceta file**][file].</span><span class="sxs-lookup"><span data-stu-id="5e095-113">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="5e095-114">As imagens têm uma [**faceta image**][image], além de facetas file.</span><span class="sxs-lookup"><span data-stu-id="5e095-114">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="5e095-115">Imagens obtidas com uma câmera (fotos) têm uma [**faceta photo**][photo] que identifica o item como uma foto e fornece as propriedades de quando foi tirada e com qual dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e095-115">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="5e095-116">Itens com a faceta **folder** atuam como contêineres de itens e, portanto, têm uma referência `children` apontando para um conjunto de **driveItems** na pasta.</span><span class="sxs-lookup"><span data-stu-id="5e095-116">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e095-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e095-117">JSON representation</span></span>

<span data-ttu-id="5e095-118">Veja a seguir uma representação JSON de um recurso **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="5e095-118">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="5e095-119">O recurso **driveItem** é derivado de [**baseItem**][baseItem] e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="5e095-119">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5e095-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e095-120">Properties</span></span>

| <span data-ttu-id="5e095-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e095-121">Property</span></span>             | <span data-ttu-id="5e095-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e095-122">Type</span></span>               | <span data-ttu-id="5e095-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e095-123">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="5e095-124">audio</span><span class="sxs-lookup"><span data-stu-id="5e095-124">audio</span></span>                | <span data-ttu-id="5e095-125">[audio][]</span><span class="sxs-lookup"><span data-stu-id="5e095-125">[audio][]</span></span>          | <span data-ttu-id="5e095-p104">Metadados de áudio, se o item for um arquivo de áudio. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p104">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="5e095-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="5e095-128">createdBy</span></span>            | <span data-ttu-id="5e095-129">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5e095-129">[identitySet][]</span></span>    | <span data-ttu-id="5e095-p105">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p105">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="5e095-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e095-132">createdDateTime</span></span>      | <span data-ttu-id="5e095-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e095-133">DateTimeOffset</span></span>     | <span data-ttu-id="5e095-p106">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p106">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="5e095-136">cTag</span><span class="sxs-lookup"><span data-stu-id="5e095-136">cTag</span></span>                 | <span data-ttu-id="5e095-137">String</span><span class="sxs-lookup"><span data-stu-id="5e095-137">String</span></span>             | <span data-ttu-id="5e095-p107">Uma eTag para o conteúdo do item. Essa eTag não será alterada se apenas os metadados forem alterados. **Observação** Essa propriedade não será retornada se o item for uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p107">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="5e095-142">deleted</span><span class="sxs-lookup"><span data-stu-id="5e095-142">deleted</span></span>              | <span data-ttu-id="5e095-143">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="5e095-143">[deleted][]</span></span>        | <span data-ttu-id="5e095-p108">Informações sobre o estado excluído do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p108">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="5e095-146">description</span><span class="sxs-lookup"><span data-stu-id="5e095-146">description</span></span>          | <span data-ttu-id="5e095-147">String</span><span class="sxs-lookup"><span data-stu-id="5e095-147">String</span></span>             | <span data-ttu-id="5e095-p109">Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="5e095-p109">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="5e095-151">eTag</span><span class="sxs-lookup"><span data-stu-id="5e095-151">eTag</span></span>                 | <span data-ttu-id="5e095-152">String</span><span class="sxs-lookup"><span data-stu-id="5e095-152">String</span></span>             | <span data-ttu-id="5e095-p110">eTag para o item inteiro (metadados + conteúdo). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p110">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="5e095-155">file</span><span class="sxs-lookup"><span data-stu-id="5e095-155">file</span></span>                 | <span data-ttu-id="5e095-156">[file][]</span><span class="sxs-lookup"><span data-stu-id="5e095-156">[file][]</span></span>           | <span data-ttu-id="5e095-p111">Metadados de arquivo, se o item for um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p111">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="5e095-159">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="5e095-159">fileSystemInfo</span></span>       | <span data-ttu-id="5e095-160">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="5e095-160">[fileSystemInfo][]</span></span> | <span data-ttu-id="5e095-p112">Informações do sistema de arquivos no cliente. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="5e095-p112">File system information on client. Read-write.</span></span>
| <span data-ttu-id="5e095-163">folder</span><span class="sxs-lookup"><span data-stu-id="5e095-163">folder</span></span>               | <span data-ttu-id="5e095-164">[folder][]</span><span class="sxs-lookup"><span data-stu-id="5e095-164">[folder][]</span></span>         | <span data-ttu-id="5e095-p113">Metadados de pasta, se o item for uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p113">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="5e095-167">id</span><span class="sxs-lookup"><span data-stu-id="5e095-167">id</span></span>                   | <span data-ttu-id="5e095-168">String</span><span class="sxs-lookup"><span data-stu-id="5e095-168">String</span></span>             | <span data-ttu-id="5e095-p114">O identificador exclusivo do item na Unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p114">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="5e095-171">imagem</span><span class="sxs-lookup"><span data-stu-id="5e095-171">image</span></span>                | <span data-ttu-id="5e095-172">[image][]</span><span class="sxs-lookup"><span data-stu-id="5e095-172">[image][]</span></span>          | <span data-ttu-id="5e095-p115">Metadados de imagem, se o item for uma imagem. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p115">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="5e095-175">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5e095-175">lastModifiedBy</span></span>       | <span data-ttu-id="5e095-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5e095-176">[identitySet][]</span></span>    | <span data-ttu-id="5e095-p116">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p116">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="5e095-179">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e095-179">lastModifiedDateTime</span></span> | <span data-ttu-id="5e095-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e095-180">DateTimeOffset</span></span>     | <span data-ttu-id="5e095-p117">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p117">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="5e095-183">location</span><span class="sxs-lookup"><span data-stu-id="5e095-183">location</span></span>             | <span data-ttu-id="5e095-184">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="5e095-184">[geoCoordinates][]</span></span> | <span data-ttu-id="5e095-p118">Metadados de localização, se o item tiver dados de localização. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p118">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="5e095-187">name</span><span class="sxs-lookup"><span data-stu-id="5e095-187">name</span></span>                 | <span data-ttu-id="5e095-188">String</span><span class="sxs-lookup"><span data-stu-id="5e095-188">String</span></span>             | <span data-ttu-id="5e095-p119">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="5e095-p119">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="5e095-191">pacote</span><span class="sxs-lookup"><span data-stu-id="5e095-191">package</span></span>              | <span data-ttu-id="5e095-192">[package][]</span><span class="sxs-lookup"><span data-stu-id="5e095-192">[package][]</span></span>        | <span data-ttu-id="5e095-p120">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p120">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="5e095-196">parentReference</span><span class="sxs-lookup"><span data-stu-id="5e095-196">parentReference</span></span>      | <span data-ttu-id="5e095-197">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="5e095-197">[itemReference][]</span></span>  | <span data-ttu-id="5e095-p121">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="5e095-p121">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="5e095-200">Foto</span><span class="sxs-lookup"><span data-stu-id="5e095-200">photo</span></span>                | <span data-ttu-id="5e095-201">[photo][]</span><span class="sxs-lookup"><span data-stu-id="5e095-201">[photo][]</span></span>          | <span data-ttu-id="5e095-p122">Metadados de foto, se o item for uma foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p122">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="5e095-204">publication</span><span class="sxs-lookup"><span data-stu-id="5e095-204">publication</span></span>          | <span data-ttu-id="5e095-205">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="5e095-205">[publicationFacet][]</span></span> | <span data-ttu-id="5e095-206">Fornece informações sobre o estado de publicação ou de check-out de um item, nos locais que oferecem suporte a essas ações.</span><span class="sxs-lookup"><span data-stu-id="5e095-206">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="5e095-207">Esta propriedade não retorna por padrão.</span><span class="sxs-lookup"><span data-stu-id="5e095-207">This property is not returned by default.</span></span> <span data-ttu-id="5e095-208">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-208">Read-only.</span></span> |
| <span data-ttu-id="5e095-209">remoteItem</span><span class="sxs-lookup"><span data-stu-id="5e095-209">remoteItem</span></span>           | <span data-ttu-id="5e095-210">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="5e095-210">[remoteItem][]</span></span>     | <span data-ttu-id="5e095-p124">Dados do item remoto, se o item for compartilhado de uma unidade diferente daquela que está sendo acessada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p124">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="5e095-213">root</span><span class="sxs-lookup"><span data-stu-id="5e095-213">root</span></span>                 | <span data-ttu-id="5e095-214">[root][]</span><span class="sxs-lookup"><span data-stu-id="5e095-214">[root][]</span></span>           | <span data-ttu-id="5e095-215">Se essa propriedade for não nula, indicará que o driveItem é o principal driveItem na unidade.</span><span class="sxs-lookup"><span data-stu-id="5e095-215">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="5e095-216">searchResult</span><span class="sxs-lookup"><span data-stu-id="5e095-216">searchResult</span></span>         | <span data-ttu-id="5e095-217">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="5e095-217">[searchResult][]</span></span>   | <span data-ttu-id="5e095-p125">Metadados de pesquisa, se o item for de um resultado de pesquisa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p125">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="5e095-220">shared</span><span class="sxs-lookup"><span data-stu-id="5e095-220">shared</span></span>               | <span data-ttu-id="5e095-221">[shared][]</span><span class="sxs-lookup"><span data-stu-id="5e095-221">[shared][]</span></span>         | <span data-ttu-id="5e095-p126">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p126">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="5e095-224">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="5e095-224">sharepointIds</span></span>        | <span data-ttu-id="5e095-225">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="5e095-225">[sharepointIds][]</span></span>  | <span data-ttu-id="5e095-p127">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p127">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="5e095-228">size</span><span class="sxs-lookup"><span data-stu-id="5e095-228">size</span></span>                 | <span data-ttu-id="5e095-229">Int64</span><span class="sxs-lookup"><span data-stu-id="5e095-229">Int64</span></span>              | <span data-ttu-id="5e095-p128">O tamanho do item em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p128">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="5e095-232">specialFolder</span><span class="sxs-lookup"><span data-stu-id="5e095-232">specialFolder</span></span>        | <span data-ttu-id="5e095-233">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="5e095-233">[specialFolder][]</span></span>  | <span data-ttu-id="5e095-p129">Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p129">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="5e095-236">video</span><span class="sxs-lookup"><span data-stu-id="5e095-236">video</span></span>                | <span data-ttu-id="5e095-237">[video][]</span><span class="sxs-lookup"><span data-stu-id="5e095-237">[video][]</span></span>          | <span data-ttu-id="5e095-p130">Metadados de vídeo, se o item for um vídeo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p130">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="5e095-240">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="5e095-240">webDavUrl</span></span>            | <span data-ttu-id="5e095-241">String</span><span class="sxs-lookup"><span data-stu-id="5e095-241">String</span></span>             | <span data-ttu-id="5e095-242">URL compatível com WebDAV para o item.</span><span class="sxs-lookup"><span data-stu-id="5e095-242">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="5e095-243">webUrl</span><span class="sxs-lookup"><span data-stu-id="5e095-243">webUrl</span></span>               | <span data-ttu-id="5e095-244">String</span><span class="sxs-lookup"><span data-stu-id="5e095-244">String</span></span>             | <span data-ttu-id="5e095-p131">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p131">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="5e095-p132">**Observação:** As propriedades eTag e cTag funcionam de maneira diferente em contêineres (pastas). O valor de cTag é modificado quando o conteúdo ou os metadados de qualquer descendente da pasta são alterados. O valor de eTag é modificado apenas quando as propriedades da pasta são alteradas, exceto para propriedades derivadas de descendentes (como **childCount** ou **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="5e095-p132">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="5e095-250">Relações</span><span class="sxs-lookup"><span data-stu-id="5e095-250">Relationships</span></span>

| <span data-ttu-id="5e095-251">Relação</span><span class="sxs-lookup"><span data-stu-id="5e095-251">Relationship</span></span>       | <span data-ttu-id="5e095-252">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e095-252">Type</span></span>                            | <span data-ttu-id="5e095-253">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e095-253">Description</span></span>
|:-------------------|:--------------------------------|:--------------------------
| <span data-ttu-id="5e095-254">activities</span><span class="sxs-lookup"><span data-stu-id="5e095-254">activities</span></span>         | <span data-ttu-id="5e095-255">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="5e095-255">[itemActivity][] collection</span></span>     | <span data-ttu-id="5e095-256">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="5e095-256">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="5e095-257">análise</span><span class="sxs-lookup"><span data-stu-id="5e095-257">analytics</span></span>          | <span data-ttu-id="5e095-258">recurso de [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="5e095-258">[itemAnalytics][] resource</span></span>      | <span data-ttu-id="5e095-259">Análise sobre as atividades de modo de exibição que foram realizada neste item.</span><span class="sxs-lookup"><span data-stu-id="5e095-259">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="5e095-260">content</span><span class="sxs-lookup"><span data-stu-id="5e095-260">content</span></span>            | <span data-ttu-id="5e095-261">Fluxo</span><span class="sxs-lookup"><span data-stu-id="5e095-261">Stream</span></span>                          | <span data-ttu-id="5e095-262">O fluxo de conteúdo, se o item representar um arquivo.</span><span class="sxs-lookup"><span data-stu-id="5e095-262">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="5e095-263">children</span><span class="sxs-lookup"><span data-stu-id="5e095-263">children</span></span>           | <span data-ttu-id="5e095-264">Conjunto driveitem</span><span class="sxs-lookup"><span data-stu-id="5e095-264">driveitem collection</span></span>            | <span data-ttu-id="5e095-p133">Conjunto que contêm objetos Item para os filhos imediatos de Item. Somente os itens que representam pastas têm filhos. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5e095-p133">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="5e095-269">listItem</span><span class="sxs-lookup"><span data-stu-id="5e095-269">listItem</span></span>           | <span data-ttu-id="5e095-270">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="5e095-270">[listItem][]</span></span>                    | <span data-ttu-id="5e095-271">Para as unidades no SharePoint, o item de lista da biblioteca de documento associado.</span><span class="sxs-lookup"><span data-stu-id="5e095-271">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="5e095-272">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-272">Read-only.</span></span> <span data-ttu-id="5e095-273">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5e095-273">Nullable.</span></span>
| <span data-ttu-id="5e095-274">permissions</span><span class="sxs-lookup"><span data-stu-id="5e095-274">permissions</span></span>        | <span data-ttu-id="5e095-275">Coleção [permission][]</span><span class="sxs-lookup"><span data-stu-id="5e095-275">[permission][] collection</span></span>       | <span data-ttu-id="5e095-p135">O conjunto de permissões do item. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5e095-p135">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="5e095-279">miniaturas</span><span class="sxs-lookup"><span data-stu-id="5e095-279">thumbnails</span></span>         | <span data-ttu-id="5e095-280">Coleção [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="5e095-280">[thumbnailSet][] collection</span></span>     | <span data-ttu-id="5e095-p136">Coleção contendo objetos [ThumbnailSet][] associados ao item. Para saber mais, confira [obtendo miniaturas][]. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5e095-p136">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="5e095-285">versions</span><span class="sxs-lookup"><span data-stu-id="5e095-285">versions</span></span>           | <span data-ttu-id="5e095-286">coleção [driveItemVersion][]</span><span class="sxs-lookup"><span data-stu-id="5e095-286">[driveItemVersion][] collection</span></span> | <span data-ttu-id="5e095-287">Lista de versões anteriores do item.</span><span class="sxs-lookup"><span data-stu-id="5e095-287">The list of previous versions of the item.</span></span> <span data-ttu-id="5e095-288">Para obter mais informações, consulte a [obtenção de versões anteriores][].</span><span class="sxs-lookup"><span data-stu-id="5e095-288">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="5e095-289">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-289">Read-only.</span></span> <span data-ttu-id="5e095-290">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5e095-290">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="5e095-291">Atributos de instância</span><span class="sxs-lookup"><span data-stu-id="5e095-291">Instance Attributes</span></span>

<span data-ttu-id="5e095-p138">Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.</span><span class="sxs-lookup"><span data-stu-id="5e095-p138">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="5e095-294">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5e095-294">Property name</span></span>                     | <span data-ttu-id="5e095-295">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e095-295">Type</span></span>   | <span data-ttu-id="5e095-296">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e095-296">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="5e095-297">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="5e095-297">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="5e095-298">string</span><span class="sxs-lookup"><span data-stu-id="5e095-298">string</span></span> | <span data-ttu-id="5e095-p139">O comportamento de resolução de conflitos para ações que criam um novo item. Você pode usar os valores *fail*, *replace* ou *rename*. O padrão para PUT é *replace*. Um item nunca será retornado com essa anotação. Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="5e095-p139">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="5e095-304">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="5e095-304">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="5e095-305">string</span><span class="sxs-lookup"><span data-stu-id="5e095-305">string</span></span> | <span data-ttu-id="5e095-p140">Uma URL que pode ser usada para baixar conteúdo desse arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5e095-p140">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="5e095-309">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="5e095-309">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="5e095-310">string</span><span class="sxs-lookup"><span data-stu-id="5e095-310">string</span></span> | <span data-ttu-id="5e095-p141">Quando uma solicitação PUT é emitida, essa anotação de instância pode ser usada para instruir o serviço a baixar o conteúdo da URL e armazená-lo como o arquivo. Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="5e095-p141">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="5e095-313">**Observação:** O valor de @microsoft.graph.downloadUrl é uma URL de curta duração e não pode ser armazenados em cache.</span><span class="sxs-lookup"><span data-stu-id="5e095-313">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="5e095-314">A URL só estará disponível por um curto período de tempo (1 hora) antes de ele será invalidado.</span><span class="sxs-lookup"><span data-stu-id="5e095-314">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span> <span data-ttu-id="5e095-315">Remover permissões de arquivo para um usuário não pode invalidar a URL imediatamente.</span><span class="sxs-lookup"><span data-stu-id="5e095-315">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

## <a name="methods"></a><span data-ttu-id="5e095-316">Métodos</span><span class="sxs-lookup"><span data-stu-id="5e095-316">Methods</span></span>

| <span data-ttu-id="5e095-317">Método</span><span class="sxs-lookup"><span data-stu-id="5e095-317">Method</span></span>                                                   | <span data-ttu-id="5e095-318">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="5e095-318">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="5e095-319">Obter item</span><span class="sxs-lookup"><span data-stu-id="5e095-319">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="5e095-320">Listar atividades</span><span class="sxs-lookup"><span data-stu-id="5e095-320">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="5e095-321">[Obtenha a análise][]</span><span class="sxs-lookup"><span data-stu-id="5e095-321">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="5e095-322">[Fazer atividades pelo intervalo][]</span><span class="sxs-lookup"><span data-stu-id="5e095-322">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="5e095-323">Listar filhos</span><span class="sxs-lookup"><span data-stu-id="5e095-323">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="5e095-324">Listar versões</span><span class="sxs-lookup"><span data-stu-id="5e095-324">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="5e095-325">Criar item</span><span class="sxs-lookup"><span data-stu-id="5e095-325">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="5e095-326">Atualizar item</span><span class="sxs-lookup"><span data-stu-id="5e095-326">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="5e095-327">Carregar conteúdo</span><span class="sxs-lookup"><span data-stu-id="5e095-327">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="5e095-328">Baixar conteúdo</span><span class="sxs-lookup"><span data-stu-id="5e095-328">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="5e095-329">[Baixar formato de arquivo específico][download-format]</span><span class="sxs-lookup"><span data-stu-id="5e095-329">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="5e095-330">Excluir item</span><span class="sxs-lookup"><span data-stu-id="5e095-330">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="5e095-331">Mover item</span><span class="sxs-lookup"><span data-stu-id="5e095-331">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="5e095-332">Copiar item</span><span class="sxs-lookup"><span data-stu-id="5e095-332">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="5e095-333">Pesquisar itens</span><span class="sxs-lookup"><span data-stu-id="5e095-333">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="5e095-334">Listar alterações em uma unidade</span><span class="sxs-lookup"><span data-stu-id="5e095-334">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="5e095-335">Listar miniaturas</span><span class="sxs-lookup"><span data-stu-id="5e095-335">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="5e095-336">Criar um link de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="5e095-336">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="5e095-337">Adicionar permissões</span><span class="sxs-lookup"><span data-stu-id="5e095-337">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="5e095-338">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="5e095-338">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="5e095-339">Excluir permissão</span><span class="sxs-lookup"><span data-stu-id="5e095-339">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="5e095-340">[Obtenha o canal WebSocket][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="5e095-340">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="5e095-341">[Item de visualização][item-preview]</span><span class="sxs-lookup"><span data-stu-id="5e095-341">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`

[item-preview]: ../api/driveitem-preview.md
[Obtenha a análise]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Fazer atividades pelo intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="5e095-344">Comentários</span><span class="sxs-lookup"><span data-stu-id="5e095-344">Remarks</span></span>

<span data-ttu-id="5e095-345">Em bibliotecas de documentos do OneDrive for Business ou do SharePoint, a propriedade **cTag** não será retornada se **driveItem** for uma faceta [folder][].</span><span class="sxs-lookup"><span data-stu-id="5e095-345">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

[audio]: audio.md
[baseItem]: baseitem.md
[deleted]: deleted.md
[download-format]: ../api/driveitem-get-content-format.md
[driveItemVersion]: driveitemversion.md
[file]: file.md
[fileSystemInfo]: filesysteminfo.md
[folder]: folder.md
[obtenção de versões anteriores]: ../api/driveitem-list-versions.md
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
