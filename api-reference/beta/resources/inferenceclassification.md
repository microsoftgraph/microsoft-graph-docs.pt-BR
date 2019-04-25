---
title: Tipo de recurso inferenceClassification
description: 'Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário. '
localization_priority: Normal
ms.openlocfilehash: f06177db9907deb3be38c2cdab82669764503cd6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549039"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="d641a-103">Tipo de recurso inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="d641a-103">inferenceClassification resource type</span></span>

<span data-ttu-id="d641a-104">Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d641a-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="d641a-105">Para saber mais, consulte [Gerenciar a Caixa de Entrada Prioritária](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="d641a-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="d641a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d641a-106">Methods</span></span>

| <span data-ttu-id="d641a-107">Método</span><span class="sxs-lookup"><span data-stu-id="d641a-107">Method</span></span>           | <span data-ttu-id="d641a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d641a-108">Return Type</span></span>    |<span data-ttu-id="d641a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d641a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d641a-110">Create inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="d641a-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="d641a-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="d641a-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="d641a-p101">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="d641a-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="d641a-114">List overrides</span><span class="sxs-lookup"><span data-stu-id="d641a-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="d641a-115">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="d641a-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="d641a-116">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="d641a-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="d641a-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d641a-117">Properties</span></span>
| <span data-ttu-id="d641a-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d641a-118">Property</span></span>     | <span data-ttu-id="d641a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="d641a-119">Type</span></span>   |<span data-ttu-id="d641a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d641a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d641a-121">id</span><span class="sxs-lookup"><span data-stu-id="d641a-121">id</span></span>|<span data-ttu-id="d641a-122">string</span><span class="sxs-lookup"><span data-stu-id="d641a-122">string</span></span>| <span data-ttu-id="d641a-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d641a-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d641a-124">Relações</span><span class="sxs-lookup"><span data-stu-id="d641a-124">Relationships</span></span>
| <span data-ttu-id="d641a-125">Relação</span><span class="sxs-lookup"><span data-stu-id="d641a-125">Relationship</span></span> | <span data-ttu-id="d641a-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d641a-126">Type</span></span>   |<span data-ttu-id="d641a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d641a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d641a-128">overrides</span><span class="sxs-lookup"><span data-stu-id="d641a-128">overrides</span></span>|<span data-ttu-id="d641a-129">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="d641a-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="d641a-p102">Um conjunto de substituições para um usuário sempre classificar mensagens a partir de remetentes específicos, de maneiras específicas: `focused`, ou `other`. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="d641a-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d641a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d641a-133">JSON representation</span></span>

<span data-ttu-id="d641a-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d641a-134">Here is a JSON representation of the resource.</span></span>

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
