---
title: tipo de recurso chatInfo
description: Informações sobre uma mensagem no Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c1414d10a262280bcf0d3a307fc0c71aed2fbde
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461068"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="f2d99-103">tipo de recurso chatInfo</span><span class="sxs-lookup"><span data-stu-id="f2d99-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2d99-104">Informações sobre uma mensagem no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f2d99-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="f2d99-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2d99-105">Properties</span></span>

| <span data-ttu-id="f2d99-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2d99-106">Property</span></span>            | <span data-ttu-id="f2d99-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2d99-107">Type</span></span>    | <span data-ttu-id="f2d99-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2d99-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="f2d99-109">messageId</span><span class="sxs-lookup"><span data-stu-id="f2d99-109">messageId</span></span>           | <span data-ttu-id="f2d99-110">String</span><span class="sxs-lookup"><span data-stu-id="f2d99-110">String</span></span>  | <span data-ttu-id="f2d99-111">O identificador exclusivo de uma mensagem em um canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f2d99-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="f2d99-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="f2d99-112">replyChainMessageId</span></span> | <span data-ttu-id="f2d99-113">String</span><span class="sxs-lookup"><span data-stu-id="f2d99-113">String</span></span>  | <span data-ttu-id="f2d99-114">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="f2d99-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="f2d99-115">threadId</span><span class="sxs-lookup"><span data-stu-id="f2d99-115">threadId</span></span>            | <span data-ttu-id="f2d99-116">String</span><span class="sxs-lookup"><span data-stu-id="f2d99-116">String</span></span>  | <span data-ttu-id="f2d99-117">O identificador exclusivo de um thread no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f2d99-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2d99-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2d99-118">JSON representation</span></span>

<span data-ttu-id="f2d99-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2d99-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatInfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
