---
title: Tipo de recurso changeNotification
description: Representa a notificação de alteração enviada ao Assinante.
localization_priority: Normal
author: davidmu1
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 6a39d156849236a40268064cb234e6015c9424f3
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598539"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="e80c9-103">Tipo de recurso changeNotification</span><span class="sxs-lookup"><span data-stu-id="e80c9-103">changeNotification resource type</span></span>

<span data-ttu-id="e80c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e80c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e80c9-105">Representa a notificação enviada ao Assinante.</span><span class="sxs-lookup"><span data-stu-id="e80c9-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="e80c9-106">Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="e80c9-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e80c9-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e80c9-107">Methods</span></span>

<span data-ttu-id="e80c9-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e80c9-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="e80c9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e80c9-109">Properties</span></span>

| <span data-ttu-id="e80c9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e80c9-110">Property</span></span> | <span data-ttu-id="e80c9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e80c9-111">Type</span></span> | <span data-ttu-id="e80c9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e80c9-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e80c9-113">changeType</span><span class="sxs-lookup"><span data-stu-id="e80c9-113">changeType</span></span> | <span data-ttu-id="e80c9-114">string</span><span class="sxs-lookup"><span data-stu-id="e80c9-114">string</span></span> | <span data-ttu-id="e80c9-115">Indica o tipo de alteração que irá gerar a notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e80c9-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="e80c9-116">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="e80c9-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="e80c9-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e80c9-117">Required.</span></span> |
| <span data-ttu-id="e80c9-118">clientState</span><span class="sxs-lookup"><span data-stu-id="e80c9-118">clientState</span></span> | <span data-ttu-id="e80c9-119">string</span><span class="sxs-lookup"><span data-stu-id="e80c9-119">string</span></span> | <span data-ttu-id="e80c9-120">O valor da propriedade **ClientState** enviado especificado na solicitação de assinatura (se houver).</span><span class="sxs-lookup"><span data-stu-id="e80c9-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="e80c9-121">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="e80c9-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="e80c9-122">O cliente pode verificar se a notificação de alteração veio do serviço, comparando os valores da propriedade **ClientState** .</span><span class="sxs-lookup"><span data-stu-id="e80c9-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="e80c9-123">O valor da propriedade **ClientState** enviada com a assinatura é comparado com o valor da propriedade **ClientState** recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e80c9-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="e80c9-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e80c9-124">Optional.</span></span> |
| <span data-ttu-id="e80c9-125">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="e80c9-125">encryptedContent</span></span> | [<span data-ttu-id="e80c9-126">Microsoft. Graph. changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="e80c9-126">microsoft.graph.changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="e80c9-127">Prever Conteúdo criptografado anexado à notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="e80c9-127">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="e80c9-128">Só é fornecido se **encryptionCertificate** e **includeResourceData** foram definidos durante a solicitação de assinatura e se o recurso oferecer suporte a ele.</span><span class="sxs-lookup"><span data-stu-id="e80c9-128">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="e80c9-129">Opcional</span><span class="sxs-lookup"><span data-stu-id="e80c9-129">Optional</span></span> |
| <span data-ttu-id="e80c9-130">lifecycleEvent</span><span class="sxs-lookup"><span data-stu-id="e80c9-130">lifecycleEvent</span></span> | <span data-ttu-id="e80c9-131">string</span><span class="sxs-lookup"><span data-stu-id="e80c9-131">string</span></span> | <span data-ttu-id="e80c9-132">O tipo de notificação de ciclo de vida se a notificação atual é uma notificação de ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="e80c9-132">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="e80c9-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e80c9-133">Optional.</span></span> <span data-ttu-id="e80c9-134">Os valores com suporte são `missed` , `removed` , `reauthorizationRequired` .</span><span class="sxs-lookup"><span data-stu-id="e80c9-134">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="e80c9-135">id</span><span class="sxs-lookup"><span data-stu-id="e80c9-135">id</span></span> | <span data-ttu-id="e80c9-136">string</span><span class="sxs-lookup"><span data-stu-id="e80c9-136">string</span></span> | <span data-ttu-id="e80c9-137">ID exclusiva da notificação.</span><span class="sxs-lookup"><span data-stu-id="e80c9-137">Unique ID for the notification.</span></span> <span data-ttu-id="e80c9-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="e80c9-138">Optional.</span></span> |
| <span data-ttu-id="e80c9-139">recurso</span><span class="sxs-lookup"><span data-stu-id="e80c9-139">resource</span></span> | <span data-ttu-id="e80c9-140">string</span><span class="sxs-lookup"><span data-stu-id="e80c9-140">string</span></span> | <span data-ttu-id="e80c9-141">O URI do recurso que emitiu a notificação de alteração relativa a `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="e80c9-141">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="e80c9-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e80c9-142">Required.</span></span> |
| <span data-ttu-id="e80c9-143">resourceData</span><span class="sxs-lookup"><span data-stu-id="e80c9-143">resourceData</span></span> | [<span data-ttu-id="e80c9-144">Microsoft. Graph. resourceData</span><span class="sxs-lookup"><span data-stu-id="e80c9-144">microsoft.graph.resourceData</span></span>](resourcedata.md) | <span data-ttu-id="e80c9-145">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="e80c9-145">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="e80c9-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e80c9-146">Required.</span></span> |
| <span data-ttu-id="e80c9-147">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e80c9-147">subscriptionExpirationDateTime</span></span> | [<span data-ttu-id="e80c9-148">dateTime</span><span class="sxs-lookup"><span data-stu-id="e80c9-148">dateTime</span></span>](https://tools.ietf.org/html/rfc3339) | <span data-ttu-id="e80c9-149">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e80c9-149">The expiration time for the subscription.</span></span> <span data-ttu-id="e80c9-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e80c9-150">Required.</span></span> |
| <span data-ttu-id="e80c9-151">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="e80c9-151">subscriptionId</span></span> | <span data-ttu-id="e80c9-152">string</span><span class="sxs-lookup"><span data-stu-id="e80c9-152">string</span></span> | <span data-ttu-id="e80c9-153">O identificador exclusivo da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="e80c9-153">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="e80c9-154">tenantId</span><span class="sxs-lookup"><span data-stu-id="e80c9-154">tenantId</span></span> | <span data-ttu-id="e80c9-155">#c0</span><span class="sxs-lookup"><span data-stu-id="e80c9-155">guid</span></span> | <span data-ttu-id="e80c9-156">O identificador exclusivo do locatário do qual a notificação de alteração se originou.</span><span class="sxs-lookup"><span data-stu-id="e80c9-156">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e80c9-157">Relações</span><span class="sxs-lookup"><span data-stu-id="e80c9-157">Relationships</span></span>

<span data-ttu-id="e80c9-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e80c9-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e80c9-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e80c9-159">JSON representation</span></span>

<span data-ttu-id="e80c9-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e80c9-160">The following is a JSON representation of the resource.</span></span>

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
