---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: SystemFacet
localization_priority: Normal
ms.openlocfilehash: afafb69e9d887d2cb8d9537dd7ef9d3a712f3333
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553936"
---
# <a name="system-facet"></a><span data-ttu-id="02128-102">Faceta System</span><span class="sxs-lookup"><span data-stu-id="02128-102">System facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02128-103">A faceta **System** indica que o objeto é gerenciado pelo sistema para sua própria operação.</span><span class="sxs-lookup"><span data-stu-id="02128-103">The **System** facet indicates that the object is managed by the system for its own operation.</span></span>
<span data-ttu-id="02128-104">A maioria dos aplicativos deve ignorar itens que têm uma faceta do Sistema.</span><span class="sxs-lookup"><span data-stu-id="02128-104">Most apps should ignore items that have a System facet.</span></span>

<span data-ttu-id="02128-105">**Observação**: Embora essa faceta esteja vazia no momento, em revisões futuras da API a faceta pode ser preenchida com propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="02128-105">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="02128-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02128-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.systemFacet", "@type.aka": "microsoft.graph.systemFacet" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="02128-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02128-107">Properties</span></span>

<span data-ttu-id="02128-p102">Nenhum. Esta faceta é um valor nulo ou não nulo e não contém propriedades.</span><span class="sxs-lookup"><span data-stu-id="02128-p102">None. This facet is a null or not-null value and contains no properties.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/System",
  "suppressions": [
    "Error: /api-reference/beta/resources/systemfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
