---
title: Tipo de recurso inferenceClassification
description: 'Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf1ea3b61df2166f58f161b804f55e87e474be97
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006266"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="63f3a-103">Tipo de recurso inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="63f3a-103">inferenceClassification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63f3a-104">Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário.</span><span class="sxs-lookup"><span data-stu-id="63f3a-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="63f3a-105">Para saber mais, consulte [Gerenciar a Caixa de Entrada Prioritária](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="63f3a-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="63f3a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="63f3a-106">Methods</span></span>

| <span data-ttu-id="63f3a-107">Método</span><span class="sxs-lookup"><span data-stu-id="63f3a-107">Method</span></span>           | <span data-ttu-id="63f3a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="63f3a-108">Return Type</span></span>    |<span data-ttu-id="63f3a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f3a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="63f3a-110">Create inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="63f3a-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="63f3a-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="63f3a-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="63f3a-p101">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="63f3a-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="63f3a-114">List overrides</span><span class="sxs-lookup"><span data-stu-id="63f3a-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="63f3a-115">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="63f3a-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="63f3a-116">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="63f3a-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="63f3a-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="63f3a-117">Properties</span></span>
| <span data-ttu-id="63f3a-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="63f3a-118">Property</span></span>     | <span data-ttu-id="63f3a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="63f3a-119">Type</span></span>   |<span data-ttu-id="63f3a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f3a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63f3a-121">id</span><span class="sxs-lookup"><span data-stu-id="63f3a-121">id</span></span>|<span data-ttu-id="63f3a-122">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="63f3a-122">string</span></span>| <span data-ttu-id="63f3a-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="63f3a-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63f3a-124">Relações</span><span class="sxs-lookup"><span data-stu-id="63f3a-124">Relationships</span></span>
| <span data-ttu-id="63f3a-125">Relação</span><span class="sxs-lookup"><span data-stu-id="63f3a-125">Relationship</span></span> | <span data-ttu-id="63f3a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="63f3a-126">Type</span></span>   |<span data-ttu-id="63f3a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="63f3a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63f3a-128">overrides</span><span class="sxs-lookup"><span data-stu-id="63f3a-128">overrides</span></span>|<span data-ttu-id="63f3a-129">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="63f3a-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="63f3a-p102">Um conjunto de substituições para um usuário sempre classificar mensagens a partir de remetentes específicos, de maneiras específicas: `focused`, ou `other`. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="63f3a-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63f3a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="63f3a-133">JSON representation</span></span>

<span data-ttu-id="63f3a-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="63f3a-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
