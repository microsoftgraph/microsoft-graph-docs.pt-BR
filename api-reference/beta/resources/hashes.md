---
author: JeremyKelley
description: O recurso hash agrupa hashes disponíveis em uma estrutura única para um item.
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 985efa857fdf9aaa254884e04bfccf1d780d5b8c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496926"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="7b8c3-103">tipo de recurso hashes</span><span class="sxs-lookup"><span data-stu-id="7b8c3-103">hashes resource type</span></span>

<span data-ttu-id="7b8c3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7b8c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b8c3-105">Agrupa hashes disponíveis em uma estrutura única para um item.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-105">Groups available hashes into a single structure for an item.</span></span>

> [!NOTE]
> <span data-ttu-id="7b8c3-106">Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-106">Not all services provide a value for all hash properties listed.</span></span> <span data-ttu-id="7b8c3-107">No OneDrive for Business e no SharePoint Server 2016, **sha1Hash**, **crc32Hash**e **sha256Hash** não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-107">In OneDrive for Business and SharePoint Server 2016, **sha1Hash**, **crc32Hash**, and **sha256Hash** are not available.</span></span> <span data-ttu-id="7b8c3-108">No OneDrive Personal, o **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-108">In OneDrive Personal, **quickXorHash** is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="7b8c3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b8c3-109">Properties</span></span>

| <span data-ttu-id="7b8c3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b8c3-110">Property</span></span>         | <span data-ttu-id="7b8c3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b8c3-111">Type</span></span>   | <span data-ttu-id="7b8c3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b8c3-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="7b8c3-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="7b8c3-113">**sha1Hash**</span></span>     | <span data-ttu-id="7b8c3-114">String</span><span class="sxs-lookup"><span data-stu-id="7b8c3-114">String</span></span> | <span data-ttu-id="7b8c3-p102">Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="7b8c3-117">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="7b8c3-117">**sha256Hash**</span></span>   | <span data-ttu-id="7b8c3-118">String</span><span class="sxs-lookup"><span data-stu-id="7b8c3-118">String</span></span> | <span data-ttu-id="7b8c3-119">O hash SHA256 para o conteúdo do arquivo (se disponível).</span><span class="sxs-lookup"><span data-stu-id="7b8c3-119">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="7b8c3-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-120">Read-only.</span></span> |
| <span data-ttu-id="7b8c3-121">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="7b8c3-121">**crc32Hash**</span></span>    | <span data-ttu-id="7b8c3-122">String</span><span class="sxs-lookup"><span data-stu-id="7b8c3-122">String</span></span> | <span data-ttu-id="7b8c3-p104">O valor de CRC32 do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-p104">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="7b8c3-125">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="7b8c3-125">**quickXorHash**</span></span> | <span data-ttu-id="7b8c3-126">String</span><span class="sxs-lookup"><span data-stu-id="7b8c3-126">String</span></span> | <span data-ttu-id="7b8c3-p105">Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-p105">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

> <span data-ttu-id="7b8c3-129">**Observação:** Nos casos em que os valores de hash não estiverem disponíveis, os valores de hash em um item serão atualizados após o download do item.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-129">**Note:** In cases where the hash values are not available, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b8c3-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b8c3-130">JSON representation</span></span>

<span data-ttu-id="7b8c3-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b8c3-131">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7b8c3-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="7b8c3-132">See also</span></span>

- <span data-ttu-id="7b8c3-133">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7b8c3-133">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
- <span data-ttu-id="7b8c3-134">Para calcular o **quickXorHash** de um arquivo, confira o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="7b8c3-134">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes",
  "suppressions": []
}
-->
