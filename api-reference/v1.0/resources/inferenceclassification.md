---
title: Tipo de recurso inferenceClassification
description: 'Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário. '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 894deaf58f8e2e6466a6670caadb1d587b2a227a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531311"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="5b0ba-103">Tipo de recurso inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="5b0ba-103">inferenceClassification resource type</span></span>

<span data-ttu-id="5b0ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b0ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5b0ba-105">Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário.</span><span class="sxs-lookup"><span data-stu-id="5b0ba-105">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="5b0ba-106">Para saber mais, consulte [Gerenciar a Caixa de Entrada Prioritária](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="5b0ba-106">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="5b0ba-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5b0ba-107">Methods</span></span>

| <span data-ttu-id="5b0ba-108">Método</span><span class="sxs-lookup"><span data-stu-id="5b0ba-108">Method</span></span>           | <span data-ttu-id="5b0ba-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5b0ba-109">Return Type</span></span>    |<span data-ttu-id="5b0ba-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b0ba-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b0ba-111">Create inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="5b0ba-111">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="5b0ba-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="5b0ba-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="5b0ba-p101">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="5b0ba-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="5b0ba-115">List overrides</span><span class="sxs-lookup"><span data-stu-id="5b0ba-115">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="5b0ba-116">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="5b0ba-116">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="5b0ba-117">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="5b0ba-117">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="5b0ba-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b0ba-118">Properties</span></span>
| <span data-ttu-id="5b0ba-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b0ba-119">Property</span></span>     | <span data-ttu-id="5b0ba-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b0ba-120">Type</span></span>   |<span data-ttu-id="5b0ba-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b0ba-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b0ba-122">id</span><span class="sxs-lookup"><span data-stu-id="5b0ba-122">id</span></span>|<span data-ttu-id="5b0ba-123">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b0ba-123">string</span></span>| <span data-ttu-id="5b0ba-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b0ba-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b0ba-125">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="5b0ba-125">Relationships</span></span>
| <span data-ttu-id="5b0ba-126">Relação</span><span class="sxs-lookup"><span data-stu-id="5b0ba-126">Relationship</span></span> | <span data-ttu-id="5b0ba-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b0ba-127">Type</span></span>   |<span data-ttu-id="5b0ba-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b0ba-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b0ba-129">overrides</span><span class="sxs-lookup"><span data-stu-id="5b0ba-129">overrides</span></span>|<span data-ttu-id="5b0ba-130">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="5b0ba-130">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="5b0ba-p102">Um conjunto de substituições para um usuário sempre classificar mensagens a partir de remetentes específicos, de maneiras específicas: `focused`, ou `other`. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="5b0ba-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b0ba-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b0ba-134">JSON representation</span></span>

<span data-ttu-id="5b0ba-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b0ba-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
