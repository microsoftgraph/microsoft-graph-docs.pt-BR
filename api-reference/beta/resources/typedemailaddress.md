---
title: tipo de recurso typedEmailAddress
description: Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um contato.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7d6c064e7a87b0e9c776a5691f24b48dfff56422
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519628"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="7a1fe-103">tipo de recurso typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7a1fe-103">typedEmailAddress resource type</span></span>

<span data-ttu-id="7a1fe-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7a1fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a1fe-105">Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um [contato](contact.md).</span><span class="sxs-lookup"><span data-stu-id="7a1fe-105">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7a1fe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a1fe-106">Properties</span></span>
| <span data-ttu-id="7a1fe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a1fe-107">Property</span></span>     | <span data-ttu-id="7a1fe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a1fe-108">Type</span></span>   |<span data-ttu-id="7a1fe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a1fe-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a1fe-110">address</span><span class="sxs-lookup"><span data-stu-id="7a1fe-110">address</span></span>|<span data-ttu-id="7a1fe-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a1fe-111">String</span></span>|<span data-ttu-id="7a1fe-112">O endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="7a1fe-112">The email address of a contact.</span></span>|
|<span data-ttu-id="7a1fe-113">nome</span><span class="sxs-lookup"><span data-stu-id="7a1fe-113">name</span></span>|<span data-ttu-id="7a1fe-114">String</span><span class="sxs-lookup"><span data-stu-id="7a1fe-114">String</span></span>|<span data-ttu-id="7a1fe-115">O nome de exibição de um contato.</span><span class="sxs-lookup"><span data-stu-id="7a1fe-115">The display name of a contact.</span></span>|
|<span data-ttu-id="7a1fe-116">type</span><span class="sxs-lookup"><span data-stu-id="7a1fe-116">type</span></span> |<span data-ttu-id="7a1fe-117">String</span><span class="sxs-lookup"><span data-stu-id="7a1fe-117">String</span></span> |<span data-ttu-id="7a1fe-118">O tipo de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="7a1fe-118">The type of email address.</span></span> <span data-ttu-id="7a1fe-119">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="7a1fe-119">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="7a1fe-120">O valor padrão é `unknown`, o que significa que o **endereço** não foi definido como um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="7a1fe-120">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="7a1fe-121">otherLabel</span><span class="sxs-lookup"><span data-stu-id="7a1fe-121">otherLabel</span></span> |<span data-ttu-id="7a1fe-122">String</span><span class="sxs-lookup"><span data-stu-id="7a1fe-122">String</span></span>  |<span data-ttu-id="7a1fe-123">Para especificar um tipo personalizado de endereço de email, \*\*\*\* defina Type `other`como e atribua **otherLabel** a uma cadeia de caracteres personalizada.</span><span class="sxs-lookup"><span data-stu-id="7a1fe-123">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="7a1fe-124">Por exemplo, você pode usar um endereço de email específico para suas atividades de voluntários.</span><span class="sxs-lookup"><span data-stu-id="7a1fe-124">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="7a1fe-125">Defina \*\*\*\* o tipo `other`como e defina **otherLabel** como uma cadeia de caracteres personalizada `Volunteer work`, como.</span><span class="sxs-lookup"><span data-stu-id="7a1fe-125">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a1fe-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a1fe-126">JSON representation</span></span>

<span data-ttu-id="7a1fe-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7a1fe-127">Here is a JSON representation of the resource</span></span>

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
