---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.
localization_priority: Normal
ms.openlocfilehash: 8df0f1e5fa34c630c51de7c73234e6092448f867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885061"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="02b8f-103">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="02b8f-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="02b8f-104">Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="02b8f-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="02b8f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="02b8f-105">Methods</span></span>

| <span data-ttu-id="02b8f-106">Método</span><span class="sxs-lookup"><span data-stu-id="02b8f-106">Method</span></span>           | <span data-ttu-id="02b8f-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="02b8f-107">Return Type</span></span>    |<span data-ttu-id="02b8f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="02b8f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="02b8f-109">Update</span><span class="sxs-lookup"><span data-stu-id="02b8f-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="02b8f-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="02b8f-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="02b8f-111">Altere o campo **ClassifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="02b8f-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="02b8f-112">Delete</span><span class="sxs-lookup"><span data-stu-id="02b8f-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="02b8f-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="02b8f-113">None</span></span> |<span data-ttu-id="02b8f-114">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="02b8f-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="02b8f-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="02b8f-115">Properties</span></span>
| <span data-ttu-id="02b8f-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="02b8f-116">Property</span></span>     | <span data-ttu-id="02b8f-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="02b8f-117">Type</span></span>   |<span data-ttu-id="02b8f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="02b8f-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02b8f-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="02b8f-119">classifyAs</span></span>|<span data-ttu-id="02b8f-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="02b8f-120">inferenceClassificationType</span></span>| <span data-ttu-id="02b8f-121">Especifica como mensagens recebidas de uma determinada remetente deve sempre ser classificada como.</span><span class="sxs-lookup"><span data-stu-id="02b8f-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="02b8f-122">Os valores possíveis são: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="02b8f-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="02b8f-123">id</span><span class="sxs-lookup"><span data-stu-id="02b8f-123">id</span></span>|<span data-ttu-id="02b8f-124">string</span><span class="sxs-lookup"><span data-stu-id="02b8f-124">string</span></span>| <span data-ttu-id="02b8f-p102">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="02b8f-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="02b8f-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="02b8f-127">senderEmailAddress</span></span>|[<span data-ttu-id="02b8f-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="02b8f-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="02b8f-129">As informações de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="02b8f-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02b8f-130">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="02b8f-130">Relationships</span></span>
<span data-ttu-id="02b8f-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="02b8f-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="02b8f-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="02b8f-132">JSON representation</span></span>

<span data-ttu-id="02b8f-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="02b8f-133">Here is a JSON representation of the resource.</span></span>

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
