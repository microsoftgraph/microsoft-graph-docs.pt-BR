---
author: JeremyKelley
description: O recurso hash agrupa hashes disponíveis em uma estrutura única para um item.
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b620170cf05e8e04cb4368874ea20d29c5440298
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333245"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="0c77e-103">tipo de recurso hashes</span><span class="sxs-lookup"><span data-stu-id="0c77e-103">hashes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c77e-104">Agrupa hashes disponíveis em uma estrutura única para um item.</span><span class="sxs-lookup"><span data-stu-id="0c77e-104">Groups available hashes into a single structure for an item.</span></span>

> [!NOTE]
> <span data-ttu-id="0c77e-105">Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="0c77e-105">Not all services provide a value for all hash properties listed.</span></span> <span data-ttu-id="0c77e-106">No OneDrive for Business e no SharePoint Server 2016, **sha1Hash**, **crc32Hash**e **sha256Hash** não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="0c77e-106">In OneDrive for Business and SharePoint Server 2016, **sha1Hash**, **crc32Hash**, and **sha256Hash** are not available.</span></span> <span data-ttu-id="0c77e-107">No OneDrive Personal, o **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="0c77e-107">In OneDrive Personal, **quickXorHash** is not available.</span></span>

## <a name="properties"></a><span data-ttu-id="0c77e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c77e-108">Properties</span></span>

| <span data-ttu-id="0c77e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c77e-109">Property</span></span>         | <span data-ttu-id="0c77e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c77e-110">Type</span></span>   | <span data-ttu-id="0c77e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c77e-111">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="0c77e-112">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="0c77e-112">**sha1Hash**</span></span>     | <span data-ttu-id="0c77e-113">String</span><span class="sxs-lookup"><span data-stu-id="0c77e-113">String</span></span> | <span data-ttu-id="0c77e-p102">Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c77e-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="0c77e-116">**sha256Hash**</span><span class="sxs-lookup"><span data-stu-id="0c77e-116">**sha256Hash**</span></span>   | <span data-ttu-id="0c77e-117">String</span><span class="sxs-lookup"><span data-stu-id="0c77e-117">String</span></span> | <span data-ttu-id="0c77e-118">O hash SHA256 para o conteúdo do arquivo (se disponível).</span><span class="sxs-lookup"><span data-stu-id="0c77e-118">SHA256 hash for the contents of the file (if available).</span></span> <span data-ttu-id="0c77e-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c77e-119">Read-only.</span></span> |
| <span data-ttu-id="0c77e-120">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="0c77e-120">**crc32Hash**</span></span>    | <span data-ttu-id="0c77e-121">String</span><span class="sxs-lookup"><span data-stu-id="0c77e-121">String</span></span> | <span data-ttu-id="0c77e-p104">O valor de CRC32 do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c77e-p104">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="0c77e-124">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="0c77e-124">**quickXorHash**</span></span> | <span data-ttu-id="0c77e-125">String</span><span class="sxs-lookup"><span data-stu-id="0c77e-125">String</span></span> | <span data-ttu-id="0c77e-p105">Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c77e-p105">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

> <span data-ttu-id="0c77e-128">**Observação:** Nos casos em que os valores de hash não estiverem disponíveis, os valores de hash em um item serão atualizados após o download do item.</span><span class="sxs-lookup"><span data-stu-id="0c77e-128">**Note:** In cases where the hash values are not available, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c77e-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c77e-129">JSON representation</span></span>

<span data-ttu-id="0c77e-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c77e-130">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="0c77e-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="0c77e-131">See also</span></span>

- <span data-ttu-id="0c77e-132">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0c77e-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>
- <span data-ttu-id="0c77e-133">Para calcular o **quickXorHash** de um arquivo, confira o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="0c77e-133">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>


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
