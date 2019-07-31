---
author: JeremyKelley
description: " ou uma coleção de itens que deve ser tratada como uma coleção em vez de itens individuais."
ms.date: 09/10/2017
title: Packager
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6ae382d1f69a88d814339370264dc5dc7fac9414
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966262"
---
# <a name="package-resource-type"></a><span data-ttu-id="c6bbb-103">Tipo de recurso Package</span><span class="sxs-lookup"><span data-stu-id="c6bbb-103">Package resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6bbb-104">O recurso **Package** indica que um DriveItem é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção, em vez de itens individuais.</span><span class="sxs-lookup"><span data-stu-id="c6bbb-104">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="c6bbb-p101">Um exemplo de um pacote é um bloco de anotações do OneNote. Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **package** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.</span><span class="sxs-lookup"><span data-stu-id="c6bbb-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="c6bbb-107">DriveItems com a faceta **package** não incluem uma faceta **folder** ou **file**, mas são conceitualmente semelhantes a um item com uma faceta **folder**.</span><span class="sxs-lookup"><span data-stu-id="c6bbb-107">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6bbb-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6bbb-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="c6bbb-109">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6bbb-109">Property Name</span></span> | <span data-ttu-id="c6bbb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6bbb-110">Type</span></span>   | <span data-ttu-id="c6bbb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6bbb-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c6bbb-112">**type**</span><span class="sxs-lookup"><span data-stu-id="c6bbb-112">**type**</span></span>      | <span data-ttu-id="c6bbb-113">string</span><span class="sxs-lookup"><span data-stu-id="c6bbb-113">string</span></span> | <span data-ttu-id="c6bbb-p102">Uma cadeia de caracteres indicando o tipo de pacote. Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada.</span><span class="sxs-lookup"><span data-stu-id="c6bbb-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="c6bbb-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="c6bbb-116">Remarks</span></span> 

<span data-ttu-id="c6bbb-117">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c6bbb-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "suppressions": []
}
-->
