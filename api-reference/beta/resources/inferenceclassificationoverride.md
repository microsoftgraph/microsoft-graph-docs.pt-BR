---
title: Tipo de recurso inferenceClassificationOverride
description: Representa a substituição de um usuário sobre como as mensagens de entrada de um remetente específico devem sempre ser classificadas como
localization_priority: Normal
ms.openlocfilehash: 1cf1896b43dccfe59ed253c22a8a7341e9ee6e1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548730"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="7b306-103">Tipo de recurso inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="7b306-103">inferenceClassificationOverride resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b306-104">Representa a substituição de um usuário sobre como as mensagens de entrada de um remetente específico devem sempre ser classificadas como em uma [caixa de entrada destaques](manage-focused-inbox.md).</span><span class="sxs-lookup"><span data-stu-id="7b306-104">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="7b306-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7b306-105">Methods</span></span>

| <span data-ttu-id="7b306-106">Método</span><span class="sxs-lookup"><span data-stu-id="7b306-106">Method</span></span>           | <span data-ttu-id="7b306-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7b306-107">Return Type</span></span>    |<span data-ttu-id="7b306-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b306-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b306-109">Update</span><span class="sxs-lookup"><span data-stu-id="7b306-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="7b306-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="7b306-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="7b306-111">Altere o campo **ClassifyAs** de uma substituição conforme especificado.</span><span class="sxs-lookup"><span data-stu-id="7b306-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="7b306-112">Excluir</span><span class="sxs-lookup"><span data-stu-id="7b306-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="7b306-113">None</span><span class="sxs-lookup"><span data-stu-id="7b306-113">None</span></span> |<span data-ttu-id="7b306-114">Exclua uma substituição especificada de acordo com sua ID.</span><span class="sxs-lookup"><span data-stu-id="7b306-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="7b306-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b306-115">Properties</span></span>
| <span data-ttu-id="7b306-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b306-116">Property</span></span>     | <span data-ttu-id="7b306-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b306-117">Type</span></span>   |<span data-ttu-id="7b306-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b306-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b306-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="7b306-119">classifyAs</span></span>|<span data-ttu-id="7b306-120">string</span><span class="sxs-lookup"><span data-stu-id="7b306-120">string</span></span>| <span data-ttu-id="7b306-p101">Representa como classificar as mensagens recebidas de um remetente específico. Os valores possíveis são: `focused` e `other`.</span><span class="sxs-lookup"><span data-stu-id="7b306-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="7b306-123">id</span><span class="sxs-lookup"><span data-stu-id="7b306-123">id</span></span>|<span data-ttu-id="7b306-124">string</span><span class="sxs-lookup"><span data-stu-id="7b306-124">string</span></span>| <span data-ttu-id="7b306-p102">O identificador exclusivo da substituição. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7b306-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="7b306-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7b306-127">senderEmailAddress</span></span>|[<span data-ttu-id="7b306-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7b306-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="7b306-129">As informações de endereço de email do remetente para quem a substituição é criada.</span><span class="sxs-lookup"><span data-stu-id="7b306-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b306-130">Relações</span><span class="sxs-lookup"><span data-stu-id="7b306-130">Relationships</span></span>
<span data-ttu-id="7b306-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7b306-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7b306-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b306-132">JSON representation</span></span>

<span data-ttu-id="7b306-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b306-133">Here is a JSON representation of the resource.</span></span>

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
