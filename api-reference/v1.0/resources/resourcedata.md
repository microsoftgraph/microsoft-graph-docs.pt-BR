---
title: tipo de recurso resourceData
description: Representa os dados de recursos anexados à notificação de alteração enviada ao Assinante.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: c9da2041a6d982556ec909375ff46b3a9b3e2e2d
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598400"
---
# <a name="resourcedata-resource-type"></a><span data-ttu-id="fee24-103">tipo de recurso resourceData</span><span class="sxs-lookup"><span data-stu-id="fee24-103">resourceData resource type</span></span>

<span data-ttu-id="fee24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fee24-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fee24-105">Representa os dados de recursos anexados à notificação de alteração enviada ao Assinante.</span><span class="sxs-lookup"><span data-stu-id="fee24-105">Represents the resouce data attached to the change notification sent to the subscriber.</span></span>

<span data-ttu-id="fee24-106">Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="fee24-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fee24-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="fee24-107">Methods</span></span>

<span data-ttu-id="fee24-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fee24-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="fee24-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fee24-109">Properties</span></span>

<span data-ttu-id="fee24-110">Para recursos do Outlook, **resourceData** contém os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="fee24-110">For Outlook resources, **resourceData** contains the following fields:</span></span>

| <span data-ttu-id="fee24-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fee24-111">Property</span></span> | <span data-ttu-id="fee24-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="fee24-112">Type</span></span> | <span data-ttu-id="fee24-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="fee24-113">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="fee24-114">@odata.type</span><span class="sxs-lookup"><span data-stu-id="fee24-114">@odata.type</span></span> | <span data-ttu-id="fee24-115">string</span><span class="sxs-lookup"><span data-stu-id="fee24-115">string</span></span> | <span data-ttu-id="fee24-116">O tipo de entidade OData no Microsoft Graph que descreve o objeto representado.</span><span class="sxs-lookup"><span data-stu-id="fee24-116">The OData entity type in Microsoft Graph that describes the represented object.</span></span> |
| <span data-ttu-id="fee24-117">@odata.id</span><span class="sxs-lookup"><span data-stu-id="fee24-117">@odata.id</span></span> | <span data-ttu-id="fee24-118">string</span><span class="sxs-lookup"><span data-stu-id="fee24-118">string</span></span> | <span data-ttu-id="fee24-119">O identificador OData do objeto.</span><span class="sxs-lookup"><span data-stu-id="fee24-119">The OData identifier of the object.</span></span> |
| <span data-ttu-id="fee24-120">@odata.etag</span><span class="sxs-lookup"><span data-stu-id="fee24-120">@odata.etag</span></span> | <span data-ttu-id="fee24-121">string</span><span class="sxs-lookup"><span data-stu-id="fee24-121">string</span></span> | <span data-ttu-id="fee24-122">A marca da entidade HTTP que representa a versão do objeto.</span><span class="sxs-lookup"><span data-stu-id="fee24-122">The HTTP entity tag that represents the version of the object.</span></span> |
| <span data-ttu-id="fee24-123">id</span><span class="sxs-lookup"><span data-stu-id="fee24-123">id</span></span> | <span data-ttu-id="fee24-124">string</span><span class="sxs-lookup"><span data-stu-id="fee24-124">string</span></span> | <span data-ttu-id="fee24-125">O identificador do objeto.</span><span class="sxs-lookup"><span data-stu-id="fee24-125">The identifier of the object.</span></span> |

> <span data-ttu-id="fee24-126">**Observação:** O `id` valor fornecido em **resourceData** é válido no momento em que a notificação de alteração foi gerada.</span><span class="sxs-lookup"><span data-stu-id="fee24-126">**Note:** The `id` value provided in **resourceData** is valid at the time the change notification was generated.</span></span> <span data-ttu-id="fee24-127">Algumas ações, como mover uma mensagem para outra pasta podem resultar na `id` não mais ser válida quando a notificação de alteração for processada.</span><span class="sxs-lookup"><span data-stu-id="fee24-127">Some actions, such as moving a message to another folder, might result in the `id` no longer being valid when the change notification is processed.</span></span>

## <a name="relationships"></a><span data-ttu-id="fee24-128">Relações</span><span class="sxs-lookup"><span data-stu-id="fee24-128">Relationships</span></span>

<span data-ttu-id="fee24-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fee24-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fee24-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fee24-130">JSON representation</span></span>

<span data-ttu-id="fee24-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fee24-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceData"
}-->

```json
{
  "id": "1565293727947",
  "@odata.type": "#Microsoft.Graph.ChatMessage",
  "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
}
```

<!-- uuid: eb6c98ec-8257-4826-910e-5c603265257f
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource data resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
