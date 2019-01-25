---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário para definir como classificar as mensagens recebidas de um remetente específico.
localization_priority: Normal
ms.openlocfilehash: 1cf1896b43dccfe59ed253c22a8a7341e9ee6e1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511797"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="ebccb-103">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="ebccb-103">inferenceClassificationOverride resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebccb-104">Representa a substituição de um usuário para como mensagens recebidas de um remetente específico sempre devem ser classificadas como uma [Caixa de entrada com foco](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="ebccb-104">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="ebccb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ebccb-105">Methods</span></span>

| <span data-ttu-id="ebccb-106">Método</span><span class="sxs-lookup"><span data-stu-id="ebccb-106">Method</span></span>           | <span data-ttu-id="ebccb-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ebccb-107">Return Type</span></span>    |<span data-ttu-id="ebccb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebccb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ebccb-109">Update</span><span class="sxs-lookup"><span data-stu-id="ebccb-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="ebccb-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="ebccb-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="ebccb-111">Altere o campo **classifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="ebccb-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="ebccb-112">Delete</span><span class="sxs-lookup"><span data-stu-id="ebccb-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="ebccb-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebccb-113">None</span></span> |<span data-ttu-id="ebccb-114">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="ebccb-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="ebccb-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebccb-115">Properties</span></span>
| <span data-ttu-id="ebccb-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebccb-116">Property</span></span>     | <span data-ttu-id="ebccb-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebccb-117">Type</span></span>   |<span data-ttu-id="ebccb-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebccb-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ebccb-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="ebccb-119">classifyAs</span></span>|<span data-ttu-id="ebccb-120">string</span><span class="sxs-lookup"><span data-stu-id="ebccb-120">string</span></span>| <span data-ttu-id="ebccb-p101">Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.</span><span class="sxs-lookup"><span data-stu-id="ebccb-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="ebccb-123">id</span><span class="sxs-lookup"><span data-stu-id="ebccb-123">id</span></span>|<span data-ttu-id="ebccb-124">string</span><span class="sxs-lookup"><span data-stu-id="ebccb-124">string</span></span>| <span data-ttu-id="ebccb-p102">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ebccb-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="ebccb-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ebccb-127">senderEmailAddress</span></span>|[<span data-ttu-id="ebccb-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ebccb-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ebccb-129">As informações de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="ebccb-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebccb-130">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ebccb-130">Relationships</span></span>
<span data-ttu-id="ebccb-131">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ebccb-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ebccb-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebccb-132">JSON representation</span></span>

<span data-ttu-id="ebccb-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebccb-133">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/inferenceclassificationoverride.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
