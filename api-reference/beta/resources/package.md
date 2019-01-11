---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Pacote
localization_priority: Normal
ms.openlocfilehash: ab3d9298b0a03e31a9e33e9c187c1a0af8691cc3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833940"
---
# <a name="package-resource-type"></a><span data-ttu-id="624dc-102">Tipo de recurso Package</span><span class="sxs-lookup"><span data-stu-id="624dc-102">Package resource type</span></span>

> <span data-ttu-id="624dc-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="624dc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="624dc-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="624dc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="624dc-105">O recurso **Package** indica que um DriveItem é o item de nível superior em um "pacote" ou uma coleção de itens que devem ser tratados como uma coleção, em vez de itens individuais.</span><span class="sxs-lookup"><span data-stu-id="624dc-105">The **Package** resource indicates that a DriveItem is the top level item in a "package" or a collection of items that should be treated as a collection instead of individual items.</span></span>

<span data-ttu-id="624dc-106">Um exemplo de um pacote é um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="624dc-106">An example of a package is a OneNote notebook.</span></span> <span data-ttu-id="624dc-107">Embora o bloco de anotações seja composto de arquivos e pastas que representam o conteúdo do bloco de anotações, o item de nível superior que representa o bloco de anotações tem uma faceta **package** para indicar aos clientes que se trata de uma coleção de dados que deve ser tratada de forma especial.</span><span class="sxs-lookup"><span data-stu-id="624dc-107">While the notebook is made up of files and folders that represent the contents of the notebook, the top level item that represents the notebook has a **package** facet to indicate to clients that this is a collection of data that should be treated special.</span></span>

<span data-ttu-id="624dc-108">DriveItems com a faceta **package** não incluem uma faceta **folder** ou **file**, mas são conceitualmente semelhantes a um item com uma faceta **folder**.</span><span class="sxs-lookup"><span data-stu-id="624dc-108">DriveItems with the **package** facet do not include a **folder** or **file** facet but are conceptually similar to an item with a **folder** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="624dc-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="624dc-109">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.package" } -->
```json
{
  "type": "oneNote"
}
```

| <span data-ttu-id="624dc-110">Nome da Propriedade</span><span class="sxs-lookup"><span data-stu-id="624dc-110">Property Name</span></span> | <span data-ttu-id="624dc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="624dc-111">Type</span></span>   | <span data-ttu-id="624dc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="624dc-112">Description</span></span>                                                                                                                                                                      |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="624dc-113">**type**</span><span class="sxs-lookup"><span data-stu-id="624dc-113">**type**</span></span>      | <span data-ttu-id="624dc-114">string</span><span class="sxs-lookup"><span data-stu-id="624dc-114">string</span></span> | <span data-ttu-id="624dc-p103">Uma cadeia de caracteres indicando o tipo de pacote. Embora `oneNote` seja o único valor definido atualmente, você deve esperar que outros tipos de pacote sejam retornados e lidar com eles da forma apropriada.</span><span class="sxs-lookup"><span data-stu-id="624dc-p103">An string indicating the type of package. While `oneNote` is the only currently defined value, you should expect other package types to be returned and handle them accordingly.</span></span> |

## <a name="remarks"></a><span data-ttu-id="624dc-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="624dc-117">Remarks</span></span> 

<span data-ttu-id="624dc-118">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="624dc-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The Package facet indicates that an item is the root of a special collection of items that should be treated as a single unit.",
  "keywords": "package, facet, onenote",
  "section": "documentation"
} -->
