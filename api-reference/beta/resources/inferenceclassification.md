---
title: Tipo de recurso inferenceClassification
description: 'Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário. '
localization_priority: Normal
ms.openlocfilehash: 3bfd5371d3600f985f9e170f717b4775fa31b9b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339966"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="b07c6-103">Tipo de recurso inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="b07c6-103">inferenceClassification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b07c6-104">Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b07c6-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="b07c6-105">Para saber mais, consulte [Gerenciar a Caixa de Entrada Prioritária](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="b07c6-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="b07c6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b07c6-106">Methods</span></span>

| <span data-ttu-id="b07c6-107">Método</span><span class="sxs-lookup"><span data-stu-id="b07c6-107">Method</span></span>           | <span data-ttu-id="b07c6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b07c6-108">Return Type</span></span>    |<span data-ttu-id="b07c6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b07c6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b07c6-110">Create inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="b07c6-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="b07c6-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="b07c6-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="b07c6-p101">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="b07c6-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="b07c6-114">List overrides</span><span class="sxs-lookup"><span data-stu-id="b07c6-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="b07c6-115">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="b07c6-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="b07c6-116">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="b07c6-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="b07c6-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b07c6-117">Properties</span></span>
| <span data-ttu-id="b07c6-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b07c6-118">Property</span></span>     | <span data-ttu-id="b07c6-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="b07c6-119">Type</span></span>   |<span data-ttu-id="b07c6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b07c6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b07c6-121">id</span><span class="sxs-lookup"><span data-stu-id="b07c6-121">id</span></span>|<span data-ttu-id="b07c6-122">string</span><span class="sxs-lookup"><span data-stu-id="b07c6-122">string</span></span>| <span data-ttu-id="b07c6-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b07c6-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b07c6-124">Relações</span><span class="sxs-lookup"><span data-stu-id="b07c6-124">Relationships</span></span>
| <span data-ttu-id="b07c6-125">Relação</span><span class="sxs-lookup"><span data-stu-id="b07c6-125">Relationship</span></span> | <span data-ttu-id="b07c6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="b07c6-126">Type</span></span>   |<span data-ttu-id="b07c6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="b07c6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b07c6-128">overrides</span><span class="sxs-lookup"><span data-stu-id="b07c6-128">overrides</span></span>|<span data-ttu-id="b07c6-129">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="b07c6-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="b07c6-p102">Um conjunto de substituições para um usuário sempre classificar mensagens a partir de remetentes específicos, de maneiras específicas: `focused`, ou `other`. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b07c6-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b07c6-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b07c6-133">JSON representation</span></span>

<span data-ttu-id="b07c6-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b07c6-134">Here is a JSON representation of the resource.</span></span>

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
