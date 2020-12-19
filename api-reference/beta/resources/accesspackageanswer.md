---
title: tipo de recurso accessPackageAnswer
description: O tipo complexo para as respostas a um accessPackageQuestion que são armazenadas em um accessPackageAssignmentRequest.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f947c5235c18d3be5115199d789512602a3e0739
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720071"
---
# <a name="accesspackageanswer-resource-type"></a><span data-ttu-id="39d42-103">tipo de recurso accessPackageAnswer</span><span class="sxs-lookup"><span data-stu-id="39d42-103">accessPackageAnswer resource type</span></span>

<span data-ttu-id="39d42-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39d42-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39d42-105">O tipo complexo de uma resposta fornecida pelo solicitante para um [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="39d42-105">The complex type of a requestor's provided answer to an [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span> <span data-ttu-id="39d42-106">A resposta real será um subtipo desse tipo complexo, seja [accessPackageAnswerString](../resources/accesspackageanswerstring.md) ou [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md).</span><span class="sxs-lookup"><span data-stu-id="39d42-106">The actual answer will be a subtype of this complex type, either [accessPackageAnswerString](../resources/accesspackageanswerstring.md) or [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md).</span></span> <span data-ttu-id="39d42-107">Essas respostas serão armazenadas em um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="39d42-107">These answers will be stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

## <a name="properties"></a><span data-ttu-id="39d42-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39d42-108">Properties</span></span>
|<span data-ttu-id="39d42-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39d42-109">Property</span></span>|<span data-ttu-id="39d42-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="39d42-110">Type</span></span>|<span data-ttu-id="39d42-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="39d42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39d42-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="39d42-112">answeredQuestion</span></span>|[<span data-ttu-id="39d42-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="39d42-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="39d42-114">A pergunta para a resposta.</span><span class="sxs-lookup"><span data-stu-id="39d42-114">The question the answer is for.</span></span> <span data-ttu-id="39d42-115">Obrigatório e somente leitura.</span><span class="sxs-lookup"><span data-stu-id="39d42-115">Required and Read-only.</span></span>|
|<span data-ttu-id="39d42-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="39d42-116">displayValue</span></span>|<span data-ttu-id="39d42-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39d42-117">String</span></span>|<span data-ttu-id="39d42-118">O valor de exibição da resposta.</span><span class="sxs-lookup"><span data-stu-id="39d42-118">The display value of the answer.</span></span> <span data-ttu-id="39d42-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39d42-119">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39d42-120">Relações</span><span class="sxs-lookup"><span data-stu-id="39d42-120">Relationships</span></span>
<span data-ttu-id="39d42-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39d42-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39d42-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39d42-122">JSON representation</span></span>
<span data-ttu-id="39d42-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39d42-123">The following is a JSON representation of the resource.</span></span>
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

