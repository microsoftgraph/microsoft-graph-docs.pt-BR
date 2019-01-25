---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância da entidade, por exemplo, uma mensagem destinatário ou calendário proprietário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bc1f00ab09ac71f4f3cd9eb1aff8163a537ce257
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518664"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="a5a6a-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="a5a6a-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5a6a-104">Representa o nome e o endereço SMTP de uma instância da entidade, por exemplo, uma mensagem destinatário ou calendário proprietário.</span><span class="sxs-lookup"><span data-stu-id="a5a6a-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="a5a6a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5a6a-105">Properties</span></span>
| <span data-ttu-id="a5a6a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5a6a-106">Property</span></span>     | <span data-ttu-id="a5a6a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5a6a-107">Type</span></span>   |<span data-ttu-id="a5a6a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5a6a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5a6a-109">address</span><span class="sxs-lookup"><span data-stu-id="a5a6a-109">address</span></span>|<span data-ttu-id="a5a6a-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5a6a-110">String</span></span>|<span data-ttu-id="a5a6a-111">O endereço de email de uma instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="a5a6a-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="a5a6a-112">name</span><span class="sxs-lookup"><span data-stu-id="a5a6a-112">name</span></span>|<span data-ttu-id="a5a6a-113">String</span><span class="sxs-lookup"><span data-stu-id="a5a6a-113">String</span></span>|<span data-ttu-id="a5a6a-114">O nome de exibição de uma instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="a5a6a-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5a6a-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5a6a-115">JSON representation</span></span>

<span data-ttu-id="a5a6a-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a5a6a-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/emailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
