---
title: tipo de recurso de typedEmailAddress
description: Representa o nome, endereços de email e seu correspondente tipo de endereço de email de um contato.
localization_priority: Normal
ms.openlocfilehash: 3b1230dabc1e49c6cb9220eea95f0c3b93053d96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510705"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="3df6b-103">tipo de recurso de typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3df6b-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3df6b-104">Representa o nome, endereços de email e seu correspondente tipo de endereço de email de um [contato](contact.md).</span><span class="sxs-lookup"><span data-stu-id="3df6b-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3df6b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3df6b-105">Properties</span></span>
| <span data-ttu-id="3df6b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3df6b-106">Property</span></span>     | <span data-ttu-id="3df6b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3df6b-107">Type</span></span>   |<span data-ttu-id="3df6b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3df6b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3df6b-109">address</span><span class="sxs-lookup"><span data-stu-id="3df6b-109">address</span></span>|<span data-ttu-id="3df6b-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3df6b-110">String</span></span>|<span data-ttu-id="3df6b-111">O endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="3df6b-111">The email address of a contact.</span></span>|
|<span data-ttu-id="3df6b-112">name</span><span class="sxs-lookup"><span data-stu-id="3df6b-112">name</span></span>|<span data-ttu-id="3df6b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3df6b-113">String</span></span>|<span data-ttu-id="3df6b-114">O nome de exibição de um contato.</span><span class="sxs-lookup"><span data-stu-id="3df6b-114">The display name of a contact.</span></span>|
|<span data-ttu-id="3df6b-115">type</span><span class="sxs-lookup"><span data-stu-id="3df6b-115">type</span></span> |<span data-ttu-id="3df6b-116">String</span><span class="sxs-lookup"><span data-stu-id="3df6b-116">String</span></span> |<span data-ttu-id="3df6b-117">O tipo de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="3df6b-117">The type of email address.</span></span> <span data-ttu-id="3df6b-118">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="3df6b-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="3df6b-119">O valor padrão é `unknown`, que significa que o **endereço** não tiver sido definida como um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="3df6b-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="3df6b-120">otherLabel</span><span class="sxs-lookup"><span data-stu-id="3df6b-120">otherLabel</span></span> |<span data-ttu-id="3df6b-121">String</span><span class="sxs-lookup"><span data-stu-id="3df6b-121">String</span></span>  |<span data-ttu-id="3df6b-122">Para especificar um tipo personalizado de endereço de email, defina o **tipo** como `other`e atribuir **otherLabel** a uma cadeia de caracteres personalizada.</span><span class="sxs-lookup"><span data-stu-id="3df6b-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="3df6b-123">Por exemplo, você pode usar um endereço de email específica para suas atividades voluntárias.</span><span class="sxs-lookup"><span data-stu-id="3df6b-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="3df6b-124">Definir **tipo** `other`e configurado **otherLabel** como uma cadeia de caracteres personalizada como `Volunteer work`.</span><span class="sxs-lookup"><span data-stu-id="3df6b-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3df6b-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3df6b-125">JSON representation</span></span>

<span data-ttu-id="3df6b-126">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3df6b-126">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.typedEmailAddress"
}-->

```json
{
  "address": "string",
  "name": "string",
  "type": "string",
  "otherLabel": "string"
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
    "Error: /api-reference/beta/resources/typedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
