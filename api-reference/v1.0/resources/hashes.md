---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Tipo de recurso de hashes
description: O recurso hash agrupa hashes disponíveis em uma estrutura simples para um item.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: da326576b148fdaee79ebfc3df2d7832bfeee4e5
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863737"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="903b3-103">Tipo de recurso de hashes</span><span class="sxs-lookup"><span data-stu-id="903b3-103">Hashes resource type</span></span>

<span data-ttu-id="903b3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="903b3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="903b3-105">O recurso **hash** agrupa hashes disponíveis em uma estrutura simples para um item.</span><span class="sxs-lookup"><span data-stu-id="903b3-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="903b3-106">**Observação:** Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="903b3-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="903b3-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="903b3-107">JSON representation</span></span>

<span data-ttu-id="903b3-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="903b3-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "sha1Hash", "crc32Hash", "quickXorHash" ],
  "@odata.type": "microsoft.graph.hashes"
}-->

```json
{
  "crc32Hash": "string (hex)",
  "sha1Hash": "string (hex)",
  "sha256Hash": "string (hex)",
  "quickXorHash": "string (base64)"
}
```

## <a name="properties"></a><span data-ttu-id="903b3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="903b3-109">Properties</span></span>

| <span data-ttu-id="903b3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="903b3-110">Property</span></span>         | <span data-ttu-id="903b3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="903b3-111">Type</span></span>   | <span data-ttu-id="903b3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="903b3-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="903b3-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="903b3-113">**sha1Hash**</span></span>     | <span data-ttu-id="903b3-114">String</span><span class="sxs-lookup"><span data-stu-id="903b3-114">String</span></span> | <span data-ttu-id="903b3-115">SHA1 hash for the contents of the file (if available).</span><span class="sxs-lookup"><span data-stu-id="903b3-115">SHA1 hash for the contents of the file (if available).</span></span> <span data-ttu-id="903b3-116">Read-only.</span><span class="sxs-lookup"><span data-stu-id="903b3-116">Read-only.</span></span> |
| <span data-ttu-id="903b3-117">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="903b3-117">**sha256Hash**</span></span>   | <span data-ttu-id="903b3-118">String</span><span class="sxs-lookup"><span data-stu-id="903b3-118">String</span></span> | <span data-ttu-id="903b3-119">O hash SHA256 para o conteúdo do arquivo (se disponível).</span><span class="sxs-lookup"><span data-stu-id="903b3-119">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="903b3-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="903b3-120">Read-only.</span></span> |
| <span data-ttu-id="903b3-121">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="903b3-121">**crc32Hash**</span></span>    | <span data-ttu-id="903b3-122">String</span><span class="sxs-lookup"><span data-stu-id="903b3-122">String</span></span> | <span data-ttu-id="903b3-123">O valor CRC32 do arquivo em little endian (se disponível).</span><span class="sxs-lookup"><span data-stu-id="903b3-123">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="903b3-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="903b3-124">Read-only.</span></span>            |
| <span data-ttu-id="903b3-125">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="903b3-125">**quickXorHash**</span></span> | <span data-ttu-id="903b3-126">String</span><span class="sxs-lookup"><span data-stu-id="903b3-126">String</span></span> | <span data-ttu-id="903b3-127">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available).</span><span class="sxs-lookup"><span data-stu-id="903b3-127">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available).</span></span> <span data-ttu-id="903b3-128">Read-only.</span><span class="sxs-lookup"><span data-stu-id="903b3-128">Read-only.</span></span> |

<span data-ttu-id="903b3-129">**Note:** In some cases hash values may not be available.</span><span class="sxs-lookup"><span data-stu-id="903b3-129">**Note:** In some cases hash values may not be available.</span></span> <span data-ttu-id="903b3-130">If this is the case, the hash values on an item will be updated after the item is downloaded.</span><span class="sxs-lookup"><span data-stu-id="903b3-130">If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="903b3-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="903b3-131">Remarks</span></span>

<span data-ttu-id="903b3-132">No OneDrive for Business e no SharePoint Server 2016, **sha1Hash** e **crc32Hash**e **sha256Hash** não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="903b3-132">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash**, and **sha256Hash** are not available.</span></span>

<span data-ttu-id="903b3-133">No OneDrive Personal, o **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="903b3-133">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="903b3-134">Para calcular o **quickXorHash** de um arquivo, consulte o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="903b3-134">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="903b3-135">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="903b3-135">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
