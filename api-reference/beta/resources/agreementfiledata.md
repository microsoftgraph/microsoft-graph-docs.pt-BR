---
title: tipo de recurso agreementFileData
description: Representa o blob de um arquivo de contrato de uso do Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: c6f4b6708493c0063928a81c95eeb60b7e7603b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339136"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="304cf-103">tipo de recurso agreementFileData</span><span class="sxs-lookup"><span data-stu-id="304cf-103">agreementFileData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="304cf-104">Representa o blob de um arquivo de contrato de uso do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="304cf-104">Represents the blob of an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="304cf-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="304cf-105">Properties</span></span>
| <span data-ttu-id="304cf-106">Método</span><span class="sxs-lookup"><span data-stu-id="304cf-106">Method</span></span>       | <span data-ttu-id="304cf-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="304cf-107">Return Type</span></span> | <span data-ttu-id="304cf-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="304cf-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="304cf-109">data</span><span class="sxs-lookup"><span data-stu-id="304cf-109">data</span></span>|<span data-ttu-id="304cf-110">Binária</span><span class="sxs-lookup"><span data-stu-id="304cf-110">Binary</span></span>|<span data-ttu-id="304cf-111">Dados que representam o documento PDF termos de uso.</span><span class="sxs-lookup"><span data-stu-id="304cf-111">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="304cf-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="304cf-112">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="304cf-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="304cf-113">JSON representation</span></span>

<span data-ttu-id="304cf-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="304cf-114">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
