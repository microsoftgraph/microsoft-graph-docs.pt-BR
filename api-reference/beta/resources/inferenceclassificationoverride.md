---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário para como as mensagens de entrada de um remetente específico sempre devem ser classificadas como
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 537032c220ed98fc9052afe6a31376359836fa94
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954983"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="4e23a-103">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4e23a-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="4e23a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e23a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e23a-105">Representa a substituição de um usuário para saber como as mensagens de entrada de um remetente específico sempre devem ser classificadas como em uma [Caixa de Entrada Focada.](manage-focused-inbox.md)</span><span class="sxs-lookup"><span data-stu-id="4e23a-105">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="4e23a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="4e23a-106">Methods</span></span>

| <span data-ttu-id="4e23a-107">Método</span><span class="sxs-lookup"><span data-stu-id="4e23a-107">Method</span></span>           | <span data-ttu-id="4e23a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4e23a-108">Return Type</span></span>    |<span data-ttu-id="4e23a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e23a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e23a-110">Update</span><span class="sxs-lookup"><span data-stu-id="4e23a-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="4e23a-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="4e23a-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="4e23a-112">Altere o campo **ClassifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="4e23a-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="4e23a-113">Delete</span><span class="sxs-lookup"><span data-stu-id="4e23a-113">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="4e23a-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e23a-114">None</span></span> |<span data-ttu-id="4e23a-115">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="4e23a-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="4e23a-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e23a-116">Properties</span></span>
| <span data-ttu-id="4e23a-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e23a-117">Property</span></span>     | <span data-ttu-id="4e23a-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e23a-118">Type</span></span>   |<span data-ttu-id="4e23a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e23a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e23a-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="4e23a-120">classifyAs</span></span>|<span data-ttu-id="4e23a-121">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="4e23a-121">inferenceClassificationType</span></span>| <span data-ttu-id="4e23a-p101">Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.</span><span class="sxs-lookup"><span data-stu-id="4e23a-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="4e23a-124">id</span><span class="sxs-lookup"><span data-stu-id="4e23a-124">id</span></span>|<span data-ttu-id="4e23a-125">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4e23a-125">string</span></span>| <span data-ttu-id="4e23a-p102">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4e23a-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="4e23a-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="4e23a-128">senderEmailAddress</span></span>|[<span data-ttu-id="4e23a-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4e23a-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="4e23a-130">As informações de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="4e23a-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e23a-131">Relações</span><span class="sxs-lookup"><span data-stu-id="4e23a-131">Relationships</span></span>
<span data-ttu-id="4e23a-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e23a-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4e23a-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e23a-133">JSON representation</span></span>

<span data-ttu-id="4e23a-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e23a-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


