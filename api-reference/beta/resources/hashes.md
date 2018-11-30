---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Hashes
ms.openlocfilehash: 2387af83450f667aa4732cc46d7d3cf2111579f0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033437"
---
# <a name="hashes-resource-type"></a><span data-ttu-id="c6d46-102">Tipo de recurso de hashes</span><span class="sxs-lookup"><span data-stu-id="c6d46-102">Hashes resource type</span></span>

> <span data-ttu-id="c6d46-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c6d46-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6d46-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c6d46-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6d46-105">O recurso **hash** agrupa hashes disponíveis em uma estrutura simples para um item.</span><span class="sxs-lookup"><span data-stu-id="c6d46-105">The **Hashes** resource groups available hashes into a single structure for an item.</span></span>

<span data-ttu-id="c6d46-106">**Observação:** Nem todos os serviços fornecem um valor para todas as propriedades de hash listadas.</span><span class="sxs-lookup"><span data-stu-id="c6d46-106">**Note:** Not all services provide a value for all hash properties listed.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6d46-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6d46-107">JSON representation</span></span>

<span data-ttu-id="c6d46-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c6d46-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="c6d46-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6d46-109">Properties</span></span>

| <span data-ttu-id="c6d46-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6d46-110">Property</span></span>         | <span data-ttu-id="c6d46-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6d46-111">Type</span></span>   | <span data-ttu-id="c6d46-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6d46-112">Description</span></span>                                                       |
|:-----------------|:-------|:------------------------------------------------------------------|
| <span data-ttu-id="c6d46-113">**sha1Hash**</span><span class="sxs-lookup"><span data-stu-id="c6d46-113">**sha1Hash**</span></span>     | <span data-ttu-id="c6d46-114">String</span><span class="sxs-lookup"><span data-stu-id="c6d46-114">String</span></span> | <span data-ttu-id="c6d46-p102">Hash SHA1 para o conteúdo do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c6d46-p102">SHA1 hash for the contents of the file (if available). Read-only.</span></span> |
| <span data-ttu-id="c6d46-117">**crc32Hash**</span><span class="sxs-lookup"><span data-stu-id="c6d46-117">**crc32Hash**</span></span>    | <span data-ttu-id="c6d46-118">String</span><span class="sxs-lookup"><span data-stu-id="c6d46-118">String</span></span> | <span data-ttu-id="c6d46-p103">O valor de CRC32 do arquivo (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c6d46-p103">The CRC32 value of the file (if available). Read-only.</span></span>            |
| <span data-ttu-id="c6d46-121">**quickXorHash**</span><span class="sxs-lookup"><span data-stu-id="c6d46-121">**quickXorHash**</span></span> | <span data-ttu-id="c6d46-122">String</span><span class="sxs-lookup"><span data-stu-id="c6d46-122">String</span></span> | <span data-ttu-id="c6d46-p104">Um hash de proprietário do arquivo que pode ser usado para determinar se o conteúdo do arquivo foi alterado (se disponível). Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c6d46-p104">A proprietary hash of the file that can be used to determine if the contents of the file have changed (if available). Read-only.</span></span> |

<span data-ttu-id="c6d46-p105">**Observação:** Em alguns casos, os valores de hash podem não estar disponíveis. Nesse caso, os valores de hash em um item serão atualizados depois que o item for baixado.</span><span class="sxs-lookup"><span data-stu-id="c6d46-p105">**Note:** In some cases hash values may not be available. If this is the case, the hash values on an item will be updated after the item is downloaded.</span></span>

## <a name="remarks"></a><span data-ttu-id="c6d46-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="c6d46-127">Remarks</span></span>

<span data-ttu-id="c6d46-128">No OneDrive for Business e no SharePoint Server 2016, **sha1Hash** e **crc32Hash** não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c6d46-128">In OneDrive for Business and SharePoint Server 2016, **sha1Hash** and **crc32Hash** are not available.</span></span>

<span data-ttu-id="c6d46-129">No OneDrive Personal, o **quickXorHash** não está disponível.</span><span class="sxs-lookup"><span data-stu-id="c6d46-129">In OneDrive Personal, **quickXorHash** is not available.</span></span>

<span data-ttu-id="c6d46-130">Para calcular o **quickXorHash** de um arquivo, consulte o [trecho de código QuickXorHash](https://dev.onedrive.com/snippets/quickxorhash.htm).</span><span class="sxs-lookup"><span data-stu-id="c6d46-130">To calculate **quickXorHash** for a file, refer to the [QuickXorHash snippet](https://dev.onedrive.com/snippets/quickxorhash.htm).</span></span>

<span data-ttu-id="c6d46-131">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c6d46-131">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The hashes facet provides hash identifiers for a file in OneDrive",
  "keywords": "hash,sha1,crc32,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Hashes"
} -->
