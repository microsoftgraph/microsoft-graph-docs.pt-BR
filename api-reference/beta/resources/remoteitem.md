---
author: JeremyKelley
description: O recurso remoteItem indica que um driveItem faz referência a um item que existe em outra unidade.
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0b672f917487719b8994d8c99aad8be8c8d24190
ms.sourcegitcommit: 2ac179fb774a15c9e9c01502e59c76efb57803a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2020
ms.locfileid: "42986093"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="72b65-103">Tipo de recurso RemoteItem</span><span class="sxs-lookup"><span data-stu-id="72b65-103">RemoteItem resource type</span></span>

<span data-ttu-id="72b65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72b65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b65-105">O recurso **remoteItem** indica que um [**driveItem**](driveitem.md) faz referência a um item que existe em outra unidade.</span><span class="sxs-lookup"><span data-stu-id="72b65-105">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="72b65-106">Este recurso fornece as IDs exclusivas do da unidade de origem e do item de destino.</span><span class="sxs-lookup"><span data-stu-id="72b65-106">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="72b65-107">[**DriveItems**](driveitem.md) com uma faceta **remoteItem** não nula são recursos que são compartilhados, adicionados ao OneDrive do usuário ou em itens retornados de coleções de itens heterogêneas (como resultados de pesquisa).</span><span class="sxs-lookup"><span data-stu-id="72b65-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="72b65-108">**Observação:** Diferentemente de pastas na mesma unidade, um **driveItem** movido para um item remoto pode ter seu valor `id` alterado.</span><span class="sxs-lookup"><span data-stu-id="72b65-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72b65-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72b65-109">JSON representation</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.remoteItem", 
       "optionalProperties": ["name", "fileSystemInfo", "file", "folder"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "file": { "@odata.type": "microsoft.graph.file" },
  "fileSystemInfo": { "@odata.type": "microsoft.graph.fileSystemInfo" },
  "folder": { "@odata.type": "microsoft.graph.folder" },
  "image" : { "@odata.type": "microsoft.graph.image" },
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "size": 1024,
  "video": { "@odata.type": "microsoft.graph.video" },
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="72b65-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72b65-110">Properties</span></span>

| <span data-ttu-id="72b65-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="72b65-111">Property name</span></span>        | <span data-ttu-id="72b65-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="72b65-112">Type</span></span>                                | <span data-ttu-id="72b65-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="72b65-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="72b65-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="72b65-114">createdBy</span></span>            | [<span data-ttu-id="72b65-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="72b65-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="72b65-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="72b65-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72b65-118">createdDateTime</span></span>      | <span data-ttu-id="72b65-119">Carimbo de data/hora</span><span class="sxs-lookup"><span data-stu-id="72b65-119">Timestamp</span></span>                           | <span data-ttu-id="72b65-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="72b65-122">file</span><span class="sxs-lookup"><span data-stu-id="72b65-122">file</span></span>                 | [<span data-ttu-id="72b65-123">File</span><span class="sxs-lookup"><span data-stu-id="72b65-123">File</span></span>](file.md)                     | <span data-ttu-id="72b65-p104">Indica que o item remoto é um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="72b65-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="72b65-126">fileSystemInfo</span></span>       | [<span data-ttu-id="72b65-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="72b65-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="72b65-p105">Informações sobre o item remoto do sistema de arquivos local. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="72b65-130">folder</span><span class="sxs-lookup"><span data-stu-id="72b65-130">folder</span></span>               | [<span data-ttu-id="72b65-131">Folder</span><span class="sxs-lookup"><span data-stu-id="72b65-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="72b65-p106">Indica que o item remoto é uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="72b65-134">id</span><span class="sxs-lookup"><span data-stu-id="72b65-134">id</span></span>                   | <span data-ttu-id="72b65-135">String</span><span class="sxs-lookup"><span data-stu-id="72b65-135">String</span></span>                              | <span data-ttu-id="72b65-p107">Identificador exclusivo do item remoto em sua unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="72b65-138">image</span><span class="sxs-lookup"><span data-stu-id="72b65-138">image</span></span>                | [<span data-ttu-id="72b65-139">Imagem</span><span class="sxs-lookup"><span data-stu-id="72b65-139">Image</span></span>](image.md)                   | <span data-ttu-id="72b65-p108">Metadados de imagem, se o item for uma imagem. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p108">Image metadata, if the item is an image. Read-only.</span></span>                                                                                               |
| <span data-ttu-id="72b65-142">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="72b65-142">lastModifiedBy</span></span>       | [<span data-ttu-id="72b65-143">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="72b65-143">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="72b65-p109">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p109">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="72b65-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72b65-146">lastModifiedDateTime</span></span> | <span data-ttu-id="72b65-147">Timestamp</span><span class="sxs-lookup"><span data-stu-id="72b65-147">Timestamp</span></span>                           | <span data-ttu-id="72b65-p110">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p110">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="72b65-150">nome</span><span class="sxs-lookup"><span data-stu-id="72b65-150">name</span></span>                 | <span data-ttu-id="72b65-151">String</span><span class="sxs-lookup"><span data-stu-id="72b65-151">String</span></span>                              | <span data-ttu-id="72b65-p111">Opcional. Nome de arquivo do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p111">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="72b65-155">pacote</span><span class="sxs-lookup"><span data-stu-id="72b65-155">package</span></span>              | [<span data-ttu-id="72b65-156">Pacote</span><span class="sxs-lookup"><span data-stu-id="72b65-156">Package</span></span>](package.md)               | <span data-ttu-id="72b65-p112">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p112">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="72b65-160">parentReference</span><span class="sxs-lookup"><span data-stu-id="72b65-160">parentReference</span></span>      | [<span data-ttu-id="72b65-161">ItemReference</span><span class="sxs-lookup"><span data-stu-id="72b65-161">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="72b65-p113">Propriedades do pai do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p113">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="72b65-164">compartilhado</span><span class="sxs-lookup"><span data-stu-id="72b65-164">shared</span></span>               | [<span data-ttu-id="72b65-165">compartilhado</span><span class="sxs-lookup"><span data-stu-id="72b65-165">shared</span></span>](shared.md)                 | <span data-ttu-id="72b65-p114">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p114">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="72b65-168">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="72b65-168">sharepointIds</span></span>        | [<span data-ttu-id="72b65-169">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="72b65-169">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="72b65-p115">Fornece interoperabilidade entre itens no OneDrive for Business e no SharePoint com o conjunto completo de identificadores de item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p115">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="72b65-172">size</span><span class="sxs-lookup"><span data-stu-id="72b65-172">size</span></span>                 | <span data-ttu-id="72b65-173">Int64</span><span class="sxs-lookup"><span data-stu-id="72b65-173">Int64</span></span>                               | <span data-ttu-id="72b65-p116">Tamanho do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p116">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="72b65-176">video</span><span class="sxs-lookup"><span data-stu-id="72b65-176">video</span></span>                | [<span data-ttu-id="72b65-177">Video</span><span class="sxs-lookup"><span data-stu-id="72b65-177">Video</span></span>](video.md)                   | <span data-ttu-id="72b65-p117">Metadados de vídeo, se o item for um vídeo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p117">Video metadata, if the item is a video. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="72b65-180">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="72b65-180">webDavUrl</span></span>            | <span data-ttu-id="72b65-181">URL</span><span class="sxs-lookup"><span data-stu-id="72b65-181">Url</span></span>                                 | <span data-ttu-id="72b65-182">URL compatível com DAV para o item.</span><span class="sxs-lookup"><span data-stu-id="72b65-182">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="72b65-183">webUrl</span><span class="sxs-lookup"><span data-stu-id="72b65-183">webUrl</span></span>               | <span data-ttu-id="72b65-184">URL</span><span class="sxs-lookup"><span data-stu-id="72b65-184">Url</span></span>                                 | <span data-ttu-id="72b65-p118">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="72b65-p118">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="72b65-187">Comentários</span><span class="sxs-lookup"><span data-stu-id="72b65-187">Remarks</span></span>

<span data-ttu-id="72b65-188">Para saber mais sobre as facetas de um **driveItem**, confira [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="72b65-188">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem",
  "suppressions": []
}
-->
