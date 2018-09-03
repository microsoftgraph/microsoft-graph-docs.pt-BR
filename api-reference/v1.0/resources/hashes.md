---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.openlocfilehash: 92882910ecf86d19e1f0a8a5767d148f5aa95775
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264032"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="00411-101">Tipo de recurso de hashes</span><span class="sxs-lookup"><span data-stu-id="00411-101">Hashes resource type</span></span>

<span data-ttu-id="00411-102">O recurso **hash** agrupa hashes disponíveis em uma estrutura simples para um item.</span><span class="sxs-lookup"><span data-stu-id="00411-102">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="00411-103">**Observação:** Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="00411-103">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="00411-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00411-104">JSON representation</span></span>

<span data-ttu-id="00411-105">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00411-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="00411-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00411-106">Properties</span></span>

| <span data-ttu-id="00411-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00411-107">Property</span></span>         | <span data-ttu-id="00411-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="00411-108">Type</span></span>   | <span data-ttu-id="00411-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="00411-109">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="00411-110">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="00411-110">**sha1Hash**</span></span>     | <span data-ttu-id="00411-111">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="00411-111">String</span></span> | <span data-ttu-id="00411-p101">Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00411-p101">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="00411-114">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="00411-114">**crc32Hash**</span></span>    | <span data-ttu-id="00411-115">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="00411-115">String</span></span> | <span data-ttu-id="00411-116">O valor de CRC32 do arquivo em little endian (se disponível).</span><span class="sxs-lookup"><span data-stu-id="00411-116">The CRC32 value of the file (if available). Read-only.</span></span> <span data-ttu-id="00411-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00411-117">Read-only.</span></span>            |
| <span data-ttu-id="00411-118">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="00411-118">**quickXorHash**</span></span> | <span data-ttu-id="00411-119">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="00411-119">String</span></span> | <span data-ttu-id="00411-p103">Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="00411-p103">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="00411-p104">**Observação:** Em alguns casos, os valores de hash podem não estar disponíveis. Nesse caso, os valores de hash em um item serão atualizados depois que o item for baixado.</span><span class="sxs-lookup"><span data-stu-id="00411-p104">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="00411-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="00411-124">Remarks</span></span>

<span data-ttu-id="00411-125">No OneDrive for Business e no SharePoint Server 2016, **sha1Hash** e **crc32Hash** não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="00411-125">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="00411-126">No OneDrive Personal, o **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="00411-126">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="00411-127">Para calcular o **quickXorHash** de um arquivo, consulte o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="00411-127">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>
<span data-ttu-id="00411-128">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="00411-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
