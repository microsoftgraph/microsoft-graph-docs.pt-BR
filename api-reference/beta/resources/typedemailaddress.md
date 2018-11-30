---
title: tipo de recurso de typedEmailAddress
description: Representa o nome, endereços de email e seu correspondente tipo de endereço de email de um contato.
ms.openlocfilehash: 3f40add32fbc219606b6d78041552fc108803d1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041071"
---
# <a name="typedemailaddress-resource-type"></a><span data-ttu-id="72b76-103">tipo de recurso de typedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="72b76-103">typedEmailAddress resource type</span></span>

> <span data-ttu-id="72b76-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="72b76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72b76-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="72b76-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72b76-106">Representa o nome, endereços de email e seu correspondente tipo de endereço de email de um [contato](contact.md).</span><span class="sxs-lookup"><span data-stu-id="72b76-106">Represents the name, email addresses, and their corresponding email address type of a [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="72b76-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72b76-107">Properties</span></span>
| <span data-ttu-id="72b76-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72b76-108">Property</span></span>     | <span data-ttu-id="72b76-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="72b76-109">Type</span></span>   |<span data-ttu-id="72b76-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="72b76-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72b76-111">address</span><span class="sxs-lookup"><span data-stu-id="72b76-111">address</span></span>|<span data-ttu-id="72b76-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b76-112">String</span></span>|<span data-ttu-id="72b76-113">O endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="72b76-113">The email address of a contact.</span></span>|
|<span data-ttu-id="72b76-114">name</span><span class="sxs-lookup"><span data-stu-id="72b76-114">name</span></span>|<span data-ttu-id="72b76-115">String</span><span class="sxs-lookup"><span data-stu-id="72b76-115">String</span></span>|<span data-ttu-id="72b76-116">O nome de exibição de um contato.</span><span class="sxs-lookup"><span data-stu-id="72b76-116">The display name of a contact.</span></span>|
|<span data-ttu-id="72b76-117">type</span><span class="sxs-lookup"><span data-stu-id="72b76-117">type</span></span> |<span data-ttu-id="72b76-118">String</span><span class="sxs-lookup"><span data-stu-id="72b76-118">String</span></span> |<span data-ttu-id="72b76-119">O tipo de endereço de email.</span><span class="sxs-lookup"><span data-stu-id="72b76-119">The type of email address.</span></span> <span data-ttu-id="72b76-120">Os valores possíveis são: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="72b76-120">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span> <span data-ttu-id="72b76-121">O valor padrão é `unknown`, que significa que o **endereço** não tiver sido definida como um tipo específico.</span><span class="sxs-lookup"><span data-stu-id="72b76-121">The default value is `unknown`, which means **address** has not been set as a specific type.</span></span> |
|<span data-ttu-id="72b76-122">otherLabel</span><span class="sxs-lookup"><span data-stu-id="72b76-122">otherLabel</span></span> |<span data-ttu-id="72b76-123">String</span><span class="sxs-lookup"><span data-stu-id="72b76-123">String</span></span>  |<span data-ttu-id="72b76-124">Para especificar um tipo personalizado de endereço de email, defina o **tipo** como `other`e atribuir **otherLabel** a uma cadeia de caracteres personalizada.</span><span class="sxs-lookup"><span data-stu-id="72b76-124">To specify a custom type of email address, set **type** to `other`, and assign **otherLabel** to a custom string.</span></span> <span data-ttu-id="72b76-125">Por exemplo, você pode usar um endereço de email específica para suas atividades voluntárias.</span><span class="sxs-lookup"><span data-stu-id="72b76-125">For example, you may use a specific email address for your volunteer activities.</span></span> <span data-ttu-id="72b76-126">Definir **tipo** `other`e configurado **otherLabel** como uma cadeia de caracteres personalizada como `Volunteer work`.</span><span class="sxs-lookup"><span data-stu-id="72b76-126">Set **type** to `other`, and set **otherLabel** to a custom string such as `Volunteer work`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="72b76-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72b76-127">JSON representation</span></span>

<span data-ttu-id="72b76-128">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="72b76-128">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
