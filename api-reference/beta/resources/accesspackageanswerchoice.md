---
title: tipo de recurso accessPackageAnswerChoice
description: Uma opção de resposta para um accessPackageMultipleChoiceQuestion.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6f34656a72d217adec1ff46be689b283461332fb
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720083"
---
# <a name="accesspackageanswerchoice-resource-type"></a><span data-ttu-id="10bbb-103">tipo de recurso accessPackageAnswerChoice</span><span class="sxs-lookup"><span data-stu-id="10bbb-103">accessPackageAnswerChoice resource type</span></span>

<span data-ttu-id="10bbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10bbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10bbb-105">Indica uma opção de resposta para um [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span><span class="sxs-lookup"><span data-stu-id="10bbb-105">Indicates an answer option for an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span> <span data-ttu-id="10bbb-106">Vários accessPackageAnswerChoices podem ser adicionados a um [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span><span class="sxs-lookup"><span data-stu-id="10bbb-106">Multiple accessPackageAnswerChoices can be added to an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="10bbb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10bbb-107">Properties</span></span>
|<span data-ttu-id="10bbb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10bbb-108">Property</span></span>|<span data-ttu-id="10bbb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="10bbb-109">Type</span></span>|<span data-ttu-id="10bbb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10bbb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10bbb-111">realvalue</span><span class="sxs-lookup"><span data-stu-id="10bbb-111">actualValue</span></span>|<span data-ttu-id="10bbb-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="10bbb-112">String</span></span>|<span data-ttu-id="10bbb-113">O valor real da escolha selecionada.</span><span class="sxs-lookup"><span data-stu-id="10bbb-113">The actual value of the selected choice.</span></span> <span data-ttu-id="10bbb-114">Normalmente, esse é um valor de cadeia de caracteres que é compreensível por aplicativos.</span><span class="sxs-lookup"><span data-stu-id="10bbb-114">This is typically a string value which is understandable by applications.</span></span> <span data-ttu-id="10bbb-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10bbb-115">Required.</span></span> |
|<span data-ttu-id="10bbb-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="10bbb-116">displayValue</span></span>|[<span data-ttu-id="10bbb-117">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="10bbb-117">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="10bbb-118">Os valores de exibição localizados mostrados para o solicitante e aprovadores.</span><span class="sxs-lookup"><span data-stu-id="10bbb-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="10bbb-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10bbb-119">Required.</span></span>

## <a name="relationships"></a><span data-ttu-id="10bbb-120">Relações</span><span class="sxs-lookup"><span data-stu-id="10bbb-120">Relationships</span></span>
<span data-ttu-id="10bbb-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10bbb-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10bbb-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10bbb-122">JSON representation</span></span>
<span data-ttu-id="10bbb-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10bbb-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAnswerChoice",
  "actualValue": "String",
  "displayValue": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  }
}
```
