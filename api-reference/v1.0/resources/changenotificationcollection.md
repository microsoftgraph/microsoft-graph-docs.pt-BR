---
title: tipo de recurso changeNotificationCollection
description: Representa uma coleção de notificações de assinatura enviadas ao Assinante.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 242ab35d95cfc35c19e6d1f37cefa33ee8bd1632
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45004767"
---
# <a name="changenotificationcollection-resource-type"></a><span data-ttu-id="df79b-103">tipo de recurso changeNotificationCollection</span><span class="sxs-lookup"><span data-stu-id="df79b-103">changeNotificationCollection resource type</span></span>

<span data-ttu-id="df79b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df79b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df79b-105">Representa uma coleção de notificações de alteração de recursos enviadas ao Assinante.</span><span class="sxs-lookup"><span data-stu-id="df79b-105">Represents a collection of resource change notifications sent to the subscriber.</span></span>

<span data-ttu-id="df79b-106">Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="df79b-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="df79b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="df79b-107">Methods</span></span>

<span data-ttu-id="df79b-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="df79b-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="df79b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df79b-109">Properties</span></span>

| <span data-ttu-id="df79b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df79b-110">Property</span></span> | <span data-ttu-id="df79b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="df79b-111">Type</span></span> | <span data-ttu-id="df79b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="df79b-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="df79b-113">valor</span><span class="sxs-lookup"><span data-stu-id="df79b-113">value</span></span> | <span data-ttu-id="df79b-114">coleção ([changeNotification](changenotification.md))</span><span class="sxs-lookup"><span data-stu-id="df79b-114">collection([changeNotification](changenotification.md))</span></span> | <span data-ttu-id="df79b-115">O conjunto de notificações que estão sendo enviadas à URL de notificação.</span><span class="sxs-lookup"><span data-stu-id="df79b-115">The set of notifications being sent to the notification URL.</span></span> <span data-ttu-id="df79b-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df79b-116">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="df79b-117">Relações</span><span class="sxs-lookup"><span data-stu-id="df79b-117">Relationships</span></span>

<span data-ttu-id="df79b-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df79b-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df79b-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df79b-119">JSON representation</span></span>

<span data-ttu-id="df79b-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df79b-120">The following is a JSON representation of the resource.</span></span>

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
