---
title: Tipo de recurso accessPackageAnswer
description: O tipo complexo para respostas a um accessPackageQuestion armazenado em um accessPackageAssignmentRequest.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3da6d1b0e2e519895af4dacca009b027807b0184
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135485"
---
# <a name="accesspackageanswer-resource-type"></a><span data-ttu-id="a147d-103">Tipo de recurso accessPackageAnswer</span><span class="sxs-lookup"><span data-stu-id="a147d-103">accessPackageAnswer resource type</span></span>

<span data-ttu-id="a147d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a147d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a147d-105">O tipo complexo de uma resposta fornecida pelo solicitante para um [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="a147d-105">The complex type of a requestor's provided answer to an [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span> <span data-ttu-id="a147d-106">A resposta real será um subtipo desse tipo complexo, [accessPackageAnswerString](../resources/accesspackageanswerstring.md) ou [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md).</span><span class="sxs-lookup"><span data-stu-id="a147d-106">The actual answer will be a subtype of this complex type, either [accessPackageAnswerString](../resources/accesspackageanswerstring.md) or [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md).</span></span> <span data-ttu-id="a147d-107">Essas respostas serão armazenadas em um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a147d-107">These answers will be stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a147d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a147d-108">Properties</span></span>
|<span data-ttu-id="a147d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a147d-109">Property</span></span>|<span data-ttu-id="a147d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a147d-110">Type</span></span>|<span data-ttu-id="a147d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a147d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a147d-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="a147d-112">answeredQuestion</span></span>|[<span data-ttu-id="a147d-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="a147d-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="a147d-114">A pergunta para a que a resposta se trata.</span><span class="sxs-lookup"><span data-stu-id="a147d-114">The question the answer is for.</span></span> <span data-ttu-id="a147d-115">Obrigatório e somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a147d-115">Required and Read-only.</span></span>|
|<span data-ttu-id="a147d-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="a147d-116">displayValue</span></span>|<span data-ttu-id="a147d-117">String</span><span class="sxs-lookup"><span data-stu-id="a147d-117">String</span></span>|<span data-ttu-id="a147d-118">O valor de exibição da resposta.</span><span class="sxs-lookup"><span data-stu-id="a147d-118">The display value of the answer.</span></span> <span data-ttu-id="a147d-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a147d-119">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a147d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a147d-120">Relationships</span></span>
<span data-ttu-id="a147d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a147d-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a147d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a147d-122">JSON representation</span></span>
<span data-ttu-id="a147d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a147d-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswer",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  }
}
```

