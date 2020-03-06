---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5e22b568ba05808fc9a87257686afd540145b3ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531479"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="679ff-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="679ff-103">emailAddress resource type</span></span>

<span data-ttu-id="679ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="679ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="679ff-105">O nome e o endereço de email de um destinatário da mensagem ou contato.</span><span class="sxs-lookup"><span data-stu-id="679ff-105">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="679ff-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="679ff-106">Properties</span></span>
| <span data-ttu-id="679ff-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="679ff-107">Property</span></span>     | <span data-ttu-id="679ff-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="679ff-108">Type</span></span>   |<span data-ttu-id="679ff-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="679ff-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="679ff-110">address</span><span class="sxs-lookup"><span data-stu-id="679ff-110">address</span></span>|<span data-ttu-id="679ff-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="679ff-111">String</span></span>|<span data-ttu-id="679ff-112">O endereço de email da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="679ff-112">The email address of the person or entity.</span></span>|
|<span data-ttu-id="679ff-113">nome</span><span class="sxs-lookup"><span data-stu-id="679ff-113">name</span></span>|<span data-ttu-id="679ff-114">String</span><span class="sxs-lookup"><span data-stu-id="679ff-114">String</span></span>|<span data-ttu-id="679ff-115">O nome de exibição da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="679ff-115">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="679ff-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="679ff-116">JSON representation</span></span>

<span data-ttu-id="679ff-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="679ff-117">Here is a JSON representation of the resource</span></span>

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
