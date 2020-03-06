---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a80283bd3f32c28b71d02acd2ae93e76cac1299
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531307"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="89ea4-103">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="89ea4-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="89ea4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89ea4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89ea4-105">Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="89ea4-105">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="89ea4-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="89ea4-106">Methods</span></span>

| <span data-ttu-id="89ea4-107">Método</span><span class="sxs-lookup"><span data-stu-id="89ea4-107">Method</span></span>           | <span data-ttu-id="89ea4-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="89ea4-108">Return Type</span></span>    |<span data-ttu-id="89ea4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="89ea4-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89ea4-110">Update</span><span class="sxs-lookup"><span data-stu-id="89ea4-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="89ea4-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="89ea4-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="89ea4-112">Altere o campo **ClassifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="89ea4-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="89ea4-113">Excluir</span><span class="sxs-lookup"><span data-stu-id="89ea4-113">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="89ea4-114">None</span><span class="sxs-lookup"><span data-stu-id="89ea4-114">None</span></span> |<span data-ttu-id="89ea4-115">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="89ea4-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="89ea4-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89ea4-116">Properties</span></span>
| <span data-ttu-id="89ea4-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89ea4-117">Property</span></span>     | <span data-ttu-id="89ea4-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="89ea4-118">Type</span></span>   |<span data-ttu-id="89ea4-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="89ea4-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89ea4-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="89ea4-120">classifyAs</span></span>|<span data-ttu-id="89ea4-121">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="89ea4-121">inferenceClassificationType</span></span>| <span data-ttu-id="89ea4-122">Representa como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="89ea4-122">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="89ea4-123">Os valores possíveis são: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="89ea4-123">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="89ea4-124">id</span><span class="sxs-lookup"><span data-stu-id="89ea4-124">id</span></span>|<span data-ttu-id="89ea4-125">string</span><span class="sxs-lookup"><span data-stu-id="89ea4-125">string</span></span>| <span data-ttu-id="89ea4-p102">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="89ea4-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="89ea4-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="89ea4-128">senderEmailAddress</span></span>|[<span data-ttu-id="89ea4-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="89ea4-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="89ea4-130">As informações de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="89ea4-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89ea4-131">Relações</span><span class="sxs-lookup"><span data-stu-id="89ea4-131">Relationships</span></span>
<span data-ttu-id="89ea4-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89ea4-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="89ea4-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89ea4-133">JSON representation</span></span>

<span data-ttu-id="89ea4-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89ea4-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
