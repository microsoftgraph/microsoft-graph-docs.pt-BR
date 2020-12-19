---
title: tipo de recurso accessPackageAnswerString
description: Uma resposta de cadeia de caracteres para um accessPackageTextInputQuestion
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a5273872b2ded749ddfc13998c5b0104a0a63ec
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720039"
---
# <a name="accesspackageanswerstring-resource-type"></a><span data-ttu-id="f5d3d-103">tipo de recurso accessPackageAnswerString</span><span class="sxs-lookup"><span data-stu-id="f5d3d-103">accessPackageAnswerString resource type</span></span>

<span data-ttu-id="f5d3d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5d3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5d3d-105">Indica a resposta de entrada da cadeia de caracteres para um [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md).</span><span class="sxs-lookup"><span data-stu-id="f5d3d-105">Indicates the string input answer to an [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md).</span></span> <span data-ttu-id="f5d3d-106">Armazenado em um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f5d3d-106">Stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

<span data-ttu-id="f5d3d-107">Herda de [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="f5d3d-107">Inherits from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f5d3d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5d3d-108">Properties</span></span>
|<span data-ttu-id="f5d3d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5d3d-109">Property</span></span>|<span data-ttu-id="f5d3d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5d3d-110">Type</span></span>|<span data-ttu-id="f5d3d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5d3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5d3d-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="f5d3d-112">answeredQuestion</span></span>|[<span data-ttu-id="f5d3d-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="f5d3d-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="f5d3d-114">A pergunta à qual a resposta se aplica.</span><span class="sxs-lookup"><span data-stu-id="f5d3d-114">The question the answer applies to.</span></span> <span data-ttu-id="f5d3d-115">Herdado de [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="f5d3d-115">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="f5d3d-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="f5d3d-116">displayValue</span></span>|<span data-ttu-id="f5d3d-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5d3d-117">String</span></span>|<span data-ttu-id="f5d3d-118">Os valores de exibição localizados mostrados para o solicitante e aprovadores.</span><span class="sxs-lookup"><span data-stu-id="f5d3d-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="f5d3d-119">Herdado de [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="f5d3d-119">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="f5d3d-120">value</span><span class="sxs-lookup"><span data-stu-id="f5d3d-120">value</span></span>|<span data-ttu-id="f5d3d-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5d3d-121">String</span></span>|<span data-ttu-id="f5d3d-122">O valor armazenado no perfil de usuário do solicitante, se essa resposta estiver configurada para ser armazenada como um atributo específico.</span><span class="sxs-lookup"><span data-stu-id="f5d3d-122">The value stored on the requestor's user profile, if this answer is configured to be stored as a specific attribute.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5d3d-123">Relações</span><span class="sxs-lookup"><span data-stu-id="f5d3d-123">Relationships</span></span>
<span data-ttu-id="f5d3d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5d3d-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5d3d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5d3d-125">JSON representation</span></span>
<span data-ttu-id="f5d3d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5d3d-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerString",
  "displayValue": "String",
  "answeredQuestion": {
    "@odata.type": "microsoft.graph.accessPackageQuestion"
  },
  "value": "String"
}
```

