---
title: tipo de recurso changeNotification
description: Representa a notificação de alteração enviada ao Assinante.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: d45c3973e5b044daf3121a740a60b29e3a181348
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45004763"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="4463e-103">tipo de recurso changeNotification</span><span class="sxs-lookup"><span data-stu-id="4463e-103">changeNotification resource type</span></span>

<span data-ttu-id="4463e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4463e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4463e-105">Representa a notificação enviada ao Assinante.</span><span class="sxs-lookup"><span data-stu-id="4463e-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="4463e-106">Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="4463e-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4463e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4463e-107">Methods</span></span>

<span data-ttu-id="4463e-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4463e-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="4463e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4463e-109">Properties</span></span>

| <span data-ttu-id="4463e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4463e-110">Property</span></span> | <span data-ttu-id="4463e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4463e-111">Type</span></span> | <span data-ttu-id="4463e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4463e-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="4463e-113">changeType</span><span class="sxs-lookup"><span data-stu-id="4463e-113">changeType</span></span> | <span data-ttu-id="4463e-114">string</span><span class="sxs-lookup"><span data-stu-id="4463e-114">string</span></span> | <span data-ttu-id="4463e-115">Indica o tipo de alteração que irá gerar a notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="4463e-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="4463e-116">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="4463e-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="4463e-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4463e-117">Required.</span></span> |
| <span data-ttu-id="4463e-118">clientState</span><span class="sxs-lookup"><span data-stu-id="4463e-118">clientState</span></span> | <span data-ttu-id="4463e-119">string</span><span class="sxs-lookup"><span data-stu-id="4463e-119">string</span></span> | <span data-ttu-id="4463e-120">O valor da propriedade **ClientState** enviada na solicitação de assinatura (se houver).</span><span class="sxs-lookup"><span data-stu-id="4463e-120">Value of the **clientState** property sent in the subscription request (if any).</span></span> <span data-ttu-id="4463e-121">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="4463e-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="4463e-122">O cliente pode verificar se a notificação de alteração veio do serviço, comparando os valores da propriedade **ClientState** .</span><span class="sxs-lookup"><span data-stu-id="4463e-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="4463e-123">O valor da propriedade **ClientState** enviada com a assinatura é comparado com o valor da propriedade **ClientState** recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="4463e-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="4463e-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4463e-124">Optional.</span></span> |
| <span data-ttu-id="4463e-125">id</span><span class="sxs-lookup"><span data-stu-id="4463e-125">id</span></span> | <span data-ttu-id="4463e-126">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4463e-126">string</span></span> | <span data-ttu-id="4463e-127">ID exclusiva da notificação.</span><span class="sxs-lookup"><span data-stu-id="4463e-127">Unique ID for the notification.</span></span> <span data-ttu-id="4463e-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4463e-128">Optional.</span></span> |
| <span data-ttu-id="4463e-129">recurso</span><span class="sxs-lookup"><span data-stu-id="4463e-129">resource</span></span> | <span data-ttu-id="4463e-130">string</span><span class="sxs-lookup"><span data-stu-id="4463e-130">string</span></span> | <span data-ttu-id="4463e-131">O URI do recurso que emitiu a notificação de alteração relativa a `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="4463e-131">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="4463e-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4463e-132">Required.</span></span> |
| <span data-ttu-id="4463e-133">resourceData</span><span class="sxs-lookup"><span data-stu-id="4463e-133">resourceData</span></span> | [<span data-ttu-id="4463e-134">Microsoft. Graph. resourceData</span><span class="sxs-lookup"><span data-stu-id="4463e-134">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="4463e-135">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="4463e-135">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="4463e-136">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4463e-136">Required.</span></span> |
| <span data-ttu-id="4463e-137">sequenceNumber</span><span class="sxs-lookup"><span data-stu-id="4463e-137">sequenceNumber</span></span> | <span data-ttu-id="4463e-138">int</span><span class="sxs-lookup"><span data-stu-id="4463e-138">int</span></span> | <span data-ttu-id="4463e-139">Um número em sequência para uma notificação, para ajudar o aplicativo cliente a identificar se as notificações estão em sequência ou se uma notificação estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="4463e-139">A number in sequence for a notification, to help the client app identify if notifications are in sequence or if a notification is missing.</span></span> <span data-ttu-id="4463e-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4463e-140">Optional.</span></span> |
| <span data-ttu-id="4463e-141">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4463e-141">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="4463e-142">dateTime</span><span class="sxs-lookup"><span data-stu-id="4463e-142">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="4463e-143">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="4463e-143">The expiration time for the subscription.</span></span> <span data-ttu-id="4463e-144">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4463e-144">Required.</span></span> |
| <span data-ttu-id="4463e-145">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="4463e-145">subscriptionId</span></span> | <span data-ttu-id="4463e-146">string</span><span class="sxs-lookup"><span data-stu-id="4463e-146">string</span></span> | <span data-ttu-id="4463e-147">O identificador exclusivo da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="4463e-147">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="4463e-148">tenantId</span><span class="sxs-lookup"><span data-stu-id="4463e-148">tenantId</span></span> | <span data-ttu-id="4463e-149">#c0</span><span class="sxs-lookup"><span data-stu-id="4463e-149">guid</span></span> | <span data-ttu-id="4463e-150">O identificador exclusivo do locatário do qual a notificação de alteração se originou.</span><span class="sxs-lookup"><span data-stu-id="4463e-150">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4463e-151">Relações</span><span class="sxs-lookup"><span data-stu-id="4463e-151">Relationships</span></span>

<span data-ttu-id="4463e-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4463e-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4463e-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4463e-153">JSON representation</span></span>

<span data-ttu-id="4463e-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4463e-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotification"
}-->

```json
{
  "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
  "changeType": "created",
  "clientState": "client state provided when creating subscription",
  "id": "15ee1d1f-af7b-42d9-885b-9d00db065dd9",
  "sequenceNumber": 20,
  "tenantId": "2c937fad-a8a7-496c-b0e4-bf77dcc7eb2a",
  "subscriptionExpirationDateTime": "2020-04-12T23:20:50.52Z",
  "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
  "resourceData": {
    "id": "1565293727947",
    "@odata.type": "#Microsoft.Graph.ChatMessage",
    "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
  }
}
```

<!-- uuid: 15ee1d1f-af7b-42d9-885b-9d00db065dd9
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
