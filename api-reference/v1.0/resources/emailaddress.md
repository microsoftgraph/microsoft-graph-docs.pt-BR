---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
localization_priority: Normal
ms.openlocfilehash: 5ea1919e5c5f389c9b7fece508e8339f722b725a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826878"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="b8889-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="b8889-103">emailAddress resource type</span></span>

<span data-ttu-id="b8889-104">O nome e o endereço de email de um destinatário da mensagem ou contato.</span><span class="sxs-lookup"><span data-stu-id="b8889-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="b8889-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8889-105">Properties</span></span>
| <span data-ttu-id="b8889-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8889-106">Property</span></span>     | <span data-ttu-id="b8889-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8889-107">Type</span></span>   |<span data-ttu-id="b8889-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8889-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8889-109">address</span><span class="sxs-lookup"><span data-stu-id="b8889-109">address</span></span>|<span data-ttu-id="b8889-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8889-110">String</span></span>|<span data-ttu-id="b8889-111">O endereço de email da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="b8889-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="b8889-112">name</span><span class="sxs-lookup"><span data-stu-id="b8889-112">name</span></span>|<span data-ttu-id="b8889-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b8889-113">String</span></span>|<span data-ttu-id="b8889-114">O nome de exibição da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="b8889-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8889-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8889-115">JSON representation</span></span>

<span data-ttu-id="b8889-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b8889-116">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
