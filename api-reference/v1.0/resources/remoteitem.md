---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: ceb66fdacd4a108318c84fd9297aca8b2332c3f3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579335"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="154d6-102">Tipo de recurso RemoteItem</span><span class="sxs-lookup"><span data-stu-id="154d6-102">RemoteItem resource type</span></span>

<span data-ttu-id="154d6-103">O recurso **remoteItem** indica que um [**driveItem**](driveitem.md) faz referência a um item que existe em outra unidade.</span><span class="sxs-lookup"><span data-stu-id="154d6-103">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="154d6-104">Este recurso fornece as IDs exclusivas do da unidade de origem e do item de destino.</span><span class="sxs-lookup"><span data-stu-id="154d6-104">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="154d6-105">[**DriveItems**](driveitem.md) com uma faceta **remoteItem** não nula são recursos que são compartilhados, adicionados ao OneDrive do usuário ou em itens retornados de coleções de itens heterogêneas (como resultados de pesquisa).</span><span class="sxs-lookup"><span data-stu-id="154d6-105">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="154d6-106">**Observação:** Diferentemente de pastas na mesma unidade, um **driveItem** movido para um item remoto pode ter seu valor `id` alterado.</span><span class="sxs-lookup"><span data-stu-id="154d6-106">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="154d6-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="154d6-107">JSON representation</span></span>

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
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "name": "string",
  "package": { "@odata.type": "microsoft.graph.package" },
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "shared": { "@odata.type": "microsoft.graph.shared" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "specialFolder": { "@odata.type": "microsoft.graph.specialFolder" },
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="154d6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="154d6-108">Properties</span></span>

| <span data-ttu-id="154d6-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="154d6-109">Property name</span></span>        | <span data-ttu-id="154d6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="154d6-110">Type</span></span>                                | <span data-ttu-id="154d6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="154d6-111">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="154d6-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="154d6-112">createdBy</span></span>            | [<span data-ttu-id="154d6-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="154d6-113">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="154d6-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="154d6-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="154d6-116">createdDateTime</span></span>      | <span data-ttu-id="154d6-117">Carimbo de data/hora</span><span class="sxs-lookup"><span data-stu-id="154d6-117">Timestamp</span></span>                           | <span data-ttu-id="154d6-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="154d6-120">file</span><span class="sxs-lookup"><span data-stu-id="154d6-120">file</span></span>                 | [<span data-ttu-id="154d6-121">File</span><span class="sxs-lookup"><span data-stu-id="154d6-121">File</span></span>](file.md)                     | <span data-ttu-id="154d6-p104">Indica que o item remoto é um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="154d6-124">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="154d6-124">fileSystemInfo</span></span>       | [<span data-ttu-id="154d6-125">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="154d6-125">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="154d6-p105">Informações sobre o item remoto do sistema de arquivos local. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="154d6-128">folder</span><span class="sxs-lookup"><span data-stu-id="154d6-128">folder</span></span>               | [<span data-ttu-id="154d6-129">Folder</span><span class="sxs-lookup"><span data-stu-id="154d6-129">Folder</span></span>](folder.md)                 | <span data-ttu-id="154d6-p106">Indica que o item remoto é uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="154d6-132">id</span><span class="sxs-lookup"><span data-stu-id="154d6-132">id</span></span>                   | <span data-ttu-id="154d6-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="154d6-133">String</span></span>                              | <span data-ttu-id="154d6-p107">Identificador exclusivo do item remoto em sua unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="154d6-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="154d6-136">lastModifiedBy</span></span>       | [<span data-ttu-id="154d6-137">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="154d6-137">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="154d6-p108">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="154d6-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="154d6-140">lastModifiedDateTime</span></span> | <span data-ttu-id="154d6-141">Timestamp</span><span class="sxs-lookup"><span data-stu-id="154d6-141">Timestamp</span></span>                           | <span data-ttu-id="154d6-p109">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="154d6-144">nome</span><span class="sxs-lookup"><span data-stu-id="154d6-144">name</span></span>                 | <span data-ttu-id="154d6-145">String</span><span class="sxs-lookup"><span data-stu-id="154d6-145">String</span></span>                              | <span data-ttu-id="154d6-p110">Opcional. Nome de arquivo do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="154d6-149">pacote</span><span class="sxs-lookup"><span data-stu-id="154d6-149">package</span></span>              | [<span data-ttu-id="154d6-150">Pacote</span><span class="sxs-lookup"><span data-stu-id="154d6-150">Package</span></span>](package.md)               | <span data-ttu-id="154d6-p111">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="154d6-154">parentReference</span><span class="sxs-lookup"><span data-stu-id="154d6-154">parentReference</span></span>      | [<span data-ttu-id="154d6-155">ItemReference</span><span class="sxs-lookup"><span data-stu-id="154d6-155">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="154d6-p112">Propriedades do pai do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="154d6-158">compartilhado</span><span class="sxs-lookup"><span data-stu-id="154d6-158">shared</span></span>               | [<span data-ttu-id="154d6-159">compartilhado</span><span class="sxs-lookup"><span data-stu-id="154d6-159">shared</span></span>](shared.md)                 | <span data-ttu-id="154d6-p113">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="154d6-162">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="154d6-162">sharepointIds</span></span>        | [<span data-ttu-id="154d6-163">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="154d6-163">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="154d6-p114">Fornece interoperabilidade entre itens no OneDrive for Business e no SharePoint com o conjunto completo de identificadores de item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="154d6-166">size</span><span class="sxs-lookup"><span data-stu-id="154d6-166">size</span></span>                 | <span data-ttu-id="154d6-167">Int64</span><span class="sxs-lookup"><span data-stu-id="154d6-167">Int64</span></span>                               | <span data-ttu-id="154d6-p115">Tamanho do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="154d6-170">specialFolder</span><span class="sxs-lookup"><span data-stu-id="154d6-170">specialFolder</span></span>        | <span data-ttu-id="154d6-171">[specialFolder][]</span><span class="sxs-lookup"><span data-stu-id="154d6-171">[specialFolder][]</span></span>                   | <span data-ttu-id="154d6-p116">Se o item atual também estiver disponível como uma pasta especial, essa faceta será retornada. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p116">If the current item is also available as a special folder, this facet is returned. Read-only.</span></span>                                                                     |
| <span data-ttu-id="154d6-174">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="154d6-174">webDavUrl</span></span>            | <span data-ttu-id="154d6-175">URL</span><span class="sxs-lookup"><span data-stu-id="154d6-175">Url</span></span>                                 | <span data-ttu-id="154d6-176">URL compatível com DAV para o item.</span><span class="sxs-lookup"><span data-stu-id="154d6-176">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="154d6-177">webUrl</span><span class="sxs-lookup"><span data-stu-id="154d6-177">webUrl</span></span>               | <span data-ttu-id="154d6-178">URL</span><span class="sxs-lookup"><span data-stu-id="154d6-178">Url</span></span>                                 | <span data-ttu-id="154d6-p117">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="154d6-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

[specialFolder]: specialfolder.md

## <a name="remarks"></a><span data-ttu-id="154d6-182">Comentários</span><span class="sxs-lookup"><span data-stu-id="154d6-182">Remarks</span></span>

<span data-ttu-id="154d6-183">Para saber mais sobre as facetas de um **driveItem**, confira [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="154d6-183">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
