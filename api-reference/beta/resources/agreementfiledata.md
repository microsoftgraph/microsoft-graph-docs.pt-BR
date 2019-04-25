---
title: tipo de recurso agreementFileData
description: Representa o blob de um arquivo de contrato de uso do Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: bc0e7395875f64a3ee52e43b26da1a2df6276c9c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544100"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="351ed-103">tipo de recurso agreementFileData</span><span class="sxs-lookup"><span data-stu-id="351ed-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="351ed-104">Representa o blob de um arquivo de contrato de uso do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="351ed-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="351ed-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="351ed-105">Properties</span></span>
| <span data-ttu-id="351ed-106">Método</span><span class="sxs-lookup"><span data-stu-id="351ed-106">Method</span></span>       | <span data-ttu-id="351ed-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="351ed-107">Return Type</span></span> | <span data-ttu-id="351ed-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="351ed-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="351ed-109">data</span><span class="sxs-lookup"><span data-stu-id="351ed-109">data</span></span>|<span data-ttu-id="351ed-110">Binário</span><span class="sxs-lookup"><span data-stu-id="351ed-110">Binary</span></span>|<span data-ttu-id="351ed-111">Dados que representam o documento PDF termos de uso.</span><span class="sxs-lookup"><span data-stu-id="351ed-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="351ed-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="351ed-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="351ed-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="351ed-113">JSON representation</span></span>

<span data-ttu-id="351ed-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="351ed-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfiledata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
