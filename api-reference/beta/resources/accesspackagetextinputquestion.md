---
title: tipo de recurso accessPackageTextInputQuestion
description: Filho de accessPackageQuestion que tem entrada de texto como o formato de resposta da pergunta.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8609532e096fb587b4dcf49b8eb624aea314a8c6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720051"
---
# <a name="accesspackagetextinputquestion-resource-type"></a><span data-ttu-id="03165-103">tipo de recurso accessPackageTextInputQuestion</span><span class="sxs-lookup"><span data-stu-id="03165-103">accessPackageTextInputQuestion resource type</span></span>

<span data-ttu-id="03165-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03165-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03165-105">Um filho de **accessPackageQuestion** que tem entrada de texto como resposta.</span><span class="sxs-lookup"><span data-stu-id="03165-105">A child of **accessPackageQuestion** that has text input as an answer.</span></span>

<span data-ttu-id="03165-106">Herda de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="03165-106">Inherits from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>

## <a name="properties"></a><span data-ttu-id="03165-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03165-107">Properties</span></span>
|<span data-ttu-id="03165-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03165-108">Property</span></span>|<span data-ttu-id="03165-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="03165-109">Type</span></span>|<span data-ttu-id="03165-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="03165-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03165-111">id</span><span class="sxs-lookup"><span data-stu-id="03165-111">id</span></span>|<span data-ttu-id="03165-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03165-112">String</span></span>|<span data-ttu-id="03165-113">ID da pergunta.</span><span class="sxs-lookup"><span data-stu-id="03165-113">ID of the question.</span></span> <span data-ttu-id="03165-114">Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="03165-114">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="03165-115">isRequired</span><span class="sxs-lookup"><span data-stu-id="03165-115">isRequired</span></span>|<span data-ttu-id="03165-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="03165-116">Boolean</span></span>|<span data-ttu-id="03165-117">Indica se o solicitante é necessário para fornecer uma resposta ou não.</span><span class="sxs-lookup"><span data-stu-id="03165-117">Indicates whether the requestor is required to supply an answer or not.</span></span> <span data-ttu-id="03165-118">Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="03165-118">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="03165-119">isSingleLineQuestion</span><span class="sxs-lookup"><span data-stu-id="03165-119">isSingleLineQuestion</span></span>|<span data-ttu-id="03165-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="03165-120">Boolean</span></span>|<span data-ttu-id="03165-121">Indica se a resposta estará em um formato de linha única ou múltipla.</span><span class="sxs-lookup"><span data-stu-id="03165-121">Indicates whether the answer will be in single or multiple line format.</span></span>|
|<span data-ttu-id="03165-122">sequence</span><span class="sxs-lookup"><span data-stu-id="03165-122">sequence</span></span>|<span data-ttu-id="03165-123">Int32</span><span class="sxs-lookup"><span data-stu-id="03165-123">Int32</span></span>|<span data-ttu-id="03165-124">Posição relativa desta pergunta ao exibir uma lista de perguntas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="03165-124">Relative position of this question when displaying a list of questions to the requestor.</span></span> <span data-ttu-id="03165-125">Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="03165-125">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|
|<span data-ttu-id="03165-126">texto</span><span class="sxs-lookup"><span data-stu-id="03165-126">text</span></span>|[<span data-ttu-id="03165-127">accessPackageLocalizedContent</span><span class="sxs-lookup"><span data-stu-id="03165-127">accessPackageLocalizedContent</span></span>](../resources/accesspackagelocalizedcontent.md)|<span data-ttu-id="03165-128">O texto da pergunta a ser mostrado para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="03165-128">The text of the question to show to the requestor.</span></span> <span data-ttu-id="03165-129">Herdado de [accessPackageQuestion](../resources/accesspackagequestion.md).</span><span class="sxs-lookup"><span data-stu-id="03165-129">Inherited from [accessPackageQuestion](../resources/accesspackagequestion.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="03165-130">Relações</span><span class="sxs-lookup"><span data-stu-id="03165-130">Relationships</span></span>
<span data-ttu-id="03165-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03165-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03165-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03165-132">JSON representation</span></span>
<span data-ttu-id="03165-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03165-133">The following is a JSON representation of the resource.</span></span>
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

