---
title: tipo de recurso changeNotification
description: Representa a notificação de alteração enviada ao Assinante.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 1bb5f8d5177e294a969fb48d335bd4a3061f1bb1
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681757"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="ea561-103">tipo de recurso changeNotification</span><span class="sxs-lookup"><span data-stu-id="ea561-103">changeNotification resource type</span></span>

<span data-ttu-id="ea561-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea561-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea561-105">Representa a notificação enviada ao Assinante.</span><span class="sxs-lookup"><span data-stu-id="ea561-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="ea561-106">Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="ea561-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ea561-107">Methods</span><span class="sxs-lookup"><span data-stu-id="ea561-107">Methods</span></span>

<span data-ttu-id="ea561-108">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea561-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="ea561-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea561-109">Properties</span></span>

| <span data-ttu-id="ea561-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea561-110">Property</span></span> | <span data-ttu-id="ea561-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea561-111">Type</span></span> | <span data-ttu-id="ea561-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea561-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="ea561-113">changeType</span><span class="sxs-lookup"><span data-stu-id="ea561-113">changeType</span></span> | <span data-ttu-id="ea561-114">string</span><span class="sxs-lookup"><span data-stu-id="ea561-114">string</span></span> | <span data-ttu-id="ea561-115">Indica o tipo de alteração que gerará a notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="ea561-115">Indicates the type of change that will raised the change notification.</span></span> <span data-ttu-id="ea561-116">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="ea561-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="ea561-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea561-117">Required.</span></span> |
| <span data-ttu-id="ea561-118">clientState</span><span class="sxs-lookup"><span data-stu-id="ea561-118">clientState</span></span> | <span data-ttu-id="ea561-119">string</span><span class="sxs-lookup"><span data-stu-id="ea561-119">string</span></span> | <span data-ttu-id="ea561-120">O valor da propriedade **ClientState** enviado especificado na solicitação de assinatura (se houver).</span><span class="sxs-lookup"><span data-stu-id="ea561-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="ea561-121">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="ea561-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="ea561-122">O cliente pode verificar se a notificação de alteração veio do serviço, comparando o valor da propriedade **ClientState** enviada com a assinatura com o valor da propriedade **ClientState** recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="ea561-122">The client can check that the change notification came from the service by comparing the value of the **clientState** property sent with the subscription with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="ea561-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea561-123">Optional.</span></span> |
| <span data-ttu-id="ea561-124">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="ea561-124">encryptedContent</span></span> | [<span data-ttu-id="ea561-125">Microsoft. Graph. changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="ea561-125">microsoft.graph.changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="ea561-126">Prever Conteúdo criptografado anexado à notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="ea561-126">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="ea561-127">Só é fornecido se **encryptionCertificate** e **includeResourceData** foram definidos durante a solicitação de assinatura e se o recurso oferecer suporte a ele.</span><span class="sxs-lookup"><span data-stu-id="ea561-127">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="ea561-128">Opcional</span><span class="sxs-lookup"><span data-stu-id="ea561-128">Optional</span></span> |
| <span data-ttu-id="ea561-129">lifecycleEvent</span><span class="sxs-lookup"><span data-stu-id="ea561-129">lifecycleEvent</span></span> | <span data-ttu-id="ea561-130">string</span><span class="sxs-lookup"><span data-stu-id="ea561-130">string</span></span> | <span data-ttu-id="ea561-131">O tipo de notificação de ciclo de vida se a notificação atual é uma notificação de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="ea561-131">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="ea561-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea561-132">Optional.</span></span> <span data-ttu-id="ea561-133">Os valores com suporte são `missed` , `removed` , `reauthorizationRequired` .</span><span class="sxs-lookup"><span data-stu-id="ea561-133">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="ea561-134">id</span><span class="sxs-lookup"><span data-stu-id="ea561-134">id</span></span> | <span data-ttu-id="ea561-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea561-135">string</span></span> | <span data-ttu-id="ea561-136">ID exclusiva da notificação.</span><span class="sxs-lookup"><span data-stu-id="ea561-136">Unique ID for the notification.</span></span> <span data-ttu-id="ea561-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea561-137">Optional.</span></span> |
| <span data-ttu-id="ea561-138">recurso</span><span class="sxs-lookup"><span data-stu-id="ea561-138">resource</span></span> | <span data-ttu-id="ea561-139">string</span><span class="sxs-lookup"><span data-stu-id="ea561-139">string</span></span> | <span data-ttu-id="ea561-140">O URI do recurso que emitiu a notificação de alteração relativa a `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="ea561-140">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="ea561-141">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea561-141">Required.</span></span> |
| <span data-ttu-id="ea561-142">resourceData</span><span class="sxs-lookup"><span data-stu-id="ea561-142">resourceData</span></span> | [<span data-ttu-id="ea561-143">Microsoft. Graph. resourceData</span><span class="sxs-lookup"><span data-stu-id="ea561-143">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="ea561-144">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="ea561-144">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="ea561-145">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea561-145">Required.</span></span> |
| <span data-ttu-id="ea561-146">sequenceNumber</span><span class="sxs-lookup"><span data-stu-id="ea561-146">sequenceNumber</span></span> | <span data-ttu-id="ea561-147">int</span><span class="sxs-lookup"><span data-stu-id="ea561-147">int</span></span> | <span data-ttu-id="ea561-148">Um número em sequência para uma notificação, para ajudar o aplicativo cliente a identificar se as notificações estão em sequência ou se uma notificação estiver ausente.</span><span class="sxs-lookup"><span data-stu-id="ea561-148">A number in sequence for a notification, to help the client app identify if notifications are in sequence or if a notification is missing.</span></span> <span data-ttu-id="ea561-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ea561-149">Optional.</span></span> |
| <span data-ttu-id="ea561-150">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ea561-150">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="ea561-151">dateTime</span><span class="sxs-lookup"><span data-stu-id="ea561-151">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="ea561-152">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="ea561-152">The expiration time for the subscription.</span></span> <span data-ttu-id="ea561-153">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea561-153">Required.</span></span> |
| <span data-ttu-id="ea561-154">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="ea561-154">subscriptionId</span></span> | <span data-ttu-id="ea561-155">string</span><span class="sxs-lookup"><span data-stu-id="ea561-155">string</span></span> | <span data-ttu-id="ea561-156">O identificador exclusivo da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="ea561-156">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="ea561-157">tenantId</span><span class="sxs-lookup"><span data-stu-id="ea561-157">tenantId</span></span> | <span data-ttu-id="ea561-158">#c0</span><span class="sxs-lookup"><span data-stu-id="ea561-158">guid</span></span> | <span data-ttu-id="ea561-159">O exclusivo identificado do locatário do qual a notificação de alteração se originou.</span><span class="sxs-lookup"><span data-stu-id="ea561-159">The unique identified of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ea561-160">Relações</span><span class="sxs-lookup"><span data-stu-id="ea561-160">Relationships</span></span>

<span data-ttu-id="ea561-161">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea561-161">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea561-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea561-162">JSON representation</span></span>

<span data-ttu-id="ea561-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea561-163">The following is a JSON representation of the resource.</span></span>

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
