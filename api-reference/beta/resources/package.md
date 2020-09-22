---
author: JeremyKelley
description: " ou uma coleção de itens que deve ser tratada como uma coleção em vez de itens individuais."
ms.date: 09/10/2017
title: Pacote
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 851e2bbe5bbacea6fe988dac1fa72fe32886cec0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998331"
---
# <a name="package-resource-type"></a><span data-ttu-id="b34c3-103">Tipo de recurso Package</span><span class="sxs-lookup"><span data-stu-id="b34c3-103">Package resource type</span></span>

<span data-ttu-id="b34c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b34c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b34c3-105">O recurso **Package** indica que um DriveItem é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção, em vez de itens individuais.</span><span class="sxs-lookup"><span data-stu-id="b34c3-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="b34c3-p101">Um exemplo de um pacote é um bloco de anotações do OneNote. Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **package** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.</span><span class="sxs-lookup"><span data-stu-id="b34c3-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="b34c3-108">DriveItems com a faceta **package** não incluem uma faceta **folder** ou **file**, mas são conceitualmente semelhantes a um item com uma faceta **folder**.</span><span class="sxs-lookup"><span data-stu-id="b34c3-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b34c3-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b34c3-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="b34c3-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b34c3-110">Property Name</span></span> | <span data-ttu-id="b34c3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b34c3-111">Type</span></span>   | <span data-ttu-id="b34c3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b34c3-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b34c3-113">**type**</span><span class="sxs-lookup"><span data-stu-id="b34c3-113">**type**</span></span>      | <span data-ttu-id="b34c3-114">string</span><span class="sxs-lookup"><span data-stu-id="b34c3-114">string</span></span> | <span data-ttu-id="b34c3-p102">Uma cadeia de caracteres indicando o tipo de pacote. Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada.</span><span class="sxs-lookup"><span data-stu-id="b34c3-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="b34c3-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="b34c3-117">Remarks</span></span> 

<span data-ttu-id="b34c3-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b34c3-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": []
}
-->


