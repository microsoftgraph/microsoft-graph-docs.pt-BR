---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: RemoteItem
localization_priority: Normal
ms.openlocfilehash: 122e13513db1a59e23a41cadd16e61996e6a6c04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843187"
---
# <a name="remoteitem-resource-type"></a><span data-ttu-id="5f088-102">Tipo de recurso RemoteItem</span><span class="sxs-lookup"><span data-stu-id="5f088-102">RemoteItem resource type</span></span>

> <span data-ttu-id="5f088-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f088-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f088-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f088-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f088-p102">O recurso **remoteItem** indica que um [**driveItem**](driveitem.md) faz referência a um item que existe em outra unidade. Este recurso fornece as IDs exclusivas do da unidade de origem e do item de destino.</span><span class="sxs-lookup"><span data-stu-id="5f088-p102">The **remoteItem** resource indicates that a [**driveItem**](driveitem.md) references an item that exists in another drive. This resource provides the unique IDs of the source drive and target item.</span></span>

<span data-ttu-id="5f088-107">[**DriveItems**](driveitem.md) com uma faceta **remoteItem** não nula são recursos que são compartilhados, adicionados ao OneDrive do usuário ou em itens retornados de coleções de itens heterogêneas (como resultados de pesquisa).</span><span class="sxs-lookup"><span data-stu-id="5f088-107">[**DriveItems**](driveitem.md) with a non-null **remoteItem** facet are resources that are shared, added to the user's OneDrive, or on items returned from hetrogenous collections of items (like search results).</span></span>

<span data-ttu-id="5f088-108">**Observação:** Diferentemente de pastas na mesma unidade, um **driveItem** movido para um item remoto pode ter seu valor `id` alterado.</span><span class="sxs-lookup"><span data-stu-id="5f088-108">**Note:** Unlike with folders in the same drive, a **driveItem** moved into a remote item may have its `id` value changed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f088-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f088-109">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="5f088-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f088-110">Properties</span></span>

| <span data-ttu-id="5f088-111">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5f088-111">Property name</span></span>        | <span data-ttu-id="5f088-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f088-112">Type</span></span>                                | <span data-ttu-id="5f088-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f088-113">Description</span></span>                                                                                                                                                       |
| :------------------- | :---------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5f088-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="5f088-114">createdBy</span></span>            | [<span data-ttu-id="5f088-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="5f088-115">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="5f088-p103">Identidade do usuário, dispositivo e aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p103">Identity of the user, device, and application which created the item. Read-only.</span></span>                                                                                  |
| <span data-ttu-id="5f088-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f088-118">createdDateTime</span></span>      | <span data-ttu-id="5f088-119">Timestamp</span><span class="sxs-lookup"><span data-stu-id="5f088-119">Timestamp</span></span>                           | <span data-ttu-id="5f088-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                        |
| <span data-ttu-id="5f088-122">file</span><span class="sxs-lookup"><span data-stu-id="5f088-122">file</span></span>                 | [<span data-ttu-id="5f088-123">File</span><span class="sxs-lookup"><span data-stu-id="5f088-123">File</span></span>](file.md)                     | <span data-ttu-id="5f088-p105">Indica que o item remoto é um arquivo. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p105">Indicates that the remote item is a file. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="5f088-126">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="5f088-126">fileSystemInfo</span></span>       | [<span data-ttu-id="5f088-127">FileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="5f088-127">FileSystemInfo</span></span>](filesysteminfo.md) | <span data-ttu-id="5f088-p106">Informações sobre o item remoto do sistema de arquivos local. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p106">Information about the remote item from the local file system. Read-only.</span></span>                                                                                          |
| <span data-ttu-id="5f088-130">folder</span><span class="sxs-lookup"><span data-stu-id="5f088-130">folder</span></span>               | [<span data-ttu-id="5f088-131">Folder</span><span class="sxs-lookup"><span data-stu-id="5f088-131">Folder</span></span>](folder.md)                 | <span data-ttu-id="5f088-p107">Indica que o item remoto é uma pasta. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p107">Indicates that the remote item is a folder. Read-only.</span></span>                                                                                                            |
| <span data-ttu-id="5f088-134">id</span><span class="sxs-lookup"><span data-stu-id="5f088-134">id</span></span>                   | <span data-ttu-id="5f088-135">String</span><span class="sxs-lookup"><span data-stu-id="5f088-135">String</span></span>                              | <span data-ttu-id="5f088-p108">Identificador exclusivo do item remoto em sua unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p108">Unique identifier for the remote item in its drive. Read-only.</span></span>                                                                                                    |
| <span data-ttu-id="5f088-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5f088-138">lastModifiedBy</span></span>       | [<span data-ttu-id="5f088-139">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="5f088-139">IdentitySet</span></span>](identityset.md)       | <span data-ttu-id="5f088-p109">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p109">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                            |
| <span data-ttu-id="5f088-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f088-142">lastModifiedDateTime</span></span> | <span data-ttu-id="5f088-143">Timestamp</span><span class="sxs-lookup"><span data-stu-id="5f088-143">Timestamp</span></span>                           | <span data-ttu-id="5f088-p110">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p110">Date and time the item was last modified. Read-only.</span></span>                                                                                                              |
| <span data-ttu-id="5f088-146">name</span><span class="sxs-lookup"><span data-stu-id="5f088-146">name</span></span>                 | <span data-ttu-id="5f088-147">String</span><span class="sxs-lookup"><span data-stu-id="5f088-147">String</span></span>                              | <span data-ttu-id="5f088-p111">Opcional. Nome de arquivo do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p111">Optional. Filename of the remote item. Read-only.</span></span>                                                                                                                 |
| <span data-ttu-id="5f088-151">pacote</span><span class="sxs-lookup"><span data-stu-id="5f088-151">package</span></span>              | [<span data-ttu-id="5f088-152">Pacote</span><span class="sxs-lookup"><span data-stu-id="5f088-152">Package</span></span>](package.md)               | <span data-ttu-id="5f088-p112">Se presente, indica que esse item é um pacote, e não uma pasta ou um arquivo. Pacotes são tratados como arquivos em alguns contextos e como pastas em outros. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p112">If present, indicates that this item is a package instead of a folder or file. Packages are treated like files in some contexts and folders in others. Read-only.</span></span> |
| <span data-ttu-id="5f088-156">parentReference</span><span class="sxs-lookup"><span data-stu-id="5f088-156">parentReference</span></span>      | [<span data-ttu-id="5f088-157">ItemReference</span><span class="sxs-lookup"><span data-stu-id="5f088-157">ItemReference</span></span>](itemreference.md)   | <span data-ttu-id="5f088-p113">Propriedades do pai do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p113">Properties of the parent of the remote item. Read-only.</span></span>                                                                                                           |
| <span data-ttu-id="5f088-160">shared</span><span class="sxs-lookup"><span data-stu-id="5f088-160">shared</span></span>               | [<span data-ttu-id="5f088-161">shared</span><span class="sxs-lookup"><span data-stu-id="5f088-161">shared</span></span>](shared.md)                 | <span data-ttu-id="5f088-p114">Indica que o item foi compartilhado com outras pessoas e fornece informações sobre o estado compartilhado desse item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p114">Indicates that the item has been shared with others and provides information about the shared state of the item. Read-only.</span></span>                                       |
| <span data-ttu-id="5f088-164">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="5f088-164">sharepointIds</span></span>        | [<span data-ttu-id="5f088-165">SharepointIds</span><span class="sxs-lookup"><span data-stu-id="5f088-165">SharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="5f088-p115">Fornece interoperabilidade entre itens no OneDrive for Business e no SharePoint com o conjunto completo de identificadores de item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p115">Provides interop between items in OneDrive for Business and SharePoint with the full set of item identifiers. Read-only.</span></span>                                          |
| <span data-ttu-id="5f088-168">size</span><span class="sxs-lookup"><span data-stu-id="5f088-168">size</span></span>                 | <span data-ttu-id="5f088-169">Int64</span><span class="sxs-lookup"><span data-stu-id="5f088-169">Int64</span></span>                               | <span data-ttu-id="5f088-p116">Tamanho do item remoto. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p116">Size of the remote item. Read-only.</span></span>                                                                                                                               |
| <span data-ttu-id="5f088-172">webDavUrl</span><span class="sxs-lookup"><span data-stu-id="5f088-172">webDavUrl</span></span>            | <span data-ttu-id="5f088-173">URL</span><span class="sxs-lookup"><span data-stu-id="5f088-173">Url</span></span>                                 | <span data-ttu-id="5f088-174">URL compatível com DAV para o item.</span><span class="sxs-lookup"><span data-stu-id="5f088-174">DAV compatible URL for the item.</span></span>                                                                                                                                  |
| <span data-ttu-id="5f088-175">webUrl</span><span class="sxs-lookup"><span data-stu-id="5f088-175">webUrl</span></span>               | <span data-ttu-id="5f088-176">URL</span><span class="sxs-lookup"><span data-stu-id="5f088-176">Url</span></span>                                 | <span data-ttu-id="5f088-p117">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f088-p117">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                         |

## <a name="remarks"></a><span data-ttu-id="5f088-179">Comentários</span><span class="sxs-lookup"><span data-stu-id="5f088-179">Remarks</span></span>

<span data-ttu-id="5f088-180">Para saber mais sobre as facetas de um **driveItem**, confira [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="5f088-180">For more information about the facets on a **driveItem**, see [driveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/RemoteItem"
} -->
