---
title: Tipo de recurso emailAddress
description: O nome e o endereço de email de um destinatário da mensagem ou contato.
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 52332c04591bc507416df325786f6f263fe7ca6e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069075"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="1b0ca-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="1b0ca-103">emailAddress resource type</span></span>

<span data-ttu-id="1b0ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b0ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b0ca-105">O nome e o endereço de email de um destinatário da mensagem ou contato.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-105">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="1b0ca-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b0ca-106">Properties</span></span>
| <span data-ttu-id="1b0ca-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b0ca-107">Property</span></span>     | <span data-ttu-id="1b0ca-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b0ca-108">Type</span></span>   |<span data-ttu-id="1b0ca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b0ca-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b0ca-110">address</span><span class="sxs-lookup"><span data-stu-id="1b0ca-110">address</span></span>|<span data-ttu-id="1b0ca-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b0ca-111">String</span></span>|<span data-ttu-id="1b0ca-112">O endereço de email da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-112">The email address of the person or entity.</span></span>|
|<span data-ttu-id="1b0ca-113">nome</span><span class="sxs-lookup"><span data-stu-id="1b0ca-113">name</span></span>|<span data-ttu-id="1b0ca-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b0ca-114">String</span></span>|<span data-ttu-id="1b0ca-115">O nome de exibição da pessoa ou entidade.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-115">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b0ca-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b0ca-116">JSON representation</span></span>

<span data-ttu-id="1b0ca-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1b0ca-117">Here is a JSON representation of the resource</span></span>

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

