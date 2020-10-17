---
author: JeremyKelley
description: O recurso DriveItem representa um arquivo, pasta ou outro item armazenado em uma unidade.
ms.date: 09/10/2017
title: DriveItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 32ddc9de6b4eb9422d79f347367aec9816d84c64
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582314"
---
# <a name="driveitem-resource-type"></a><span data-ttu-id="df223-103">tipo de recurso driveItem</span><span class="sxs-lookup"><span data-stu-id="df223-103">driveItem resource type</span></span>

<span data-ttu-id="df223-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df223-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df223-p101">O recurso **DriveItem** representa um arquivo, pasta ou outro item armazenado em uma unidade. Todos os objetos do sistema de arquivos no OneDrive e no SharePoint são retornados como recursos **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="df223-p101">The **driveItem** resource represents a file, folder, or other item stored in a drive. All file system objects in OneDrive and SharePoint are returned as **driveItem** resources.</span></span>

<span data-ttu-id="df223-107">Há duas maneiras principais de endereçar um recurso **driveItem**:</span><span class="sxs-lookup"><span data-stu-id="df223-107">There are two primary ways of addressing a **driveItem** resource:</span></span>

* <span data-ttu-id="df223-108">Pelo identificador exclusivo de **driveItem** usando `drive/items/{item-id}`</span><span class="sxs-lookup"><span data-stu-id="df223-108">By the **driveItem** unique identifier using `drive/items/{item-id}`</span></span>
* <span data-ttu-id="df223-109">Usando o caminho do sistema de arquivos `/drive/root:/path/to/file`</span><span class="sxs-lookup"><span data-stu-id="df223-109">By file system path using `/drive/root:/path/to/file`</span></span>

<span data-ttu-id="df223-p102">Os recursos **DriveItem** têm facetas modeladas como propriedades que fornecem dados sobre as identidades e capacidades de driveItem. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="df223-p102">**DriveItem** resources have facets modeled as properties that provide data about the driveItem's identities and capabilities. For example:</span></span>

* <span data-ttu-id="df223-112">As pastas têm uma [**faceta folder**][folder]</span><span class="sxs-lookup"><span data-stu-id="df223-112">Folders have a [**folder facet**][folder]</span></span>
* <span data-ttu-id="df223-113">Os arquivos têm uma [**faceta file**][file].</span><span class="sxs-lookup"><span data-stu-id="df223-113">Files have a [**file facet**][file].</span></span>
* <span data-ttu-id="df223-114">As imagens têm uma [**faceta image**][image], além de facetas file.</span><span class="sxs-lookup"><span data-stu-id="df223-114">Images have an [**image facet**][image] in addition to their file facet.</span></span>
* <span data-ttu-id="df223-115">Imagens obtidas com uma câmera (fotos) têm uma [**faceta photo**][photo] que identifica o item como uma foto e fornece as propriedades de quando foi tirada e com qual dispositivo.</span><span class="sxs-lookup"><span data-stu-id="df223-115">Images taken with a camera (photos) have a [**photo facet**][photo] that identifies the item as a photo and provides the properties of when the photo was taken and with what device.</span></span>

<span data-ttu-id="df223-116">Itens com a faceta **folder** atuam como contêineres de itens e, portanto, têm uma referência `children` apontando para um conjunto de **driveItems** na pasta.</span><span class="sxs-lookup"><span data-stu-id="df223-116">Items with the **folder** facet act as containers of items and therefore have a `children` reference pointing to a collection of **driveItems** under the folder.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df223-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df223-117">JSON representation</span></span>

<span data-ttu-id="df223-118">Veja a seguir uma representação JSON de um recurso **driveItem**.</span><span class="sxs-lookup"><span data-stu-id="df223-118">Here is a JSON representation of a **driveItem** resource.</span></span>

<span data-ttu-id="df223-119">O recurso **driveItem** é derivado de [**baseItem**][baseItem] e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="df223-119">The **driveItem** resource is derived from [**baseItem**][baseItem] and inherits properties from that resource.</span></span>

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
  "pendingOperations": { "@odata.type": "microsoft.graph.pendingOperations" },
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

## <a name="properties"></a><span data-ttu-id="df223-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df223-120">Properties</span></span>

| <span data-ttu-id="df223-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df223-121">Property</span></span>             | <span data-ttu-id="df223-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="df223-122">Type</span></span>               | <span data-ttu-id="df223-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="df223-123">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="df223-124">audio</span><span class="sxs-lookup"><span data-stu-id="df223-124">audio</span></span>                | <span data-ttu-id="df223-125">[audio][]</span><span class="sxs-lookup"><span data-stu-id="df223-125">[audio][]</span></span>          | <span data-ttu-id="df223-p103">Metadados de áudio, se o item for um arquivo de áudio. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p103">Audio metadata, if the item is an audio file. Read-only.</span></span>
| <span data-ttu-id="df223-128">conteúdo</span><span class="sxs-lookup"><span data-stu-id="df223-128">content</span></span>              | <span data-ttu-id="df223-129">Fluxo</span><span class="sxs-lookup"><span data-stu-id="df223-129">Stream</span></span>             | <span data-ttu-id="df223-130">O fluxo de conteúdo, se o item representar um arquivo.</span><span class="sxs-lookup"><span data-stu-id="df223-130">The content stream, if the item represents a file.</span></span>
| <span data-ttu-id="df223-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="df223-131">createdBy</span></span>            | <span data-ttu-id="df223-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="df223-132">[identitySet][]</span></span>    | <span data-ttu-id="df223-p104">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p104">Identity of the user, device, and application which created the item. Read-only.</span></span>
| <span data-ttu-id="df223-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df223-135">createdDateTime</span></span>      | <span data-ttu-id="df223-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df223-136">DateTimeOffset</span></span>     | <span data-ttu-id="df223-p105">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p105">Date and time of item creation. Read-only.</span></span>
| <span data-ttu-id="df223-139">cTag</span><span class="sxs-lookup"><span data-stu-id="df223-139">cTag</span></span>                 | <span data-ttu-id="df223-140">String</span><span class="sxs-lookup"><span data-stu-id="df223-140">String</span></span>             | <span data-ttu-id="df223-p106">Uma eTag para o conteúdo do item. Essa eTag não será alterada se apenas os metadados forem alterados. **Observação** Essa propriedade não será retornada se o item for uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p106">An eTag for the content of the item. This eTag is not changed if only the metadata is changed. **Note** This property is not returned if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="df223-145">deleted</span><span class="sxs-lookup"><span data-stu-id="df223-145">deleted</span></span>              | <span data-ttu-id="df223-146">[deleted][]</span><span class="sxs-lookup"><span data-stu-id="df223-146">[deleted][]</span></span>        | <span data-ttu-id="df223-p107">Informações sobre o estado excluído do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p107">Information about the deleted state of the item. Read-only.</span></span>
| <span data-ttu-id="df223-149">descrição</span><span class="sxs-lookup"><span data-stu-id="df223-149">description</span></span>          | <span data-ttu-id="df223-150">String</span><span class="sxs-lookup"><span data-stu-id="df223-150">String</span></span>             | <span data-ttu-id="df223-p108">Fornece uma descrição do item visível para o usuário. Leitura e gravação. Somente no OneDrive Personal</span><span class="sxs-lookup"><span data-stu-id="df223-p108">Provides a user-visible description of the item. Read-write. Only on OneDrive Personal</span></span>
| <span data-ttu-id="df223-154">eTag</span><span class="sxs-lookup"><span data-stu-id="df223-154">eTag</span></span>                 | <span data-ttu-id="df223-155">String</span><span class="sxs-lookup"><span data-stu-id="df223-155">String</span></span>             | <span data-ttu-id="df223-p109">eTag para o item inteiro (metadados + conteúdo). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p109">eTag for the entire item (metadata + content). Read-only.</span></span>
| <span data-ttu-id="df223-158">file</span><span class="sxs-lookup"><span data-stu-id="df223-158">file</span></span>                 | <span data-ttu-id="df223-159">[file][]</span><span class="sxs-lookup"><span data-stu-id="df223-159">[file][]</span></span>           | <span data-ttu-id="df223-p110">Metadados de arquivo, se o item for um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p110">File metadata, if the item is a file. Read-only.</span></span>
| <span data-ttu-id="df223-162">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="df223-162">fileSystemInfo</span></span>       | <span data-ttu-id="df223-163">[fileSystemInfo][]</span><span class="sxs-lookup"><span data-stu-id="df223-163">[fileSystemInfo][]</span></span> | <span data-ttu-id="df223-p111">Informações do sistema de arquivos no cliente. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="df223-p111">File system information on client. Read-write.</span></span>
| <span data-ttu-id="df223-166">folder</span><span class="sxs-lookup"><span data-stu-id="df223-166">folder</span></span>               | <span data-ttu-id="df223-167">[folder][]</span><span class="sxs-lookup"><span data-stu-id="df223-167">[folder][]</span></span>         | <span data-ttu-id="df223-p112">Metadados de pasta, se o item for uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p112">Folder metadata, if the item is a folder. Read-only.</span></span>
| <span data-ttu-id="df223-170">id</span><span class="sxs-lookup"><span data-stu-id="df223-170">id</span></span>                   | <span data-ttu-id="df223-171">String</span><span class="sxs-lookup"><span data-stu-id="df223-171">String</span></span>             | <span data-ttu-id="df223-p113">O identificador exclusivo do item na Unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p113">The unique identifier of the item within the Drive. Read-only.</span></span>
| <span data-ttu-id="df223-174">imagem</span><span class="sxs-lookup"><span data-stu-id="df223-174">image</span></span>                | <span data-ttu-id="df223-175">[image][]</span><span class="sxs-lookup"><span data-stu-id="df223-175">[image][]</span></span>          | <span data-ttu-id="df223-p114">Metadados de imagem, se o item for uma imagem. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p114">Image metadata, if the item is an image. Read-only.</span></span>
| <span data-ttu-id="df223-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="df223-178">lastModifiedBy</span></span>       | <span data-ttu-id="df223-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="df223-179">[identitySet][]</span></span>    | <span data-ttu-id="df223-p115">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p115">Identity of the user, device, and application which last modified the item. Read-only.</span></span>
| <span data-ttu-id="df223-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df223-182">lastModifiedDateTime</span></span> | <span data-ttu-id="df223-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df223-183">DateTimeOffset</span></span>     | <span data-ttu-id="df223-p116">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p116">Date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="df223-186">location</span><span class="sxs-lookup"><span data-stu-id="df223-186">location</span></span>             | <span data-ttu-id="df223-187">[geoCoordinates][]</span><span class="sxs-lookup"><span data-stu-id="df223-187">[geoCoordinates][]</span></span> | <span data-ttu-id="df223-p117">Metadados de localização, se o item tiver dados de localização. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p117">Location metadata, if the item has location data. Read-only.</span></span>
| <span data-ttu-id="df223-190">nome</span><span class="sxs-lookup"><span data-stu-id="df223-190">name</span></span>                 | <span data-ttu-id="df223-191">String</span><span class="sxs-lookup"><span data-stu-id="df223-191">String</span></span>             | <span data-ttu-id="df223-p118">O nome do item (nome do arquivo e extensão). Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="df223-p118">The name of the item (filename and extension). Read-write.</span></span>
| <span data-ttu-id="df223-194">pacote</span><span class="sxs-lookup"><span data-stu-id="df223-194">package</span></span>              | <span data-ttu-id="df223-195">[package][]</span><span class="sxs-lookup"><span data-stu-id="df223-195">[package][]</span></span>        | <span data-ttu-id="df223-p119">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p119">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span>
| <span data-ttu-id="df223-199">parentReference</span><span class="sxs-lookup"><span data-stu-id="df223-199">parentReference</span></span>      | <span data-ttu-id="df223-200">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="df223-200">[itemReference][]</span></span>  | <span data-ttu-id="df223-p120">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="df223-p120">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="df223-203">pendingOperations</span><span class="sxs-lookup"><span data-stu-id="df223-203">pendingOperations</span></span>    | <span data-ttu-id="df223-204">[pendingOperations][]</span><span class="sxs-lookup"><span data-stu-id="df223-204">[pendingOperations][]</span></span> | <span data-ttu-id="df223-205">Se presente, indica que uma ou mais operações que podem afetar o estado de driveItem estão aguardando conclusão.</span><span class="sxs-lookup"><span data-stu-id="df223-205">If present, indicates that indicates that one or more operations that may affect the state of the driveItem are pending completion.</span></span> <span data-ttu-id="df223-206">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-206">Read-only.</span></span>
| <span data-ttu-id="df223-207">photo</span><span class="sxs-lookup"><span data-stu-id="df223-207">photo</span></span>                | <span data-ttu-id="df223-208">[photo][]</span><span class="sxs-lookup"><span data-stu-id="df223-208">[photo][]</span></span>          | <span data-ttu-id="df223-p122">Metadados de foto, se o item for uma foto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p122">Photo metadata, if the item is a photo. Read-only.</span></span>
| <span data-ttu-id="df223-211">publication</span><span class="sxs-lookup"><span data-stu-id="df223-211">publication</span></span>          | <span data-ttu-id="df223-212">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="df223-212">[publicationFacet][]</span></span> | <span data-ttu-id="df223-213">Fornece informações sobre o estado de publicação ou de check-out de um item, nos locais que oferecem suporte a essas ações.</span><span class="sxs-lookup"><span data-stu-id="df223-213">Provides information about the published or checked-out state of an item, in locations that support such actions.</span></span> <span data-ttu-id="df223-214">Esta propriedade não retorna por padrão.</span><span class="sxs-lookup"><span data-stu-id="df223-214">This property is not returned by default.</span></span> <span data-ttu-id="df223-215">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-215">Read-only.</span></span> |
| <span data-ttu-id="df223-216">remoteItem</span><span class="sxs-lookup"><span data-stu-id="df223-216">remoteItem</span></span>           | <span data-ttu-id="df223-217">[remoteItem][]</span><span class="sxs-lookup"><span data-stu-id="df223-217">[remoteItem][]</span></span>     | <span data-ttu-id="df223-p124">Dados do item remoto, se o item for compartilhado de uma unidade diferente daquela que está sendo acessada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p124">Remote item data, if the item is shared from a drive other than the one being accessed. Read-only.</span></span>
| <span data-ttu-id="df223-220">root</span><span class="sxs-lookup"><span data-stu-id="df223-220">root</span></span>                 | <span data-ttu-id="df223-221">[root][]</span><span class="sxs-lookup"><span data-stu-id="df223-221">[root][]</span></span>           | <span data-ttu-id="df223-222">Se essa propriedade for não nula, indicará que o driveItem é o principal driveItem na unidade.</span><span class="sxs-lookup"><span data-stu-id="df223-222">If this property is non-null, it indicates that the driveItem is the top-most driveItem in the drive.</span></span>
| <span data-ttu-id="df223-223">searchResult</span><span class="sxs-lookup"><span data-stu-id="df223-223">searchResult</span></span>         | <span data-ttu-id="df223-224">[searchResult][]</span><span class="sxs-lookup"><span data-stu-id="df223-224">[searchResult][]</span></span>   | <span data-ttu-id="df223-p125">Metadados de pesquisa, se o item for de um resultado de pesquisa. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p125">Search metadata, if the item is from a search result. Read-only.</span></span>
| <span data-ttu-id="df223-227">compartilhado</span><span class="sxs-lookup"><span data-stu-id="df223-227">shared</span></span>               | <span data-ttu-id="df223-228">[compartilhado][]</span><span class="sxs-lookup"><span data-stu-id="df223-228">[shared][]</span></span>         | <span data-ttu-id="df223-p126">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p126">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>
| <span data-ttu-id="df223-231">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="df223-231">sharepointIds</span></span>        | <span data-ttu-id="df223-232">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="df223-232">[sharepointIds][]</span></span>  | <span data-ttu-id="df223-p127">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p127">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="df223-235">size</span><span class="sxs-lookup"><span data-stu-id="df223-235">size</span></span>                 | <span data-ttu-id="df223-236">Int64</span><span class="sxs-lookup"><span data-stu-id="df223-236">Int64</span></span>              | <span data-ttu-id="df223-p128">O tamanho do item em bytes. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p128">Size of the item in bytes. Read-only.</span></span>
| <span data-ttu-id="df223-239">specialFolder</span><span class="sxs-lookup"><span data-stu-id="df223-239">specialFolder</span></span>        | <span data-ttu-id="df223-240">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="df223-240">[specialFolder][]</span></span>  | <span data-ttu-id="df223-p129">Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p129">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>
| <span data-ttu-id="df223-243">video</span><span class="sxs-lookup"><span data-stu-id="df223-243">video</span></span>                | <span data-ttu-id="df223-244">[video][]</span><span class="sxs-lookup"><span data-stu-id="df223-244">[video][]</span></span>          | <span data-ttu-id="df223-p130">Metadados de vídeo, se o item for um vídeo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p130">Video metadata, if the item is a video. Read-only.</span></span>
| <span data-ttu-id="df223-247">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="df223-247">webDavUrl</span></span>            | <span data-ttu-id="df223-248">String</span><span class="sxs-lookup"><span data-stu-id="df223-248">String</span></span>             | <span data-ttu-id="df223-249">URL compatível com WebDAV para o item.</span><span class="sxs-lookup"><span data-stu-id="df223-249">WebDAV compatible URL for the item.</span></span>
| <span data-ttu-id="df223-250">webUrl</span><span class="sxs-lookup"><span data-stu-id="df223-250">webUrl</span></span>               | <span data-ttu-id="df223-251">String</span><span class="sxs-lookup"><span data-stu-id="df223-251">String</span></span>             | <span data-ttu-id="df223-p131">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p131">URL that displays the resource in the browser. Read-only.</span></span>

<span data-ttu-id="df223-p132">**Observação:** As propriedades eTag e cTag funcionam de maneira diferente em contêineres (pastas). O valor de cTag é modificado quando o conteúdo ou os metadados de qualquer descendente da pasta são alterados. O valor de eTag é modificado apenas quando as propriedades da pasta são alteradas, exceto para propriedades derivadas de descendentes (como **childCount** ou **lastModifiedDateTime**).</span><span class="sxs-lookup"><span data-stu-id="df223-p132">**Note:** The eTag and cTag properties work differently on containers (folders). The cTag value is modified when content or metadata of any descendant of the folder is changed. The eTag value is only modified when the folder's properties are changed, except for properties that are derived from descendants (like **childCount** or **lastModifiedDateTime**).</span></span>

## <a name="relationships"></a><span data-ttu-id="df223-257">Relações</span><span class="sxs-lookup"><span data-stu-id="df223-257">Relationships</span></span>

| <span data-ttu-id="df223-258">Relação</span><span class="sxs-lookup"><span data-stu-id="df223-258">Relationship</span></span>       | <span data-ttu-id="df223-259">Tipo</span><span class="sxs-lookup"><span data-stu-id="df223-259">Type</span></span>                        | <span data-ttu-id="df223-260">Descrição</span><span class="sxs-lookup"><span data-stu-id="df223-260">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="df223-261">activities</span><span class="sxs-lookup"><span data-stu-id="df223-261">activities</span></span>         | <span data-ttu-id="df223-262">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="df223-262">[itemActivity][] collection</span></span> | <span data-ttu-id="df223-263">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="df223-263">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="df223-264">análise</span><span class="sxs-lookup"><span data-stu-id="df223-264">analytics</span></span>          | <span data-ttu-id="df223-265">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="df223-265">[itemAnalytics][] resource</span></span>  | <span data-ttu-id="df223-266">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="df223-266">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="df223-267">children</span><span class="sxs-lookup"><span data-stu-id="df223-267">children</span></span>           | <span data-ttu-id="df223-268">coleção driveItem</span><span class="sxs-lookup"><span data-stu-id="df223-268">driveItem collection</span></span>        | <span data-ttu-id="df223-p133">Coleção que contêm objetos Item para os filhos imediatos do Item. Somente os itens que representam pastas têm filhos. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="df223-p133">Collection containing Item objects for the immediate children of Item. Only items representing folders have children. Read-only. Nullable.</span></span>
| <span data-ttu-id="df223-273">createdByUser</span><span class="sxs-lookup"><span data-stu-id="df223-273">createdByUser</span></span>      | <span data-ttu-id="df223-274">[user][]</span><span class="sxs-lookup"><span data-stu-id="df223-274">[user][]</span></span>                    | <span data-ttu-id="df223-275">A identidade do usuário que criou o item.</span><span class="sxs-lookup"><span data-stu-id="df223-275">Identity of the user who created the item.</span></span> <span data-ttu-id="df223-276">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-276">Read-only.</span></span>
| <span data-ttu-id="df223-277">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="df223-277">lastModifiedByUser</span></span> | <span data-ttu-id="df223-278">[user][]</span><span class="sxs-lookup"><span data-stu-id="df223-278">[user][]</span></span>                    | <span data-ttu-id="df223-279">A identidade do usuário que modificou o item pela última vez.</span><span class="sxs-lookup"><span data-stu-id="df223-279">Identity of the user who last modified the item.</span></span> <span data-ttu-id="df223-280">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-280">Read-only.</span></span>
| <span data-ttu-id="df223-281">listItem</span><span class="sxs-lookup"><span data-stu-id="df223-281">listItem</span></span>           | <span data-ttu-id="df223-282">[listItem][]</span><span class="sxs-lookup"><span data-stu-id="df223-282">[listItem][]</span></span>                | <span data-ttu-id="df223-283">Para unidades no SharePoint, o item da lista da biblioteca de documentos associado.</span><span class="sxs-lookup"><span data-stu-id="df223-283">For drives in SharePoint, the associated document library list item.</span></span> <span data-ttu-id="df223-284">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-284">Read-only.</span></span> <span data-ttu-id="df223-285">Anulável.</span><span class="sxs-lookup"><span data-stu-id="df223-285">Nullable.</span></span>
| <span data-ttu-id="df223-286">permissões</span><span class="sxs-lookup"><span data-stu-id="df223-286">permissions</span></span>        | <span data-ttu-id="df223-287">Coleção [permission][]</span><span class="sxs-lookup"><span data-stu-id="df223-287">[permission][] collection</span></span>   | <span data-ttu-id="df223-p137">O conjunto de permissões do item. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="df223-p137">The set of permissions for the item. Read-only. Nullable.</span></span>
| <span data-ttu-id="df223-291">assinaturas</span><span class="sxs-lookup"><span data-stu-id="df223-291">subscriptions</span></span>      | <span data-ttu-id="df223-292">conjunto de [assinaturas][]</span><span class="sxs-lookup"><span data-stu-id="df223-292">[subscription][] collection</span></span> | <span data-ttu-id="df223-293">O conjunto de assinaturas no item.</span><span class="sxs-lookup"><span data-stu-id="df223-293">The set of subscriptions on the item.</span></span> <span data-ttu-id="df223-294">Compatível somente na raiz de uma unidade.</span><span class="sxs-lookup"><span data-stu-id="df223-294">Only supported on the root of a drive.</span></span>
| <span data-ttu-id="df223-295">miniaturas</span><span class="sxs-lookup"><span data-stu-id="df223-295">thumbnails</span></span>         | <span data-ttu-id="df223-296">Coleção [thumbnailSet][]</span><span class="sxs-lookup"><span data-stu-id="df223-296">[thumbnailSet][] collection</span></span> | <span data-ttu-id="df223-p139">Coleção contendo objetos [ThumbnailSet][] associados ao item. Para saber mais, confira [obtendo miniaturas][]. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="df223-p139">Collection containing [ThumbnailSet][] objects associated with the item. For more info, see [getting thumbnails][]. Read-only. Nullable.</span></span>
| <span data-ttu-id="df223-301">versões</span><span class="sxs-lookup"><span data-stu-id="df223-301">versions</span></span>           | <span data-ttu-id="df223-302">coleção [driveItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="df223-302">[driveItemVersion][] collection</span></span> | <span data-ttu-id="df223-303">A lista de todas as versões anteriores do item.</span><span class="sxs-lookup"><span data-stu-id="df223-303">The list of previous versions of the item.</span></span> <span data-ttu-id="df223-304">Para saber mais, confira as informações sobre a [obtenção de versões anteriores][].</span><span class="sxs-lookup"><span data-stu-id="df223-304">For more info, see [getting previous versions][].</span></span> <span data-ttu-id="df223-305">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-305">Read-only.</span></span> <span data-ttu-id="df223-306">Anulável.</span><span class="sxs-lookup"><span data-stu-id="df223-306">Nullable.</span></span>
| <span data-ttu-id="df223-307">pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="df223-307">workbook</span></span>           | <span data-ttu-id="df223-308">[pasta de trabalho][]</span><span class="sxs-lookup"><span data-stu-id="df223-308">[workbook][]</span></span>                | <span data-ttu-id="df223-309">Para arquivos que são planilhas do Excel, acessa a API de pasta da trabalho para trabalhar com o conteúdo da planilha.</span><span class="sxs-lookup"><span data-stu-id="df223-309">For files that are Excel spreadsheets, accesses the workbook API to work with the spreadsheet's contents.</span></span> <span data-ttu-id="df223-310">Anulável.</span><span class="sxs-lookup"><span data-stu-id="df223-310">Nullable.</span></span>

## <a name="instance-attributes"></a><span data-ttu-id="df223-311">Atributos de instância</span><span class="sxs-lookup"><span data-stu-id="df223-311">Instance Attributes</span></span>

<span data-ttu-id="df223-p142">Atributos de instância são propriedades com comportamentos especiais. Essas propriedades são temporárias e a) definem o comportamento que o serviço deve apresentar ou b) fornecem valores de propriedades de curto prazo, como uma URL de download, para um item com data de expiração.</span><span class="sxs-lookup"><span data-stu-id="df223-p142">Instance attributes are properties with special behaviors. These properties are temporary and either a) define behavior the service should perform or b) provide short-term property values, like a download URL for an item that expires.</span></span>

| <span data-ttu-id="df223-314">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="df223-314">Property name</span></span>                     | <span data-ttu-id="df223-315">Tipo</span><span class="sxs-lookup"><span data-stu-id="df223-315">Type</span></span>   | <span data-ttu-id="df223-316">Descrição</span><span class="sxs-lookup"><span data-stu-id="df223-316">Description</span></span>
|:----------------------------------|:-------|:--------------------------------
| <span data-ttu-id="df223-317">@microsoft.graph.conflictBehavior</span><span class="sxs-lookup"><span data-stu-id="df223-317">@microsoft.graph.conflictBehavior</span></span> | <span data-ttu-id="df223-318">string</span><span class="sxs-lookup"><span data-stu-id="df223-318">string</span></span> | <span data-ttu-id="df223-p143">O comportamento de resolução de conflitos para ações que criam um novo item. Você pode usar os valores *fail*, *replace* ou *rename*. O padrão para PUT é *replace*. Um item nunca será retornado com essa anotação. Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="df223-p143">The conflict resolution behavior for actions that create a new item. You can use the values *fail*, *replace*, or *rename*. The default for PUT is *replace*. An item will never be returned with this annotation. Write-only.</span></span>
| <span data-ttu-id="df223-324">@microsoft.graph.downloadUrl</span><span class="sxs-lookup"><span data-stu-id="df223-324">@microsoft.graph.downloadUrl</span></span>      | <span data-ttu-id="df223-325">string</span><span class="sxs-lookup"><span data-stu-id="df223-325">string</span></span> | <span data-ttu-id="df223-p144">Uma URL que pode ser usada para baixar conteúdo desse arquivo. Uma autenticação não é obrigatória com essa URL. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df223-p144">A URL that can be used to download this file's content. Authentication is not required with this URL. Read-only.</span></span>
| <span data-ttu-id="df223-329">@microsoft.graph.sourceUrl</span><span class="sxs-lookup"><span data-stu-id="df223-329">@microsoft.graph.sourceUrl</span></span>        | <span data-ttu-id="df223-330">string</span><span class="sxs-lookup"><span data-stu-id="df223-330">string</span></span> | <span data-ttu-id="df223-p145">Quando uma solicitação PUT é emitida, essa anotação de instância pode ser usada para instruir o serviço a baixar o conteúdo da URL e armazená-lo como o arquivo. Somente gravação.</span><span class="sxs-lookup"><span data-stu-id="df223-p145">When issuing a PUT request, this instance annotation can be used to instruct the service to download the contents of the URL, and store it as the file. Write-only.</span></span>

<span data-ttu-id="df223-333">**Observação:** O valor de @microsoft.graph.downloadUrl é uma URL de curta duração e não pode ser armazenado em cache.</span><span class="sxs-lookup"><span data-stu-id="df223-333">**Note:** The @microsoft.graph.downloadUrl value is a short-lived URL and can't be cached.</span></span>
<span data-ttu-id="df223-334">A URL só estará disponível por um curto período de tempo (1 hora) antes de ser invalidada.</span><span class="sxs-lookup"><span data-stu-id="df223-334">The URL will only be available for a short period of time (1 hour) before it is invalidated.</span></span>
<span data-ttu-id="df223-335">A remoção das permissões de arquivo de um usuário pode não invalidar a URL imediatamente.</span><span class="sxs-lookup"><span data-stu-id="df223-335">Removing file permissions for a user may not immediately invalidate the URL.</span></span>

><span data-ttu-id="df223-336">**Observação:** o parâmetro @microsoft.graph.conflictBehavior deve ser incluído na URL, em vez do corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df223-336">**Note:** The parameter @microsoft.graph.conflictBehavior should be included in the URL instead of the body of the request.</span></span>

## <a name="methods"></a><span data-ttu-id="df223-337">Methods</span><span class="sxs-lookup"><span data-stu-id="df223-337">Methods</span></span>

| <span data-ttu-id="df223-338">Método</span><span class="sxs-lookup"><span data-stu-id="df223-338">Method</span></span>                                                   | <span data-ttu-id="df223-339">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="df223-339">REST Path</span></span>
|:---------------------------------------------------------|:------------------
| [<span data-ttu-id="df223-340">Obter item</span><span class="sxs-lookup"><span data-stu-id="df223-340">Get item</span></span>](../api/driveitem-get.md)                      | `GET /drive/items/{item-id}`
| [<span data-ttu-id="df223-341">Listar atividades</span><span class="sxs-lookup"><span data-stu-id="df223-341">List activities</span></span>](../api/activities-list.md)             | `GET /drive/items/{item-id}/activities`
| <span data-ttu-id="df223-342">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="df223-342">[Get analytics][]</span></span>                                        | `GET /drive/items/{item-id}/analytics`
| <span data-ttu-id="df223-343">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="df223-343">[Get activities by interval][]</span></span>                           | `GET /drive/items/{item-id}/getActivitiesByInterval`
| [<span data-ttu-id="df223-344">Listar filhos</span><span class="sxs-lookup"><span data-stu-id="df223-344">List children</span></span>](../api/driveitem-list-children.md)       | `GET /drive/items/{item-id}/children`
| [<span data-ttu-id="df223-345">Listar versões</span><span class="sxs-lookup"><span data-stu-id="df223-345">List versions</span></span>](../api/driveitem-list-versions.md)       | `GET /drive/items/{item-id}/versions`
| [<span data-ttu-id="df223-346">Criar item</span><span class="sxs-lookup"><span data-stu-id="df223-346">Create item</span></span>](../api/driveitem-post-children.md)         | `POST /drive/items/{item-id}/children`
| [<span data-ttu-id="df223-347">Atualizar item</span><span class="sxs-lookup"><span data-stu-id="df223-347">Update item</span></span>](../api/driveitem-update.md)                | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="df223-348">Carregar conteúdo</span><span class="sxs-lookup"><span data-stu-id="df223-348">Upload content</span></span>](../api/driveitem-put-content.md)        | `PUT /drive/items/{item-id}/content`
| [<span data-ttu-id="df223-349">Baixar conteúdo</span><span class="sxs-lookup"><span data-stu-id="df223-349">Download content</span></span>](../api/driveitem-get-content.md)      | `GET /drive/items/{item-id}/content`
| <span data-ttu-id="df223-350">[Baixar o formato de arquivo específico][download-format]</span><span class="sxs-lookup"><span data-stu-id="df223-350">[Download specific file format][download-format]</span></span>         | `GET /drive/items/{item-id}/content?format={format}`
| [<span data-ttu-id="df223-351">Excluir item</span><span class="sxs-lookup"><span data-stu-id="df223-351">Delete item</span></span>](../api/driveitem-delete.md)                | `DELETE /drive/items/{item-id}`
| [<span data-ttu-id="df223-352">Restaurar item</span><span class="sxs-lookup"><span data-stu-id="df223-352">Restore item</span></span>](../api/driveitem-restore.md)              | `POST /drive/items/{item-id}/restore`
| [<span data-ttu-id="df223-353">Mover item</span><span class="sxs-lookup"><span data-stu-id="df223-353">Move item</span></span>](../api/driveitem-move.md)                    | `PATCH /drive/items/{item-id}`
| [<span data-ttu-id="df223-354">Copiar item</span><span class="sxs-lookup"><span data-stu-id="df223-354">Copy item</span></span>](../api/driveitem-copy.md)                    | `POST /drive/items/{item-id}/copy`
| [<span data-ttu-id="df223-355">Pesquisar itens</span><span class="sxs-lookup"><span data-stu-id="df223-355">Search items</span></span>](../api/driveitem-search.md)               | `GET /drive/items/{item-id}/search(q='text')`
| [<span data-ttu-id="df223-356">Listar alterações em uma unidade</span><span class="sxs-lookup"><span data-stu-id="df223-356">List changes in a drive</span></span>](../api/driveitem-delta.md)     | `GET /drive/root/delta`
| [<span data-ttu-id="df223-357">Seguir item</span><span class="sxs-lookup"><span data-stu-id="df223-357">Follow item</span></span>](../api/driveitem-follow.md)                | `POST /drives/{drive-id}/items/{item-id}/follow`
| [<span data-ttu-id="df223-358">Item inseguir</span><span class="sxs-lookup"><span data-stu-id="df223-358">Unfollow item</span></span>](../api/driveitem-unfollow.md)            | `POST /drives/{drive-id}/items/{item-id}/unfollow`
| [<span data-ttu-id="df223-359">Listar miniaturas</span><span class="sxs-lookup"><span data-stu-id="df223-359">List thumbnails</span></span>](../api/driveitem-list-thumbnails.md)   | `GET /drive/items/{item-id}/thumbnails`
| [<span data-ttu-id="df223-360">Criar link de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="df223-360">Create sharing link</span></span>](../api/driveitem-createlink.md)    | `POST /drive/items/{item-id}/createLink`
| [<span data-ttu-id="df223-361">Adicionar permissões</span><span class="sxs-lookup"><span data-stu-id="df223-361">Add permissions</span></span>](../api/driveitem-invite.md)            | `POST /drive/items/{item-id}/invite`
| [<span data-ttu-id="df223-362">Listar permissões</span><span class="sxs-lookup"><span data-stu-id="df223-362">List permissions</span></span>](../api/driveitem-list-permissions.md) | `GET /drive/items/{item-id}/permissions`
| [<span data-ttu-id="df223-363">Excluir permissão</span><span class="sxs-lookup"><span data-stu-id="df223-363">Delete permission</span></span>](../api/permission-delete.md)         | `DELETE /drive/items/{item-id}/permissions/{perm-id}`
| <span data-ttu-id="df223-364">[Obter canal WebSocket][getWebSocket]</span><span class="sxs-lookup"><span data-stu-id="df223-364">[Get WebSocket channel][getWebSocket]</span></span>                    | `GET /drive/root/subscriptions/socketIo`
| <span data-ttu-id="df223-365">[Item de visualização][item-preview]</span><span class="sxs-lookup"><span data-stu-id="df223-365">[Preview item][item-preview]</span></span>                             | `POST /drive/items/{item-id}/preview`
| [<span data-ttu-id="df223-366">Fazer ceck-in</span><span class="sxs-lookup"><span data-stu-id="df223-366">Check in</span></span>](../api/driveitem-checkin.md)                  | `POST /drives/{driveId}/items/{itemId}/checkin`
| [<span data-ttu-id="df223-367">Fazer check-out</span><span class="sxs-lookup"><span data-stu-id="df223-367">Check out</span></span>](../api/driveitem-checkout.md)                | `POST /drives/{driveId}/items/{itemId}/checkout`
| [<span data-ttu-id="df223-368">Revogar concessões</span><span class="sxs-lookup"><span data-stu-id="df223-368">Revoke grants</span></span>](../api/permission-revokegrants.md)   | `PATCH /drive/items/{item-id}/permissions/{perm-id}/revokeGrants`

[item-preview]: ../api/driveitem-preview.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md

## <a name="remarks"></a><span data-ttu-id="df223-371">Comentários</span><span class="sxs-lookup"><span data-stu-id="df223-371">Remarks</span></span>

<span data-ttu-id="df223-372">Em bibliotecas de documentos do OneDrive for Business ou do SharePoint, a propriedade **cTag** não será retornada se **driveItem** for uma faceta [folder][].</span><span class="sxs-lookup"><span data-stu-id="df223-372">In OneDrive for Business or SharePoint document libraries, the **cTag** property is not returned, if the **driveItem** has a [folder][] facet.</span></span>

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
[getWebSocket]: ../api/subscriptions-socketio.md
[identitySet]: identityset.md
[image]: image.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[geoCoordinates]: geocoordinates.md
[List activities]: ../api/activities-list.md
[listItem]: listitem.md
[package]: package.md
[permissão]: permission.md
[permission]: permission.md
[pendingOperations]: pendingoperations.md
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
[Usuário]: /graph/api/resources/users
[user]: /graph/api/resources/users
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
  "suppressions": []
}
-->