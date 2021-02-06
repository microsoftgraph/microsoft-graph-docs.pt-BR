---
title: Tipo de recurso accessPackageTextInputQuestion
description: Filho de accessPackageQuestion que tem entrada de texto como formato de resposta da pergunta.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5f7d4d0ee7517ec3455d9e63647461e8101cab9d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133571"
---
# <a name="accesspackagetextinputquestion-resource-type"></a><span data-ttu-id="da650-103">Tipo de recurso accessPackageTextInputQuestion</span><span class="sxs-lookup"><span data-stu-id="da650-103">accessPackageTextInputQuestion resource type</span></span>

<span data-ttu-id="da650-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da650-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da650-105">Um filho de **accessPackageQuestion** que tem entrada de texto como resposta.</span><span class="sxs-lookup"><span data-stu-id="da650-105">A child of **accessPackageQuestion** that has text input as an answer.</span></span>

<span data-ttu-id="da650-106">Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="da650-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="da650-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da650-107">Properties</span></span>
|<span data-ttu-id="da650-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da650-108">Property</span></span>|<span data-ttu-id="da650-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="da650-109">Type</span></span>|<span data-ttu-id="da650-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="da650-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da650-111">id</span><span class="sxs-lookup"><span data-stu-id="da650-111">id</span></span>|<span data-ttu-id="da650-112">String</span><span class="sxs-lookup"><span data-stu-id="da650-112">String</span></span>|<span data-ttu-id="da650-113">ID da pergunta.</span><span class="sxs-lookup"><span data-stu-id="da650-113">ID of the question.</span></span> <span data-ttu-id="da650-114">Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="da650-114">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="da650-115">isRequired</span><span class="sxs-lookup"><span data-stu-id="da650-115">isRequired</span></span>|<span data-ttu-id="da650-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="da650-116">Boolean</span></span>|<span data-ttu-id="da650-117">Indica se o solicitante é obrigado a fornecer uma resposta ou não.</span><span class="sxs-lookup"><span data-stu-id="da650-117">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="da650-118">Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="da650-118">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="da650-119">isSingleLineQuestion</span><span class="sxs-lookup"><span data-stu-id="da650-119">isSingleLineQuestion</span></span>|<span data-ttu-id="da650-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="da650-120">Boolean</span></span>|<span data-ttu-id="da650-121">Indica se a resposta estará no formato de uma ou várias linhas.</span><span class="sxs-lookup"><span data-stu-id="da650-121">Indicates whether the answer will be in single or multiple line format.</span></span>|
|<span data-ttu-id="da650-122">sequence</span><span class="sxs-lookup"><span data-stu-id="da650-122">sequence</span></span>|<span data-ttu-id="da650-123">Int32</span><span class="sxs-lookup"><span data-stu-id="da650-123">Int32</span></span>|<span data-ttu-id="da650-124">Posição relativa dessa pergunta ao exibir uma lista de perguntas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="da650-124">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="da650-125">Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="da650-125">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="da650-126">texto</span><span class="sxs-lookup"><span data-stu-id="da650-126">text</span></span>|[<span data-ttu-id="da650-127">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="da650-127">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="da650-128">O texto da pergunta a ser mostre ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="da650-128">The text of the question to show to the requestor.</span></span> <span data-ttu-id="da650-129">Herdado [de accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="da650-129">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="da650-130">Relações</span><span class="sxs-lookup"><span data-stu-id="da650-130">Relationships</span></span>
<span data-ttu-id="da650-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da650-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da650-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da650-132">JSON representation</span></span>
<span data-ttu-id="da650-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da650-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageTextInputQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "isSingleLineQuestion": "Boolean"
}
```

