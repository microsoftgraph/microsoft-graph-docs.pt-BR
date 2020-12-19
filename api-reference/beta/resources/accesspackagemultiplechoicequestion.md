---
title: tipo de recurso accessPackageMultipleChoiceQuestion
description: Subclasse de accessPackageQuestion com múltipla escolha como o formato de resposta da pergunta
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab61a8df1faf0f9b1d9fa3dee10521001ddc6d31
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720069"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a><span data-ttu-id="9d21b-103">tipo de recurso accessPackageMultipleChoiceQuestion</span><span class="sxs-lookup"><span data-stu-id="9d21b-103">accessPackageMultipleChoiceQuestion resource type</span></span>

<span data-ttu-id="9d21b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d21b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d21b-105">Um filho de **accessPackageQuestion** que apresenta várias opções para as quais o solicitante deve escolher uma resposta.</span><span class="sxs-lookup"><span data-stu-id="9d21b-105">A child of **accessPackageQuestion** that presents multiple options that the requestor must choose an answer from.</span></span>

<span data-ttu-id="9d21b-106">Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="9d21b-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9d21b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d21b-107">Properties</span></span>
|<span data-ttu-id="9d21b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d21b-108">Property</span></span>|<span data-ttu-id="9d21b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d21b-109">Type</span></span>|<span data-ttu-id="9d21b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d21b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d21b-111">allowsMultipleSelection</span><span class="sxs-lookup"><span data-stu-id="9d21b-111">allowsMultipleSelection</span></span>|<span data-ttu-id="9d21b-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d21b-112">Boolean</span></span>|<span data-ttu-id="9d21b-113">Indica se o solicitante pode selecionar várias opções como resposta.</span><span class="sxs-lookup"><span data-stu-id="9d21b-113">Indicates whether requestor can select multiple choices as their answer.</span></span>|
|<span data-ttu-id="9d21b-114">respostas</span><span class="sxs-lookup"><span data-stu-id="9d21b-114">choices</span></span>|<span data-ttu-id="9d21b-115">coleção [accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md)</span><span class="sxs-lookup"><span data-stu-id="9d21b-115">[accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md) collection</span></span>|<span data-ttu-id="9d21b-116">Lista de opções de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d21b-116">List of answer choices.</span></span>|
|<span data-ttu-id="9d21b-117">id</span><span class="sxs-lookup"><span data-stu-id="9d21b-117">id</span></span>|<span data-ttu-id="9d21b-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9d21b-118">String</span></span>|<span data-ttu-id="9d21b-119">ID da pergunta.</span><span class="sxs-lookup"><span data-stu-id="9d21b-119">ID of the question.</span></span> <span data-ttu-id="9d21b-120">Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="9d21b-120">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="9d21b-121">isRequired</span><span class="sxs-lookup"><span data-stu-id="9d21b-121">isRequired</span></span>|<span data-ttu-id="9d21b-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d21b-122">Boolean</span></span>|<span data-ttu-id="9d21b-123">Indica se o solicitante é necessário para fornecer uma resposta ou não.</span><span class="sxs-lookup"><span data-stu-id="9d21b-123">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="9d21b-124">Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="9d21b-124">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="9d21b-125">sequence</span><span class="sxs-lookup"><span data-stu-id="9d21b-125">sequence</span></span>|<span data-ttu-id="9d21b-126">Int32</span><span class="sxs-lookup"><span data-stu-id="9d21b-126">Int32</span></span>|<span data-ttu-id="9d21b-127">Posição relativa desta pergunta ao exibir uma lista de perguntas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="9d21b-127">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="9d21b-128">Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="9d21b-128">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="9d21b-129">texto</span><span class="sxs-lookup"><span data-stu-id="9d21b-129">text</span></span>|[<span data-ttu-id="9d21b-130">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="9d21b-130">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="9d21b-131">O texto da pergunta para mostrar o solicitante.</span><span class="sxs-lookup"><span data-stu-id="9d21b-131">The text of the question to show the requestor.</span></span> <span data-ttu-id="9d21b-132">Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="9d21b-132">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d21b-133">Relações</span><span class="sxs-lookup"><span data-stu-id="9d21b-133">Relationships</span></span>
<span data-ttu-id="9d21b-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d21b-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d21b-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d21b-135">JSON representation</span></span>
<span data-ttu-id="9d21b-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d21b-136">The following is a JSON representation of the resource.</span></span>
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
