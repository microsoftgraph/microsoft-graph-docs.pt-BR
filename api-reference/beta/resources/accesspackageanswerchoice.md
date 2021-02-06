---
title: Tipo de recurso accessPackageAnswerChoice
description: Uma opção de resposta para um accessPackageMultipleChoiceQuestion.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c7fc7db1c9360146c2f62fd9048ad0db3d58b80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135475"
---
# <a name="accesspackageanswerchoice-resource-type"></a><span data-ttu-id="efd12-103">Tipo de recurso accessPackageAnswerChoice</span><span class="sxs-lookup"><span data-stu-id="efd12-103">accessPackageAnswerChoice resource type</span></span>

<span data-ttu-id="efd12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efd12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efd12-105">Indica uma opção de resposta para um [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span><span class="sxs-lookup"><span data-stu-id="efd12-105">Indicates an answer option for an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span> <span data-ttu-id="efd12-106">Vários accessPackageAnswerChoices podem ser adicionados a [um accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span><span class="sxs-lookup"><span data-stu-id="efd12-106">Multiple accessPackageAnswerChoices can be added to an [accessPackageMultipleChoiceQuestion](../resources/accesspackagemultiplechoicequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="efd12-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efd12-107">Properties</span></span>
|<span data-ttu-id="efd12-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efd12-108">Property</span></span>|<span data-ttu-id="efd12-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="efd12-109">Type</span></span>|<span data-ttu-id="efd12-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="efd12-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd12-111">actualValue</span><span class="sxs-lookup"><span data-stu-id="efd12-111">actualValue</span></span>|<span data-ttu-id="efd12-112">String</span><span class="sxs-lookup"><span data-stu-id="efd12-112">String</span></span>|<span data-ttu-id="efd12-113">O valor real da opção selecionada.</span><span class="sxs-lookup"><span data-stu-id="efd12-113">The actual value of the selected choice.</span></span> <span data-ttu-id="efd12-114">Isso geralmente é um valor de cadeia de caracteres que pode ser entendido pelos aplicativos.</span><span class="sxs-lookup"><span data-stu-id="efd12-114">This is typically a string value which is understandable by applications.</span></span> <span data-ttu-id="efd12-115">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efd12-115">Required.</span></span> |
|<span data-ttu-id="efd12-116">displayValue</span><span class="sxs-lookup"><span data-stu-id="efd12-116">displayValue</span></span>|[<span data-ttu-id="efd12-117">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="efd12-117">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="efd12-118">Os valores de exibição localizados mostrados para o solicitante e os aprovadores.</span><span class="sxs-lookup"><span data-stu-id="efd12-118">The localized display values shown to the requestor and approvers.</span></span> <span data-ttu-id="efd12-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="efd12-119">Required.</span></span>

## <a name="relationships"></a><span data-ttu-id="efd12-120">Relações</span><span class="sxs-lookup"><span data-stu-id="efd12-120">Relationships</span></span>
<span data-ttu-id="efd12-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efd12-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="efd12-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efd12-122">JSON representation</span></span>
<span data-ttu-id="efd12-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efd12-123">The following is a JSON representation of the resource.</span></span>
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
