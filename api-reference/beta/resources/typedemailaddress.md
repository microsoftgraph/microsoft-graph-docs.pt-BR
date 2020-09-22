---
title: tipo de recurso typedEmailAddress
description: Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um contato.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kevinbellinger
ms.openlocfilehash: 8ce8ebdd0cb5b8b2113a80dacf72617d0f361356
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993004"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="24ce2-103">tipo de recurso typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="24ce2-103">typedEmailAddress resource type</span></span>

<span data-ttu-id="24ce2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24ce2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24ce2-105">Representa o nome, os endereços de email e o tipo de endereço de email correspondente de um [contato](contact.md).</span><span class="sxs-lookup"><span data-stu-id="24ce2-105">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="24ce2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24ce2-106">Properties</span></span>
| <span data-ttu-id="24ce2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24ce2-107">Property</span></span>     | <span data-ttu-id="24ce2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="24ce2-108">Type</span></span>   |<span data-ttu-id="24ce2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="24ce2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24ce2-110">address</span><span class="sxs-lookup"><span data-stu-id="24ce2-110">address</span></span>|<span data-ttu-id="24ce2-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24ce2-111">String</span></span>|<span data-ttu-id="24ce2-112">O endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="24ce2-112">The email address of a contact.</span></span>|
|<span data-ttu-id="24ce2-113">nome</span><span class="sxs-lookup"><span data-stu-id="24ce2-113">name</span></span>|<span data-ttu-id="24ce2-114">String</span><span class="sxs-lookup"><span data-stu-id="24ce2-114">String</span></span>|<span data-ttu-id="24ce2-115">O nome de exibição de um contato.</span><span class="sxs-lookup"><span data-stu-id="24ce2-115">The display name of a contact.</span></span>|
|<span data-ttu-id="24ce2-116">tipo</span><span class="sxs-lookup"><span data-stu-id="24ce2-116">type</span></span> |<span data-ttu-id="24ce2-117">String</span><span class="sxs-lookup"><span data-stu-id="24ce2-117">String</span></span> |<span data-ttu-id="24ce2-118">O tipo de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="24ce2-118">The type of email address.</span></span> <span data-ttu-id="24ce2-119">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="24ce2-119">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="24ce2-120">O valor padrão é `unknown` , o que significa que o **endereço** não foi definido como um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="24ce2-120">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="24ce2-121">otherLabel</span><span class="sxs-lookup"><span data-stu-id="24ce2-121">otherLabel</span></span> |<span data-ttu-id="24ce2-122">String</span><span class="sxs-lookup"><span data-stu-id="24ce2-122">String</span></span>  |<span data-ttu-id="24ce2-123">Para especificar um tipo personalizado de endereço de email, defina **Type** como `other` e atribua **otherLabel** a uma cadeia de caracteres personalizada.</span><span class="sxs-lookup"><span data-stu-id="24ce2-123">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="24ce2-124">Por exemplo, você pode usar um endereço de email específico para suas atividades de voluntários.</span><span class="sxs-lookup"><span data-stu-id="24ce2-124">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="24ce2-125">Defina o **tipo** como `other` e defina **otherLabel** como uma cadeia de caracteres personalizada, como `Volunteer work` .</span><span class="sxs-lookup"><span data-stu-id="24ce2-125">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24ce2-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24ce2-126">JSON representation</span></span>

<span data-ttu-id="24ce2-127">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="24ce2-127">Here is a JSON representation of the resource</span></span>

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


