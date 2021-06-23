---
title: Tipo de recurso changeNotification
description: Representa a notificação de alteração enviada ao assinante.
localization_priority: Normal
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 43933d31b8ac12f77331887c0421c3b6fc50b66b
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082374"
---
# <a name="changenotification-resource-type"></a><span data-ttu-id="5ea46-103">Tipo de recurso changeNotification</span><span class="sxs-lookup"><span data-stu-id="5ea46-103">changeNotification resource type</span></span>

<span data-ttu-id="5ea46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ea46-105">Representa a notificação enviada ao assinante.</span><span class="sxs-lookup"><span data-stu-id="5ea46-105">Represents the notification sent to the subscriber.</span></span>

<span data-ttu-id="5ea46-106">Para obter detalhes, confira [Usar a API do Microsoft Graph para receber notificações de alteração](webhooks.md).</span><span class="sxs-lookup"><span data-stu-id="5ea46-106">For details, see [Use the Microsoft Graph API to get change notifications](webhooks.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5ea46-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5ea46-107">Methods</span></span>

<span data-ttu-id="5ea46-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5ea46-108">None.</span></span>

## <a name="properties"></a><span data-ttu-id="5ea46-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ea46-109">Properties</span></span>

| <span data-ttu-id="5ea46-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ea46-110">Property</span></span> | <span data-ttu-id="5ea46-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ea46-111">Type</span></span> | <span data-ttu-id="5ea46-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ea46-112">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5ea46-113">changeType</span><span class="sxs-lookup"><span data-stu-id="5ea46-113">changeType</span></span> | <span data-ttu-id="5ea46-114">changeType</span><span class="sxs-lookup"><span data-stu-id="5ea46-114">changeType</span></span> | <span data-ttu-id="5ea46-115">Indica o tipo de alteração que levantará a notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="5ea46-115">Indicates the type of change that will raise the change notification.</span></span> <span data-ttu-id="5ea46-116">Os valores com suporte são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="5ea46-116">The supported values are: `created`, `updated`, `deleted`.</span></span> <span data-ttu-id="5ea46-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea46-117">Required.</span></span> |
| <span data-ttu-id="5ea46-118">clientState</span><span class="sxs-lookup"><span data-stu-id="5ea46-118">clientState</span></span> | <span data-ttu-id="5ea46-119">string</span><span class="sxs-lookup"><span data-stu-id="5ea46-119">string</span></span> | <span data-ttu-id="5ea46-120">Valor da **propriedade clientState** enviada especificada na solicitação de assinatura (se alguma).</span><span class="sxs-lookup"><span data-stu-id="5ea46-120">Value of the **clientState** property sent specified in the subscription request (if any).</span></span> <span data-ttu-id="5ea46-121">O tamanho máximo é de 255 caracteres.</span><span class="sxs-lookup"><span data-stu-id="5ea46-121">The maximum length is 255 characters.</span></span> <span data-ttu-id="5ea46-122">O cliente pode verificar se a notificação de alteração veio do serviço comparando os valores da **propriedade clientState.**</span><span class="sxs-lookup"><span data-stu-id="5ea46-122">The client can check whether the change notification came from the service by comparing the values of the **clientState** property.</span></span> <span data-ttu-id="5ea46-123">O valor da **propriedade clientState** enviado com a assinatura é comparado com o valor da **propriedade clientState** recebida com cada notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="5ea46-123">The value of the **clientState** property sent with the subscription is compared with the value of the **clientState** property received with each change notification.</span></span> <span data-ttu-id="5ea46-124">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5ea46-124">Optional.</span></span> |
| <span data-ttu-id="5ea46-125">encryptedContent</span><span class="sxs-lookup"><span data-stu-id="5ea46-125">encryptedContent</span></span> | [<span data-ttu-id="5ea46-126">changeNotificationEncryptedContent</span><span class="sxs-lookup"><span data-stu-id="5ea46-126">changeNotificationEncryptedContent</span></span>](changenotificationencryptedcontent.md) | <span data-ttu-id="5ea46-127">(Visualização) Conteúdo criptografado anexado com a notificação de alteração.</span><span class="sxs-lookup"><span data-stu-id="5ea46-127">(Preview) Encrypted content attached with the change notification.</span></span> <span data-ttu-id="5ea46-128">Somente fornecido se **encryptionCertificate** e **includeResourceData** foram definidos durante a solicitação de assinatura e se o recurso oferece suporte a ela.</span><span class="sxs-lookup"><span data-stu-id="5ea46-128">Only provided if **encryptionCertificate** and **includeResourceData** were defined during the subscription request and if the resource supports it.</span></span> <span data-ttu-id="5ea46-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5ea46-129">Optional.</span></span> |
| <span data-ttu-id="5ea46-130">id</span><span class="sxs-lookup"><span data-stu-id="5ea46-130">id</span></span> | <span data-ttu-id="5ea46-131">string</span><span class="sxs-lookup"><span data-stu-id="5ea46-131">string</span></span> | <span data-ttu-id="5ea46-132">ID exclusiva da notificação.</span><span class="sxs-lookup"><span data-stu-id="5ea46-132">Unique ID for the notification.</span></span> <span data-ttu-id="5ea46-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5ea46-133">Optional.</span></span> |
| <span data-ttu-id="5ea46-134">lifecycleEvent</span><span class="sxs-lookup"><span data-stu-id="5ea46-134">lifecycleEvent</span></span> | <span data-ttu-id="5ea46-135">lifecycleEventType</span><span class="sxs-lookup"><span data-stu-id="5ea46-135">lifecycleEventType</span></span> | <span data-ttu-id="5ea46-136">O tipo de notificação do ciclo de vida se a notificação atual for uma notificação do ciclo de vida.</span><span class="sxs-lookup"><span data-stu-id="5ea46-136">The type of lifecycle notification if the current notification is a lifecycle notification.</span></span> <span data-ttu-id="5ea46-137">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5ea46-137">Optional.</span></span> <span data-ttu-id="5ea46-138">Os valores suportados `missed` são `removed` , , `reauthorizationRequired` .</span><span class="sxs-lookup"><span data-stu-id="5ea46-138">Supported values are `missed`, `removed`, `reauthorizationRequired`.</span></span> |
| <span data-ttu-id="5ea46-139">recurso</span><span class="sxs-lookup"><span data-stu-id="5ea46-139">resource</span></span> | <span data-ttu-id="5ea46-140">string</span><span class="sxs-lookup"><span data-stu-id="5ea46-140">string</span></span> | <span data-ttu-id="5ea46-141">O URI do recurso que emitiu a notificação de alteração em relação a `https://graph.microsoft.com` .</span><span class="sxs-lookup"><span data-stu-id="5ea46-141">The URI of the resource that emitted the change notification relative to `https://graph.microsoft.com`.</span></span> <span data-ttu-id="5ea46-142">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea46-142">Required.</span></span> |
| <span data-ttu-id="5ea46-143">resourceData</span><span class="sxs-lookup"><span data-stu-id="5ea46-143">resourceData</span></span> | [<span data-ttu-id="5ea46-144">resourceData</span><span class="sxs-lookup"><span data-stu-id="5ea46-144">resourceData</span></span>](resourcedata.md) | <span data-ttu-id="5ea46-145">O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado.</span><span class="sxs-lookup"><span data-stu-id="5ea46-145">The content of this property depends on the type of resource being subscribed to.</span></span> <span data-ttu-id="5ea46-146">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea46-146">Required.</span></span> |
| <span data-ttu-id="5ea46-147">subscriptionExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5ea46-147">subscriptionExpirationDateTime</span></span> | <span data-ttu-id="5ea46-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ea46-148">DateTimeOffset</span></span> | <span data-ttu-id="5ea46-149">O tempo de expiração da assinatura.</span><span class="sxs-lookup"><span data-stu-id="5ea46-149">The expiration time for the subscription.</span></span> <span data-ttu-id="5ea46-150">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ea46-150">Required.</span></span> |
| <span data-ttu-id="5ea46-151">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="5ea46-151">subscriptionId</span></span> | <span data-ttu-id="5ea46-152">GUID</span><span class="sxs-lookup"><span data-stu-id="5ea46-152">GUID</span></span> | <span data-ttu-id="5ea46-153">O identificador exclusivo da assinatura que gerou a notificação.</span><span class="sxs-lookup"><span data-stu-id="5ea46-153">The unique identifier of the subscription that generated the notification.</span></span> |
| <span data-ttu-id="5ea46-154">tenantId</span><span class="sxs-lookup"><span data-stu-id="5ea46-154">tenantId</span></span> | <span data-ttu-id="5ea46-155">GUID</span><span class="sxs-lookup"><span data-stu-id="5ea46-155">GUID</span></span> | <span data-ttu-id="5ea46-156">O identificador exclusivo do locatário do qual a notificação de alteração se originou.</span><span class="sxs-lookup"><span data-stu-id="5ea46-156">The unique identifier of the tenant from which the change notification originated.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5ea46-157">Relações</span><span class="sxs-lookup"><span data-stu-id="5ea46-157">Relationships</span></span>

<span data-ttu-id="5ea46-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ea46-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ea46-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ea46-159">JSON representation</span></span>

<span data-ttu-id="5ea46-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ea46-160">The following is a JSON representation of the resource.</span></span>

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


