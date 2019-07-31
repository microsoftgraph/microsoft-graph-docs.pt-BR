---
author: JeremyKelley
description: O recurso remoteItem indica que um driveItem faz referência a um item que existe em outra unidade.
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 05da43fb3d7b1e2adec01f707eeed61df4623f04
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008702"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="5b82e-103">Tipo de recurso RemoteItem</span><span class="sxs-lookup"><span data-stu-id="5b82e-103">RemoteItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b82e-104">O recurso **remoteItem** indica que um [**driveItem**](driveitem.md) faz referência a um item que existe em outra unidade.</span><span class="sxs-lookup"><span data-stu-id="5b82e-104">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="5b82e-105">Este recurso fornece as IDs exclusivas do da unidade de origem e do item de destino.</span><span class="sxs-lookup"><span data-stu-id="5b82e-105">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="5b82e-106">[**DriveItems**](driveitem.md) com uma faceta **remoteItem** não nula são recursos que são compartilhados, adicionados ao OneDrive do usuário ou em itens retornados de coleções de itens heterogêneas (como resultados de pesquisa).</span><span class="sxs-lookup"><span data-stu-id="5b82e-106">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="5b82e-107">**Observação:** Diferentemente de pastas na mesma unidade, um **driveItem** movido para um item remoto pode ter seu valor `id` alterado.</span><span class="sxs-lookup"><span data-stu-id="5b82e-107">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b82e-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b82e-108">JSON representation</span></span>

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
  "size": 1024,
  "webDavUrl": "url",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="5b82e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b82e-109">Properties</span></span>

| <span data-ttu-id="5b82e-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5b82e-110">Property name</span></span>        | <span data-ttu-id="5b82e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b82e-111">Type</span></span>                                | <span data-ttu-id="5b82e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b82e-112">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5b82e-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="5b82e-113">createdBy</span></span>            | [<span data-ttu-id="5b82e-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="5b82e-114">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="5b82e-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="5b82e-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b82e-117">createdDateTime</span></span>      | <span data-ttu-id="5b82e-118">Carimbo de data/hora</span><span class="sxs-lookup"><span data-stu-id="5b82e-118">Timestamp</span></span>                           | <span data-ttu-id="5b82e-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="5b82e-121">file</span><span class="sxs-lookup"><span data-stu-id="5b82e-121">file</span></span>                 | [<span data-ttu-id="5b82e-122">File</span><span class="sxs-lookup"><span data-stu-id="5b82e-122">File</span></span>](file.md)                     | <span data-ttu-id="5b82e-p104">Indica que o item remoto é um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="5b82e-125">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="5b82e-125">fileSystemInfo</span></span>       | [<span data-ttu-id="5b82e-126">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="5b82e-126">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="5b82e-p105">Informações sobre o item remoto do sistema de arquivos local. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="5b82e-129">folder</span><span class="sxs-lookup"><span data-stu-id="5b82e-129">folder</span></span>               | [<span data-ttu-id="5b82e-130">Folder</span><span class="sxs-lookup"><span data-stu-id="5b82e-130">Folder</span></span>](folder.md)                 | <span data-ttu-id="5b82e-p106">Indica que o item remoto é uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="5b82e-133">id</span><span class="sxs-lookup"><span data-stu-id="5b82e-133">id</span></span>                   | <span data-ttu-id="5b82e-134">String</span><span class="sxs-lookup"><span data-stu-id="5b82e-134">String</span></span>                              | <span data-ttu-id="5b82e-p107">Identificador exclusivo do item remoto em sua unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="5b82e-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5b82e-137">lastModifiedBy</span></span>       | [<span data-ttu-id="5b82e-138">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="5b82e-138">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="5b82e-p108">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="5b82e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b82e-141">lastModifiedDateTime</span></span> | <span data-ttu-id="5b82e-142">Timestamp</span><span class="sxs-lookup"><span data-stu-id="5b82e-142">Timestamp</span></span>                           | <span data-ttu-id="5b82e-p109">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="5b82e-145">nome</span><span class="sxs-lookup"><span data-stu-id="5b82e-145">name</span></span>                 | <span data-ttu-id="5b82e-146">String</span><span class="sxs-lookup"><span data-stu-id="5b82e-146">String</span></span>                              | <span data-ttu-id="5b82e-p110">Opcional. Nome de arquivo do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="5b82e-150">pacote</span><span class="sxs-lookup"><span data-stu-id="5b82e-150">package</span></span>              | [<span data-ttu-id="5b82e-151">Pacote</span><span class="sxs-lookup"><span data-stu-id="5b82e-151">Package</span></span>](package.md)               | <span data-ttu-id="5b82e-p111">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="5b82e-155">parentReference</span><span class="sxs-lookup"><span data-stu-id="5b82e-155">parentReference</span></span>      | [<span data-ttu-id="5b82e-156">ItemReference</span><span class="sxs-lookup"><span data-stu-id="5b82e-156">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="5b82e-p112">Propriedades do pai do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="5b82e-159">compartilhado</span><span class="sxs-lookup"><span data-stu-id="5b82e-159">shared</span></span>               | [<span data-ttu-id="5b82e-160">compartilhado</span><span class="sxs-lookup"><span data-stu-id="5b82e-160">shared</span></span>](shared.md)                 | <span data-ttu-id="5b82e-p113">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="5b82e-163">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="5b82e-163">sharepointIds</span></span>        | [<span data-ttu-id="5b82e-164">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="5b82e-164">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="5b82e-p114">Fornece interoperabilidade entre itens no OneDrive for Business e no SharePoint com o conjunto completo de identificadores de item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="5b82e-167">size</span><span class="sxs-lookup"><span data-stu-id="5b82e-167">size</span></span>                 | <span data-ttu-id="5b82e-168">Int64</span><span class="sxs-lookup"><span data-stu-id="5b82e-168">Int64</span></span>                               | <span data-ttu-id="5b82e-p115">Tamanho do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="5b82e-171">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="5b82e-171">webDavUrl</span></span>            | <span data-ttu-id="5b82e-172">URL</span><span class="sxs-lookup"><span data-stu-id="5b82e-172">Url</span></span>                                 | <span data-ttu-id="5b82e-173">URL compatível com DAV para o item.</span><span class="sxs-lookup"><span data-stu-id="5b82e-173">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="5b82e-174">webUrl</span><span class="sxs-lookup"><span data-stu-id="5b82e-174">webUrl</span></span>               | <span data-ttu-id="5b82e-175">URL</span><span class="sxs-lookup"><span data-stu-id="5b82e-175">Url</span></span>                                 | <span data-ttu-id="5b82e-p116">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b82e-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="5b82e-178">Comentários</span><span class="sxs-lookup"><span data-stu-id="5b82e-178">Remarks</span></span>

<span data-ttu-id="5b82e-179">Para saber mais sobre as facetas de um **driveItem**, confira [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5b82e-179">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

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
