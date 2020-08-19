---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c65bbecda618115e40a3c3cc36f2b952597b9c85
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808904"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="8912b-103">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="8912b-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="8912b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8912b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8912b-105">Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="8912b-105">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="8912b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8912b-106">Methods</span></span>

| <span data-ttu-id="8912b-107">Método</span><span class="sxs-lookup"><span data-stu-id="8912b-107">Method</span></span>           | <span data-ttu-id="8912b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8912b-108">Return Type</span></span>    |<span data-ttu-id="8912b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8912b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8912b-110">Update</span><span class="sxs-lookup"><span data-stu-id="8912b-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="8912b-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="8912b-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="8912b-112">Altere o campo **ClassifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="8912b-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="8912b-113">Delete</span><span class="sxs-lookup"><span data-stu-id="8912b-113">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="8912b-114">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8912b-114">None</span></span> |<span data-ttu-id="8912b-115">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="8912b-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="8912b-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8912b-116">Properties</span></span>
| <span data-ttu-id="8912b-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8912b-117">Property</span></span>     | <span data-ttu-id="8912b-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="8912b-118">Type</span></span>   |<span data-ttu-id="8912b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8912b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8912b-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="8912b-120">classifyAs</span></span>|<span data-ttu-id="8912b-121">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="8912b-121">inferenceClassificationType</span></span>| <span data-ttu-id="8912b-122">Representa como classificar as mensagens recebidas de um remetente específico.</span><span class="sxs-lookup"><span data-stu-id="8912b-122">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="8912b-123">Os valores possíveis são: `focused` , `other` .</span><span class="sxs-lookup"><span data-stu-id="8912b-123">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="8912b-124">id</span><span class="sxs-lookup"><span data-stu-id="8912b-124">id</span></span>|<span data-ttu-id="8912b-125">string</span><span class="sxs-lookup"><span data-stu-id="8912b-125">string</span></span>| <span data-ttu-id="8912b-p102">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8912b-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="8912b-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8912b-128">senderEmailAddress</span></span>|[<span data-ttu-id="8912b-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8912b-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="8912b-130">As informações de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="8912b-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8912b-131">Relações</span><span class="sxs-lookup"><span data-stu-id="8912b-131">Relationships</span></span>
<span data-ttu-id="8912b-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8912b-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8912b-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8912b-133">JSON representation</span></span>

<span data-ttu-id="8912b-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8912b-134">Here is a JSON representation of the resource.</span></span>

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
