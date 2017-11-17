---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Pacote
ms.openlocfilehash: 33be73ed79438bdf28b76747b6efb79290be8d0c
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="package-resource-type"></a><span data-ttu-id="3d716-102">Tipo de recurso de pacote</span><span class="sxs-lookup"><span data-stu-id="3d716-102">Package resource type</span></span>

<span data-ttu-id="3d716-103">O recurso **Package** indica que um DriveItem é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção, em vez de itens individuais.</span><span class="sxs-lookup"><span data-stu-id="3d716-103">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="3d716-104">Um exemplo de um pacote é um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="3d716-104">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="3d716-105">Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **package** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.</span><span class="sxs-lookup"><span data-stu-id="3d716-105">An example of a package is a OneNote notebook. While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="3d716-106">DriveItems com a faceta **package** não incluem uma faceta **folder** ou **file**, mas são conceitualmente semelhantes a um item com uma faceta **folder**.</span><span class="sxs-lookup"><span data-stu-id="3d716-106">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d716-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d716-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="3d716-108">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d716-108">Property Name</span></span> | <span data-ttu-id="3d716-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d716-109">Type</span></span>   | <span data-ttu-id="3d716-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d716-110">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3d716-111">**type**</span><span class="sxs-lookup"><span data-stu-id="3d716-111">**type**</span></span>      | <span data-ttu-id="3d716-112">string</span><span class="sxs-lookup"><span data-stu-id="3d716-112">string</span></span> | <span data-ttu-id="3d716-p102">Uma cadeia de caracteres indicando o tipo de pacote. Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada.</span><span class="sxs-lookup"><span data-stu-id="3d716-p102">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="3d716-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="3d716-115">Remarks</span></span> 

<span data-ttu-id="3d716-116">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3d716-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation",
  "tocPath": "Facets/Package"
} -->
