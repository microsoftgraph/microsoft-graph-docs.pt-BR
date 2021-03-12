---
title: Tipo de recurso agreementFileData
description: Representa um arquivo de contrato de uso do Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 31837b69a87f731f41de23a458dedec665bfe5c4
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722552"
---
# <a name="agreementfiledata-resource-type"></a><span data-ttu-id="ad0fa-103">Tipo de recurso agreementFileData</span><span class="sxs-lookup"><span data-stu-id="ad0fa-103">agreementFileData resource type</span></span>

<span data-ttu-id="ad0fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad0fa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad0fa-105">Representa um arquivo de contrato de uso do Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ad0fa-105">Represents an Azure Active Directory (Azure AD) terms of use agreement file.</span></span>

## <a name="properties"></a><span data-ttu-id="ad0fa-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad0fa-106">Properties</span></span>
| <span data-ttu-id="ad0fa-107">Método</span><span class="sxs-lookup"><span data-stu-id="ad0fa-107">Method</span></span>       | <span data-ttu-id="ad0fa-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ad0fa-108">Return Type</span></span> | <span data-ttu-id="ad0fa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad0fa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ad0fa-110">data</span><span class="sxs-lookup"><span data-stu-id="ad0fa-110">data</span></span>|<span data-ttu-id="ad0fa-111">Binária</span><span class="sxs-lookup"><span data-stu-id="ad0fa-111">Binary</span></span>|<span data-ttu-id="ad0fa-112">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="ad0fa-112">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="ad0fa-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad0fa-113">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad0fa-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad0fa-114">JSON representation</span></span>

<span data-ttu-id="ad0fa-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad0fa-115">The following is a JSON representation of the resource.</span></span>

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


