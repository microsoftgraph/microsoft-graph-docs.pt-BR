---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Tipo de recurso de hashes
description: O recurso hash agrupa hashes disponíveis em uma estrutura simples para um item.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cb852ad01394ac463cb3d23ed404a7956bbf1eea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532907"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="b1fb9-103">Tipo de recurso de hashes</span><span class="sxs-lookup"><span data-stu-id="b1fb9-103">Hashes resource type</span></span>

<span data-ttu-id="b1fb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1fb9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1fb9-105">O recurso **hash** agrupa hashes disponíveis em uma estrutura simples para um item.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="b1fb9-106">**Observação:** Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1fb9-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1fb9-107">JSON representation</span></span>

<span data-ttu-id="b1fb9-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a><span data-ttu-id="b1fb9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1fb9-109">Properties</span></span>

| <span data-ttu-id="b1fb9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1fb9-110">Property</span></span>         | <span data-ttu-id="b1fb9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1fb9-111">Type</span></span>   | <span data-ttu-id="b1fb9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1fb9-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="b1fb9-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="b1fb9-113">**sha1Hash**</span></span>     | <span data-ttu-id="b1fb9-114">String</span><span class="sxs-lookup"><span data-stu-id="b1fb9-114">String</span></span> | <span data-ttu-id="b1fb9-p101">Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="b1fb9-117">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="b1fb9-117">**crc32Hash**</span></span>    | <span data-ttu-id="b1fb9-118">String</span><span class="sxs-lookup"><span data-stu-id="b1fb9-118">String</span></span> | <span data-ttu-id="b1fb9-119">O valor CRC32 do arquivo em little endian (se disponível).</span><span class="sxs-lookup"><span data-stu-id="b1fb9-119">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="b1fb9-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-120">Read-only.</span></span>            |
| <span data-ttu-id="b1fb9-121">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="b1fb9-121">**quickXorHash**</span></span> | <span data-ttu-id="b1fb9-122">String</span><span class="sxs-lookup"><span data-stu-id="b1fb9-122">String</span></span> | <span data-ttu-id="b1fb9-p103">Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="b1fb9-p104">**Observação:** Em alguns casos, os valores de hash podem não estar disponíveis. Nesse caso, os valores de hash em um item serão atualizados depois que o item for baixado.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="b1fb9-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="b1fb9-127">Remarks</span></span>

<span data-ttu-id="b1fb9-128">No OneDrive for Business e no SharePoint Server 2016, **sha1Hash** e **crc32Hash** não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-128">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="b1fb9-129">No OneDrive Personal, o **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="b1fb9-129">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="b1fb9-130">Para calcular o **quickXorHash** de um arquivo, consulte o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="b1fb9-130">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="b1fb9-131">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b1fb9-131">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
