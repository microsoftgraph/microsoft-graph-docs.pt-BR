---
title: tipo de recurso accessPackageQuestion
description: O tipo complexo para perguntas configuradas em uma política de atribuição de pacote do Access.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 876c21018104ed579cbaf04b0f4642395627964e
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720068"
---
# <a name="accesspackagequestion-resource-type"></a><span data-ttu-id="34d37-103">tipo de recurso accessPackageQuestion</span><span class="sxs-lookup"><span data-stu-id="34d37-103">accessPackageQuestion resource type</span></span>

<span data-ttu-id="34d37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34d37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34d37-105">Usada para a `accessPackageQuestion` propriedade de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="34d37-105">Used for the `accessPackageQuestion` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> 

<span data-ttu-id="34d37-106">Os subtipos incluem [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) e [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).</span><span class="sxs-lookup"><span data-stu-id="34d37-106">Subtypes include [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) and [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="34d37-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34d37-107">Properties</span></span>
|<span data-ttu-id="34d37-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34d37-108">Property</span></span>|<span data-ttu-id="34d37-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="34d37-109">Type</span></span>|<span data-ttu-id="34d37-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="34d37-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34d37-111">id</span><span class="sxs-lookup"><span data-stu-id="34d37-111">id</span></span>|<span data-ttu-id="34d37-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34d37-112">String</span></span>| <span data-ttu-id="34d37-113">ID da pergunta.</span><span class="sxs-lookup"><span data-stu-id="34d37-113">ID of the question.</span></span>|
|<span data-ttu-id="34d37-114">isRequired</span><span class="sxs-lookup"><span data-stu-id="34d37-114">isRequired</span></span>|<span data-ttu-id="34d37-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="34d37-115">Boolean</span></span>| <span data-ttu-id="34d37-116">Se o solicitante é necessário para fornecer uma resposta ou não.</span><span class="sxs-lookup"><span data-stu-id="34d37-116">Whether the requestor is required to supply an answer or not.</span></span>|
|<span data-ttu-id="34d37-117">sequence</span><span class="sxs-lookup"><span data-stu-id="34d37-117">sequence</span></span>|<span data-ttu-id="34d37-118">Int32</span><span class="sxs-lookup"><span data-stu-id="34d37-118">Int32</span></span>| <span data-ttu-id="34d37-119">Posição relativa desta pergunta ao exibir uma lista de perguntas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="34d37-119">Relative position of this question when displaying a list of questions to the requestor.</span></span>|
|<span data-ttu-id="34d37-120">texto</span><span class="sxs-lookup"><span data-stu-id="34d37-120">text</span></span>|[<span data-ttu-id="34d37-121">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="34d37-121">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="34d37-122">O texto da pergunta a ser mostrado para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="34d37-122">The text of the question to show to the requestor.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34d37-123">Relações</span><span class="sxs-lookup"><span data-stu-id="34d37-123">Relationships</span></span>
<span data-ttu-id="34d37-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34d37-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34d37-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34d37-125">JSON representation</span></span>
<span data-ttu-id="34d37-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34d37-126">The following is a JSON representation of the resource.</span></span>
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

