---
title: Tipo de recurso accessPackageAnswerString
description: Uma resposta de cadeia de caracteres para um accessPackageTextInputQuestion
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: def7753e62239e403821ed6472b3613d025942ac
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132388"
---
# <a name="accesspackageanswerstring-resource-type"></a><span data-ttu-id="fd7c9-103">Tipo de recurso accessPackageAnswerString</span><span class="sxs-lookup"><span data-stu-id="fd7c9-103">accessPackageAnswerString resource type</span></span>

<span data-ttu-id="fd7c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd7c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd7c9-105">Indica a resposta de entrada de cadeia de caracteres para [um accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md).</span><span class="sxs-lookup"><span data-stu-id="fd7c9-105">Indicates the string input answer to an [accessPackageTextInputQuestion](../resources/accesspackagetextinputquestion.md).</span></span> <span data-ttu-id="fd7c9-106">Armazenado em um [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span><span class="sxs-lookup"><span data-stu-id="fd7c9-106">Stored on an [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md).</span></span>

<span data-ttu-id="fd7c9-107">Herda de [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="fd7c9-107">Inherits from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fd7c9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd7c9-108">Properties</span></span>
|<span data-ttu-id="fd7c9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fd7c9-109">Property</span></span>|<span data-ttu-id="fd7c9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd7c9-110">Type</span></span>|<span data-ttu-id="fd7c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd7c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd7c9-112">answeredQuestion</span><span class="sxs-lookup"><span data-stu-id="fd7c9-112">answeredQuestion</span></span>|[<span data-ttu-id="fd7c9-113">accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="fd7c9-113">accessPackageQuestion</span></span>](../resources/accesspackagequestion.md)|<span data-ttu-id="fd7c9-114">A pergunta à que a resposta se aplica.</span><span class="sxs-lookup"><span data-stu-id="fd7c9-114">The question the answer applies to.</span></span> <span data-ttu-id="fd7c9-115">Herdado de [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="fd7c9-115">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="fd7c9-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="fd7c9-116">displayValue</span></span>|<span data-ttu-id="fd7c9-117">String</span><span class="sxs-lookup"><span data-stu-id="fd7c9-117">String</span></span>|<span data-ttu-id="fd7c9-118">Os valores de exibição localizados mostrados para o solicitante e os aprovadores.</span><span class="sxs-lookup"><span data-stu-id="fd7c9-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="fd7c9-119">Herdado de [accessPackageAnswer](../resources/accesspackageanswer.md).</span><span class="sxs-lookup"><span data-stu-id="fd7c9-119">Inherited from [accessPackageAnswer](../resources/accesspackageanswer.md).</span></span>|
|<span data-ttu-id="fd7c9-120">value</span><span class="sxs-lookup"><span data-stu-id="fd7c9-120">value</span></span>|<span data-ttu-id="fd7c9-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fd7c9-121">String</span></span>|<span data-ttu-id="fd7c9-122">O valor armazenado no perfil de usuário do solicitante, se essa resposta estiver configurada para ser armazenada como um atributo específico.</span><span class="sxs-lookup"><span data-stu-id="fd7c9-122">The value stored on the requestor's user profile, if this answer is configured to be stored as a specific attribute.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd7c9-123">Relações</span><span class="sxs-lookup"><span data-stu-id="fd7c9-123">Relationships</span></span>
<span data-ttu-id="fd7c9-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fd7c9-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd7c9-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd7c9-125">JSON representation</span></span>
<span data-ttu-id="fd7c9-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fd7c9-126">The following is a JSON representation of the resource.</span></span>
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

