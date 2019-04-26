---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Hashes
localization_priority: Normal
ms.openlocfilehash: 8b2a80152a0e4e4ec2b05a4ea1080ff4e159d6c9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333683"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="39a6f-102">Tipo de recurso de hashes</span><span class="sxs-lookup"><span data-stu-id="39a6f-102">Hashes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39a6f-103">O recurso **hash** agrupa hashes disponíveis em uma estrutura simples para um item.</span><span class="sxs-lookup"><span data-stu-id="39a6f-103">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="39a6f-104">**Observação:** Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="39a6f-104">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39a6f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39a6f-105">JSON representation</span></span>

<span data-ttu-id="39a6f-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39a6f-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="39a6f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39a6f-107">Properties</span></span>

| <span data-ttu-id="39a6f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39a6f-108">Property</span></span>         | <span data-ttu-id="39a6f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="39a6f-109">Type</span></span>   | <span data-ttu-id="39a6f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39a6f-110">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="39a6f-111">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="39a6f-111">**sha1Hash**</span></span>     | <span data-ttu-id="39a6f-112">String</span><span class="sxs-lookup"><span data-stu-id="39a6f-112">String</span></span> | <span data-ttu-id="39a6f-p101">Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="39a6f-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="39a6f-115">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="39a6f-115">**crc32Hash**</span></span>    | <span data-ttu-id="39a6f-116">String</span><span class="sxs-lookup"><span data-stu-id="39a6f-116">String</span></span> | <span data-ttu-id="39a6f-p102">O valor de CRC32 do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="39a6f-p102">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="39a6f-119">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="39a6f-119">**quickXorHash**</span></span> | <span data-ttu-id="39a6f-120">String</span><span class="sxs-lookup"><span data-stu-id="39a6f-120">String</span></span> | <span data-ttu-id="39a6f-p103">Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="39a6f-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="39a6f-p104">**Observação:** Em alguns casos, os valores de hash podem não estar disponíveis. Nesse caso, os valores de hash em um item serão atualizados depois que o item for baixado.</span><span class="sxs-lookup"><span data-stu-id="39a6f-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="39a6f-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="39a6f-125">Remarks</span></span>

<span data-ttu-id="39a6f-126">No OneDrive for Business e no SharePoint Server 2016, **sha1Hash** e **crc32Hash** não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="39a6f-126">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="39a6f-127">No OneDrive Personal, o **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="39a6f-127">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="39a6f-128">Para calcular o **quickXorHash** de um arquivo, consulte o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="39a6f-128">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="39a6f-129">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="39a6f-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
