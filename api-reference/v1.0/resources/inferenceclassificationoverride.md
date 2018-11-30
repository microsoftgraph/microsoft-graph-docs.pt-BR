---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.
ms.openlocfilehash: 3f3f07e870a4ba549062197a380633ab591c54fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005245"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="8df5a-103">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="8df5a-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="8df5a-104">Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="8df5a-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="8df5a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="8df5a-105">Methods</span></span>

| <span data-ttu-id="8df5a-106">Método</span><span class="sxs-lookup"><span data-stu-id="8df5a-106">Method</span></span>           | <span data-ttu-id="8df5a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8df5a-107">Return Type</span></span>    |<span data-ttu-id="8df5a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8df5a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8df5a-109">Update</span><span class="sxs-lookup"><span data-stu-id="8df5a-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="8df5a-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="8df5a-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="8df5a-111">Altere o campo **ClassifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="8df5a-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="8df5a-112">Delete</span><span class="sxs-lookup"><span data-stu-id="8df5a-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="8df5a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8df5a-113">None</span></span> |<span data-ttu-id="8df5a-114">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="8df5a-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="8df5a-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8df5a-115">Properties</span></span>
| <span data-ttu-id="8df5a-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8df5a-116">Property</span></span>     | <span data-ttu-id="8df5a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="8df5a-117">Type</span></span>   |<span data-ttu-id="8df5a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8df5a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8df5a-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="8df5a-119">classifyAs</span></span>|<span data-ttu-id="8df5a-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="8df5a-120">inferenceClassificationType</span></span>| <span data-ttu-id="8df5a-121">Especifica como mensagens recebidas de uma determinada remetente deve sempre ser classificada como.</span><span class="sxs-lookup"><span data-stu-id="8df5a-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="8df5a-122">Os valores possíveis são: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="8df5a-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="8df5a-123">id</span><span class="sxs-lookup"><span data-stu-id="8df5a-123">id</span></span>|<span data-ttu-id="8df5a-124">string</span><span class="sxs-lookup"><span data-stu-id="8df5a-124">string</span></span>| <span data-ttu-id="8df5a-p102">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8df5a-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="8df5a-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8df5a-127">senderEmailAddress</span></span>|[<span data-ttu-id="8df5a-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8df5a-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="8df5a-129">As informações de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="8df5a-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8df5a-130">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="8df5a-130">Relationships</span></span>
<span data-ttu-id="8df5a-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8df5a-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8df5a-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8df5a-132">JSON representation</span></span>

<span data-ttu-id="8df5a-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8df5a-133">Here is a JSON representation of the resource.</span></span>

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