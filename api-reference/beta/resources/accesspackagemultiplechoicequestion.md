---
title: Tipo de recurso accessPackageMultipleChoiceQuestion
description: Subclasse de accessPackageQuestion que tem várias opções como o formato de resposta da pergunta
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 54054edcda2f41ad3f4e1bd29fb807c18709ee1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137337"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a><span data-ttu-id="15599-103">Tipo de recurso accessPackageMultipleChoiceQuestion</span><span class="sxs-lookup"><span data-stu-id="15599-103">accessPackageMultipleChoiceQuestion resource type</span></span>

<span data-ttu-id="15599-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15599-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15599-105">Um filho de **accessPackageQuestion** que apresenta várias opções das quais o solicitante deve escolher uma resposta.</span><span class="sxs-lookup"><span data-stu-id="15599-105">A child of **accessPackageQuestion** that presents multiple options that the requestor must choose an answer from.</span></span>

<span data-ttu-id="15599-106">Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="15599-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="15599-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15599-107">Properties</span></span>
|<span data-ttu-id="15599-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15599-108">Property</span></span>|<span data-ttu-id="15599-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="15599-109">Type</span></span>|<span data-ttu-id="15599-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="15599-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15599-111">allowsMultipleSelection</span><span class="sxs-lookup"><span data-stu-id="15599-111">allowsMultipleSelection</span></span>|<span data-ttu-id="15599-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="15599-112">Boolean</span></span>|<span data-ttu-id="15599-113">Indica se o solicitante pode selecionar várias opções como resposta.</span><span class="sxs-lookup"><span data-stu-id="15599-113">Indicates whether requestor can select multiple choices as their answer.</span></span>|
|<span data-ttu-id="15599-114">choices</span><span class="sxs-lookup"><span data-stu-id="15599-114">choices</span></span>|<span data-ttu-id="15599-115">[coleção accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md)</span><span class="sxs-lookup"><span data-stu-id="15599-115">[accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md) collection</span></span>|<span data-ttu-id="15599-116">Lista de opções de resposta.</span><span class="sxs-lookup"><span data-stu-id="15599-116">List of answer choices.</span></span>|
|<span data-ttu-id="15599-117">id</span><span class="sxs-lookup"><span data-stu-id="15599-117">id</span></span>|<span data-ttu-id="15599-118">String</span><span class="sxs-lookup"><span data-stu-id="15599-118">String</span></span>|<span data-ttu-id="15599-119">ID da pergunta.</span><span class="sxs-lookup"><span data-stu-id="15599-119">ID of the question.</span></span> <span data-ttu-id="15599-120">Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="15599-120">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="15599-121">isRequired</span><span class="sxs-lookup"><span data-stu-id="15599-121">isRequired</span></span>|<span data-ttu-id="15599-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="15599-122">Boolean</span></span>|<span data-ttu-id="15599-123">Indica se o solicitante é obrigado a fornecer uma resposta ou não.</span><span class="sxs-lookup"><span data-stu-id="15599-123">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="15599-124">Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="15599-124">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="15599-125">sequence</span><span class="sxs-lookup"><span data-stu-id="15599-125">sequence</span></span>|<span data-ttu-id="15599-126">Int32</span><span class="sxs-lookup"><span data-stu-id="15599-126">Int32</span></span>|<span data-ttu-id="15599-127">Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="15599-127">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="15599-128">Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="15599-128">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="15599-129">texto</span><span class="sxs-lookup"><span data-stu-id="15599-129">text</span></span>|[<span data-ttu-id="15599-130">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="15599-130">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="15599-131">O texto da pergunta para mostrar o solicitante.</span><span class="sxs-lookup"><span data-stu-id="15599-131">The text of the question to show the requestor.</span></span> <span data-ttu-id="15599-132">Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="15599-132">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="15599-133">Relações</span><span class="sxs-lookup"><span data-stu-id="15599-133">Relationships</span></span>
<span data-ttu-id="15599-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15599-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15599-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15599-135">JSON representation</span></span>
<span data-ttu-id="15599-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15599-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "choices": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
    }
  ],
  "allowsMultipleSelection": "Boolean"
}
```
