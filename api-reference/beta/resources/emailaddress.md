---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário de mensagem ou proprietário do calendário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4f0b36d84ffba5c5a8e39bd7603f92c815cda008
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972212"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="0f03f-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="0f03f-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f03f-104">Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário de mensagem ou proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="0f03f-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="0f03f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f03f-105">Properties</span></span>
| <span data-ttu-id="0f03f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f03f-106">Property</span></span>     | <span data-ttu-id="0f03f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f03f-107">Type</span></span>   |<span data-ttu-id="0f03f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f03f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f03f-109">address</span><span class="sxs-lookup"><span data-stu-id="0f03f-109">address</span></span>|<span data-ttu-id="0f03f-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f03f-110">String</span></span>|<span data-ttu-id="0f03f-111">O endereço de email de uma instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0f03f-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="0f03f-112">name</span><span class="sxs-lookup"><span data-stu-id="0f03f-112">name</span></span>|<span data-ttu-id="0f03f-113">String</span><span class="sxs-lookup"><span data-stu-id="0f03f-113">String</span></span>|<span data-ttu-id="0f03f-114">O nome de exibição de uma instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="0f03f-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f03f-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f03f-115">JSON representation</span></span>

<span data-ttu-id="0f03f-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="0f03f-116">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
