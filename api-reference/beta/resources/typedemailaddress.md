---
title: tipo de recurso typedEmailAddress
description: Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um contato.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c5ece5d1ad1c5c38253d73353b05b94727855fd5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007568"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="5ffa1-103">tipo de recurso typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5ffa1-103">typedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ffa1-104">Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um [contato](contact.md).</span><span class="sxs-lookup"><span data-stu-id="5ffa1-104">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5ffa1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ffa1-105">Properties</span></span>
| <span data-ttu-id="5ffa1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ffa1-106">Property</span></span>     | <span data-ttu-id="5ffa1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ffa1-107">Type</span></span>   |<span data-ttu-id="5ffa1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ffa1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ffa1-109">address</span><span class="sxs-lookup"><span data-stu-id="5ffa1-109">address</span></span>|<span data-ttu-id="5ffa1-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ffa1-110">String</span></span>|<span data-ttu-id="5ffa1-111">O endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="5ffa1-111">The email address of a contact.</span></span>|
|<span data-ttu-id="5ffa1-112">name</span><span class="sxs-lookup"><span data-stu-id="5ffa1-112">name</span></span>|<span data-ttu-id="5ffa1-113">String</span><span class="sxs-lookup"><span data-stu-id="5ffa1-113">String</span></span>|<span data-ttu-id="5ffa1-114">O nome de exibição de um contato.</span><span class="sxs-lookup"><span data-stu-id="5ffa1-114">The display name of a contact.</span></span>|
|<span data-ttu-id="5ffa1-115">type</span><span class="sxs-lookup"><span data-stu-id="5ffa1-115">type</span></span> |<span data-ttu-id="5ffa1-116">String</span><span class="sxs-lookup"><span data-stu-id="5ffa1-116">String</span></span> |<span data-ttu-id="5ffa1-117">O tipo de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="5ffa1-117">The type of email address.</span></span> <span data-ttu-id="5ffa1-118">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="5ffa1-118">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="5ffa1-119">O valor padrão é `unknown`, o que significa que o **endereço** não foi definido como um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="5ffa1-119">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="5ffa1-120">otherLabel</span><span class="sxs-lookup"><span data-stu-id="5ffa1-120">otherLabel</span></span> |<span data-ttu-id="5ffa1-121">String</span><span class="sxs-lookup"><span data-stu-id="5ffa1-121">String</span></span>  |<span data-ttu-id="5ffa1-122">Para especificar um tipo personalizado de endereço de email, \*\*\*\* defina Type `other`como e atribua **otherLabel** a uma cadeia de caracteres personalizada.</span><span class="sxs-lookup"><span data-stu-id="5ffa1-122">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="5ffa1-123">Por exemplo, você pode usar um endereço de email específico para suas atividades de voluntários.</span><span class="sxs-lookup"><span data-stu-id="5ffa1-123">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="5ffa1-124">Defina \*\*\*\* o tipo `other`como e defina **otherLabel** como uma cadeia de caracteres personalizada `Volunteer work`, como.</span><span class="sxs-lookup"><span data-stu-id="5ffa1-124">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5ffa1-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ffa1-125">JSON representation</span></span>

<span data-ttu-id="5ffa1-126">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="5ffa1-126">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
