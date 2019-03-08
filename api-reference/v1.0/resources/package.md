---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Pacote
localization_priority: Normal
ms.openlocfilehash: c64dfce910456ef9b9415e3332c099d7814a71f2
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482200"
---
# <a name="package-resource-type"></a><span data-ttu-id="ed6f1-102">Tipo de recurso Package</span><span class="sxs-lookup"><span data-stu-id="ed6f1-102">Package resource type</span></span>

<span data-ttu-id="ed6f1-103">O recurso **Package** indica que um DriveItem é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção, em vez de itens individuais.</span><span class="sxs-lookup"><span data-stu-id="ed6f1-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="ed6f1-p101">Um exemplo de um pacote é um bloco de anotações do OneNote. Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **package** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.</span><span class="sxs-lookup"><span data-stu-id="ed6f1-p101">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="ed6f1-106">DriveItems com a faceta **package** não incluem uma faceta **folder** ou **file**, mas são conceitualmente semelhantes a um item com uma faceta **folder**.</span><span class="sxs-lookup"><span data-stu-id="ed6f1-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed6f1-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed6f1-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

## <a name="properties"></a><span data-ttu-id="ed6f1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed6f1-108">Properties</span></span>

| <span data-ttu-id="ed6f1-109">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed6f1-109">Property Name</span></span> | <span data-ttu-id="ed6f1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed6f1-110">Type</span></span>   | <span data-ttu-id="ed6f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed6f1-111">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ed6f1-112">type</span><span class="sxs-lookup"><span data-stu-id="ed6f1-112">type</span></span>          | <span data-ttu-id="ed6f1-113">string</span><span class="sxs-lookup"><span data-stu-id="ed6f1-113">string</span></span> | <span data-ttu-id="ed6f1-114">Uma cadeia de caracteres indicando o tipo de pacote.</span><span class="sxs-lookup"><span data-stu-id="ed6f1-114">A string indicating the type of package.</span></span> <span data-ttu-id="ed6f1-115">Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada.</span><span class="sxs-lookup"><span data-stu-id="ed6f1-115">While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="ed6f1-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="ed6f1-116">Remarks</span></span> 

<span data-ttu-id="ed6f1-117">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ed6f1-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
