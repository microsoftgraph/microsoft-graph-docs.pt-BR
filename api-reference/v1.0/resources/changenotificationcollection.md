---
title: Tipo de recurso changeNotificationCollection
description: Representa uma coleção de notificações de assinatura enviadas ao Assinante.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 1eadd0fbc14fe9e6581ab6fa3375837653fc0859
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598504"
---
# <a name="changenotificationcollection-resource-type"></a><span data-ttu-id="2693c-103">Tipo de recurso changeNotificationCollection</span><span class="sxs-lookup"><span data-stu-id="2693c-103">changeNotificationCollection resource type</span></span>

<span data-ttu-id="2693c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2693c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2693c-105">Representa uma coleção de notificações de alteração de recursos enviadas ao Assinante.</span><span class="sxs-lookup"><span data-stu-id="2693c-105">Represents a collection of resource change notifications sent to the subscriber.</span></span>

<span data-ttu-id="2693c-106">Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="2693c-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2693c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2693c-107">Methods</span></span>

<span data-ttu-id="2693c-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2693c-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="2693c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2693c-109">Properties</span></span>

| <span data-ttu-id="2693c-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2693c-110">Property</span></span> | <span data-ttu-id="2693c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2693c-111">Type</span></span> | <span data-ttu-id="2693c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2693c-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="2693c-113">valor</span><span class="sxs-lookup"><span data-stu-id="2693c-113">value</span></span> | <span data-ttu-id="2693c-114">coleção ([changeNotification](changenotification.md))</span><span class="sxs-lookup"><span data-stu-id="2693c-114">collection([changeNotification](changenotification.md))</span></span> | <span data-ttu-id="2693c-115">O conjunto de notificações que estão sendo enviadas à URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="2693c-115">The set of notifications being sent to the notification URL.</span></span> <span data-ttu-id="2693c-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2693c-116">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2693c-117">Relações</span><span class="sxs-lookup"><span data-stu-id="2693c-117">Relationships</span></span>

<span data-ttu-id="2693c-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2693c-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2693c-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2693c-119">JSON representation</span></span>

<span data-ttu-id="2693c-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2693c-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotificationCollection"
}-->

```json
{
  "value": [],
  "validationTokens": [
    "eyJ0eXAiOiJKV1QiLCJhbGciOiJSU..."
  ]
}
```

<!-- uuid: 8cc2599e-9740-4191-93fa-bc13c6f91564
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification collection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
