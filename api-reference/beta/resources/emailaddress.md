---
title: Tipo de recurso emailAddress
description: Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário de mensagem ou proprietário do calendário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e8b49e0ff502f6e36e6ca3291d675c839e9ff5e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340298"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="3149d-103">Tipo de recurso emailAddress</span><span class="sxs-lookup"><span data-stu-id="3149d-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3149d-104">Representa o nome e o endereço SMTP de uma instância de entidade, por exemplo, um destinatário de mensagem ou proprietário do calendário.</span><span class="sxs-lookup"><span data-stu-id="3149d-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="3149d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3149d-105">Properties</span></span>
| <span data-ttu-id="3149d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3149d-106">Property</span></span>     | <span data-ttu-id="3149d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3149d-107">Type</span></span>   |<span data-ttu-id="3149d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3149d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3149d-109">address</span><span class="sxs-lookup"><span data-stu-id="3149d-109">address</span></span>|<span data-ttu-id="3149d-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3149d-110">String</span></span>|<span data-ttu-id="3149d-111">O endereço de email de uma instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3149d-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="3149d-112">name</span><span class="sxs-lookup"><span data-stu-id="3149d-112">name</span></span>|<span data-ttu-id="3149d-113">String</span><span class="sxs-lookup"><span data-stu-id="3149d-113">String</span></span>|<span data-ttu-id="3149d-114">O nome de exibição de uma instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3149d-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3149d-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3149d-115">JSON representation</span></span>

<span data-ttu-id="3149d-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3149d-116">Here is a JSON representation of the resource</span></span>

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
