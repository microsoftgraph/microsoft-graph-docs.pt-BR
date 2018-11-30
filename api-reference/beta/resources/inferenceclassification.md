---
title: Tipo de recurso inferenceClassification
description: 'Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário. '
ms.openlocfilehash: c1536ff2b88b1830c2f2a2bc5a7bed519782df4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033029"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="cd2e6-103">Tipo de recurso inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="cd2e6-103">inferenceClassification resource type</span></span>

> <span data-ttu-id="cd2e6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd2e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd2e6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd2e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd2e6-106">Classificação das mensagens de um usuário para possibilitar a atenção nas mensagens que são mais relevantes ou importantes para o usuário.</span><span class="sxs-lookup"><span data-stu-id="cd2e6-106">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="cd2e6-107">Para saber mais, consulte [Gerenciar a Caixa de Entrada Prioritária](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="cd2e6-107">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="cd2e6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd2e6-108">Methods</span></span>

| <span data-ttu-id="cd2e6-109">Método</span><span class="sxs-lookup"><span data-stu-id="cd2e6-109">Method</span></span>           | <span data-ttu-id="cd2e6-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd2e6-110">Return Type</span></span>    |<span data-ttu-id="cd2e6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2e6-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd2e6-112">Create inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="cd2e6-112">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="cd2e6-113">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="cd2e6-113">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="cd2e6-p102">Crie uma substituição para um remetente identificado por um endereço SMTP. Mensagens futuras desse endereço SMTP serão consistentemente classificadas conforme especificado na substituição.</span><span class="sxs-lookup"><span data-stu-id="cd2e6-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="cd2e6-116">List overrides</span><span class="sxs-lookup"><span data-stu-id="cd2e6-116">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="cd2e6-117">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="cd2e6-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="cd2e6-118">Obtenha as substituições que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.</span><span class="sxs-lookup"><span data-stu-id="cd2e6-118">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd2e6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd2e6-119">Properties</span></span>
| <span data-ttu-id="cd2e6-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd2e6-120">Property</span></span>     | <span data-ttu-id="cd2e6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd2e6-121">Type</span></span>   |<span data-ttu-id="cd2e6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2e6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd2e6-123">id</span><span class="sxs-lookup"><span data-stu-id="cd2e6-123">id</span></span>|<span data-ttu-id="cd2e6-124">string</span><span class="sxs-lookup"><span data-stu-id="cd2e6-124">string</span></span>| <span data-ttu-id="cd2e6-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd2e6-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd2e6-126">Relações</span><span class="sxs-lookup"><span data-stu-id="cd2e6-126">Relationships</span></span>
| <span data-ttu-id="cd2e6-127">Relação</span><span class="sxs-lookup"><span data-stu-id="cd2e6-127">Relationship</span></span> | <span data-ttu-id="cd2e6-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd2e6-128">Type</span></span>   |<span data-ttu-id="cd2e6-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2e6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd2e6-130">overrides</span><span class="sxs-lookup"><span data-stu-id="cd2e6-130">overrides</span></span>|<span data-ttu-id="cd2e6-131">Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md)</span><span class="sxs-lookup"><span data-stu-id="cd2e6-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="cd2e6-p103">Um conjunto de substituições para um usuário sempre classificar mensagens a partir de remetentes específicos, de maneiras específicas: `focused`, ou `other`. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="cd2e6-p103">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd2e6-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd2e6-135">JSON representation</span></span>

<span data-ttu-id="cd2e6-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd2e6-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->