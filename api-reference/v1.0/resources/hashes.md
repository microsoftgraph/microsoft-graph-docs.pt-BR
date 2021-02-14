---
author: JeremyKelley
ms.date: 09/10/2017
localization_priority: Normal
title: Tipo de recurso de hashes
description: O recurso hash agrupa hashes disponíveis em uma estrutura simples para um item.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b45d872966bc8eba3ef3d622b5b0e37c83122b6
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240000"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="85dbd-103">Tipo de recurso de hashes</span><span class="sxs-lookup"><span data-stu-id="85dbd-103">Hashes resource type</span></span>

<span data-ttu-id="85dbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85dbd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85dbd-105">O recurso **hash** agrupa hashes disponíveis em uma estrutura simples para um item.</span><span class="sxs-lookup"><span data-stu-id="85dbd-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="85dbd-106">**Observação:** Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="85dbd-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85dbd-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85dbd-107">JSON representation</span></span>

<span data-ttu-id="85dbd-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85dbd-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="85dbd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85dbd-109">Properties</span></span>

| <span data-ttu-id="85dbd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85dbd-110">Property</span></span>         | <span data-ttu-id="85dbd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="85dbd-111">Type</span></span>   | <span data-ttu-id="85dbd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="85dbd-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="85dbd-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="85dbd-113">**sha1Hash**</span></span>     | <span data-ttu-id="85dbd-114">String</span><span class="sxs-lookup"><span data-stu-id="85dbd-114">String</span></span> | <span data-ttu-id="85dbd-p101">Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85dbd-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="85dbd-117">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="85dbd-117">**sha256Hash**</span></span>   | <span data-ttu-id="85dbd-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85dbd-118">String</span></span> | <span data-ttu-id="85dbd-119">Hash SHA256 para o conteúdo do arquivo (se disponível).</span><span class="sxs-lookup"><span data-stu-id="85dbd-119">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="85dbd-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85dbd-120">Read-only.</span></span> |
| <span data-ttu-id="85dbd-121">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="85dbd-121">**crc32Hash**</span></span>    | <span data-ttu-id="85dbd-122">String</span><span class="sxs-lookup"><span data-stu-id="85dbd-122">String</span></span> | <span data-ttu-id="85dbd-123">O valor CRC32 do arquivo em pouco endian (se disponível).</span><span class="sxs-lookup"><span data-stu-id="85dbd-123">The CRC32 value of the file in little endian (if available).</span></span> <span data-ttu-id="85dbd-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85dbd-124">Read-only.</span></span>            |
| <span data-ttu-id="85dbd-125">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="85dbd-125">**quickXorHash**</span></span> | <span data-ttu-id="85dbd-126">String</span><span class="sxs-lookup"><span data-stu-id="85dbd-126">String</span></span> | <span data-ttu-id="85dbd-p104">Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85dbd-p104">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="85dbd-p105">**Observação:** Em alguns casos, os valores de hash podem não estar disponíveis. Nesse caso, os valores de hash em um item serão atualizados depois que o item for baixado.</span><span class="sxs-lookup"><span data-stu-id="85dbd-p105">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="85dbd-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="85dbd-131">Remarks</span></span>

<span data-ttu-id="85dbd-132">No OneDrive for Business e no SharePoint Server 2016, **sha1Hash** e **crc32Hash** e **sha256Hash** não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="85dbd-132">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash**, and **sha256Hash** are not available.</span></span>

<span data-ttu-id="85dbd-133">No OneDrive Personal, o **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="85dbd-133">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="85dbd-134">Para calcular o **quickXorHash** de um arquivo, consulte o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="85dbd-134">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="85dbd-135">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="85dbd-135">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->

