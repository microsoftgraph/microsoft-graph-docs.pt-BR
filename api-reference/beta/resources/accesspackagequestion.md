---
title: Tipo de recurso accessPackageQuestion
description: O tipo complexo para perguntas configuradas em uma política de atribuição de pacote de acesso.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 04849b79cfa6c58132360f8ec20c363ea21453ec
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132374"
---
# <a name="accesspackagequestion-resource-type"></a><span data-ttu-id="b601e-103">Tipo de recurso accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="b601e-103">accessPackageQuestion resource type</span></span>

<span data-ttu-id="b601e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b601e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b601e-105">Usado para a propriedade `accessPackageQuestion` de uma política de [atribuição de pacote de acesso.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b601e-105">Used for the `accessPackageQuestion` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> 

<span data-ttu-id="b601e-106">Os subtipos [incluem accessPackageTextInputQuestions](accesspackagetextinputquestion.md) e [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).</span><span class="sxs-lookup"><span data-stu-id="b601e-106">Subtypes include [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) and [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b601e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b601e-107">Properties</span></span>
|<span data-ttu-id="b601e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b601e-108">Property</span></span>|<span data-ttu-id="b601e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b601e-109">Type</span></span>|<span data-ttu-id="b601e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b601e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b601e-111">id</span><span class="sxs-lookup"><span data-stu-id="b601e-111">id</span></span>|<span data-ttu-id="b601e-112">String</span><span class="sxs-lookup"><span data-stu-id="b601e-112">String</span></span>| <span data-ttu-id="b601e-113">ID da pergunta.</span><span class="sxs-lookup"><span data-stu-id="b601e-113">ID of the question.</span></span>|
|<span data-ttu-id="b601e-114">isRequired</span><span class="sxs-lookup"><span data-stu-id="b601e-114">isRequired</span></span>|<span data-ttu-id="b601e-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="b601e-115">Boolean</span></span>| <span data-ttu-id="b601e-116">Se o solicitante precisa fornecer uma resposta ou não.</span><span class="sxs-lookup"><span data-stu-id="b601e-116">Whether the requestor is required to supply an answer or not.</span></span>|
|<span data-ttu-id="b601e-117">sequence</span><span class="sxs-lookup"><span data-stu-id="b601e-117">sequence</span></span>|<span data-ttu-id="b601e-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b601e-118">Int32</span></span>| <span data-ttu-id="b601e-119">Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="b601e-119">Relative position of this question when displaying a list of questions to the requestor.</span></span>|
|<span data-ttu-id="b601e-120">texto</span><span class="sxs-lookup"><span data-stu-id="b601e-120">text</span></span>|[<span data-ttu-id="b601e-121">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="b601e-121">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="b601e-122">O texto da pergunta a ser mostre ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="b601e-122">The text of the question to show to the requestor.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b601e-123">Relações</span><span class="sxs-lookup"><span data-stu-id="b601e-123">Relationships</span></span>
<span data-ttu-id="b601e-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b601e-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b601e-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b601e-125">JSON representation</span></span>
<span data-ttu-id="b601e-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b601e-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer"
}
```

