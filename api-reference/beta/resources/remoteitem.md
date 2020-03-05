---
author: JeremyKelley
description: O recurso remoteItem indica que um driveItem faz referência a um item que existe em outra unidade.
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: eb4d937d7b2feab6589ddd965eb6a6524162b7fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521163"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="6fb74-103">Tipo de recurso RemoteItem</span><span class="sxs-lookup"><span data-stu-id="6fb74-103">RemoteItem resource type</span></span>

<span data-ttu-id="6fb74-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6fb74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb74-105">O recurso **remoteItem** indica que um [**driveItem**](driveitem.md) faz referência a um item que existe em outra unidade.</span><span class="sxs-lookup"><span data-stu-id="6fb74-105">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive.</span></span>
<span data-ttu-id="6fb74-106">Este recurso fornece as IDs exclusivas do da unidade de origem e do item de destino.</span><span class="sxs-lookup"><span data-stu-id="6fb74-106">This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="6fb74-107">[**DriveItems**](driveitem.md) com uma faceta **remoteItem** não nula são recursos que são compartilhados, adicionados ao OneDrive do usuário ou em itens retornados de coleções de itens heterogêneas (como resultados de pesquisa).</span><span class="sxs-lookup"><span data-stu-id="6fb74-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="6fb74-108">**Observação:** Diferentemente de pastas na mesma unidade, um **driveItem** movido para um item remoto pode ter seu valor `id` alterado.</span><span class="sxs-lookup"><span data-stu-id="6fb74-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fb74-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fb74-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6fb74-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fb74-110">Properties</span></span>

| <span data-ttu-id="6fb74-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6fb74-111">Property name</span></span>        | <span data-ttu-id="6fb74-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fb74-112">Type</span></span>                                | <span data-ttu-id="6fb74-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fb74-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="6fb74-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="6fb74-114">createdBy</span></span>            | [<span data-ttu-id="6fb74-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6fb74-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="6fb74-p102">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p102">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="6fb74-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb74-118">createdDateTime</span></span>      | <span data-ttu-id="6fb74-119">Carimbo de data/hora</span><span class="sxs-lookup"><span data-stu-id="6fb74-119">Timestamp</span></span>                           | <span data-ttu-id="6fb74-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="6fb74-122">file</span><span class="sxs-lookup"><span data-stu-id="6fb74-122">file</span></span>                 | [<span data-ttu-id="6fb74-123">File</span><span class="sxs-lookup"><span data-stu-id="6fb74-123">File</span></span>](file.md)                     | <span data-ttu-id="6fb74-p104">Indica que o item remoto é um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p104">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="6fb74-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="6fb74-126">fileSystemInfo</span></span>       | [<span data-ttu-id="6fb74-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="6fb74-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="6fb74-p105">Informações sobre o item remoto do sistema de arquivos local. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p105">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="6fb74-130">folder</span><span class="sxs-lookup"><span data-stu-id="6fb74-130">folder</span></span>               | [<span data-ttu-id="6fb74-131">Folder</span><span class="sxs-lookup"><span data-stu-id="6fb74-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="6fb74-p106">Indica que o item remoto é uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p106">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="6fb74-134">id</span><span class="sxs-lookup"><span data-stu-id="6fb74-134">id</span></span>                   | <span data-ttu-id="6fb74-135">String</span><span class="sxs-lookup"><span data-stu-id="6fb74-135">String</span></span>                              | <span data-ttu-id="6fb74-p107">Identificador exclusivo do item remoto em sua unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p107">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="6fb74-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6fb74-138">lastModifiedBy</span></span>       | [<span data-ttu-id="6fb74-139">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6fb74-139">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="6fb74-p108">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="6fb74-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb74-142">lastModifiedDateTime</span></span> | <span data-ttu-id="6fb74-143">Timestamp</span><span class="sxs-lookup"><span data-stu-id="6fb74-143">Timestamp</span></span>                           | <span data-ttu-id="6fb74-p109">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="6fb74-146">nome</span><span class="sxs-lookup"><span data-stu-id="6fb74-146">name</span></span>                 | <span data-ttu-id="6fb74-147">String</span><span class="sxs-lookup"><span data-stu-id="6fb74-147">String</span></span>                              | <span data-ttu-id="6fb74-p110">Opcional. Nome de arquivo do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p110">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="6fb74-151">pacote</span><span class="sxs-lookup"><span data-stu-id="6fb74-151">package</span></span>              | [<span data-ttu-id="6fb74-152">Pacote</span><span class="sxs-lookup"><span data-stu-id="6fb74-152">Package</span></span>](package.md)               | <span data-ttu-id="6fb74-p111">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p111">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="6fb74-156">parentReference</span><span class="sxs-lookup"><span data-stu-id="6fb74-156">parentReference</span></span>      | [<span data-ttu-id="6fb74-157">ItemReference</span><span class="sxs-lookup"><span data-stu-id="6fb74-157">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="6fb74-p112">Propriedades do pai do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p112">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="6fb74-160">compartilhado</span><span class="sxs-lookup"><span data-stu-id="6fb74-160">shared</span></span>               | [<span data-ttu-id="6fb74-161">compartilhado</span><span class="sxs-lookup"><span data-stu-id="6fb74-161">shared</span></span>](shared.md)                 | <span data-ttu-id="6fb74-p113">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p113">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="6fb74-164">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6fb74-164">sharepointIds</span></span>        | [<span data-ttu-id="6fb74-165">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="6fb74-165">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="6fb74-p114">Fornece interoperabilidade entre itens no OneDrive for Business e no SharePoint com o conjunto completo de identificadores de item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p114">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="6fb74-168">size</span><span class="sxs-lookup"><span data-stu-id="6fb74-168">size</span></span>                 | <span data-ttu-id="6fb74-169">Int64</span><span class="sxs-lookup"><span data-stu-id="6fb74-169">Int64</span></span>                               | <span data-ttu-id="6fb74-p115">Tamanho do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p115">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="6fb74-172">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="6fb74-172">webDavUrl</span></span>            | <span data-ttu-id="6fb74-173">URL</span><span class="sxs-lookup"><span data-stu-id="6fb74-173">Url</span></span>                                 | <span data-ttu-id="6fb74-174">URL compatível com DAV para o item.</span><span class="sxs-lookup"><span data-stu-id="6fb74-174">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="6fb74-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="6fb74-175">webUrl</span></span>               | <span data-ttu-id="6fb74-176">URL</span><span class="sxs-lookup"><span data-stu-id="6fb74-176">Url</span></span>                                 | <span data-ttu-id="6fb74-p116">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6fb74-p116">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="6fb74-179">Comentários</span><span class="sxs-lookup"><span data-stu-id="6fb74-179">Remarks</span></span>

<span data-ttu-id="6fb74-180">Para saber mais sobre as facetas de um **driveItem**, confira [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6fb74-180">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

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
