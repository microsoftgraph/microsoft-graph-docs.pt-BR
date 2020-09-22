---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2bbcca2707223f53b59d1b3d5d2ceb75ba08c57a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091317"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="0a0ee-103">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0a0ee-103">applePushNotificationCertificate resource type</span></span>

<span data-ttu-id="0a0ee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a0ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a0ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0a0ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a0ee-106">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="0a0ee-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="0a0ee-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0a0ee-107">Methods</span></span>
|<span data-ttu-id="0a0ee-108">Método</span><span class="sxs-lookup"><span data-stu-id="0a0ee-108">Method</span></span>|<span data-ttu-id="0a0ee-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0a0ee-109">Return Type</span></span>|<span data-ttu-id="0a0ee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a0ee-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0a0ee-111">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0a0ee-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="0a0ee-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0a0ee-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="0a0ee-113">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0a0ee-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="0a0ee-114">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0a0ee-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="0a0ee-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="0a0ee-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="0a0ee-116">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="0a0ee-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="0a0ee-117">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="0a0ee-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="0a0ee-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a0ee-118">String</span></span>|<span data-ttu-id="0a0ee-119">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="0a0ee-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="0a0ee-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a0ee-120">Properties</span></span>
|<span data-ttu-id="0a0ee-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a0ee-121">Property</span></span>|<span data-ttu-id="0a0ee-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a0ee-122">Type</span></span>|<span data-ttu-id="0a0ee-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a0ee-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a0ee-124">id</span><span class="sxs-lookup"><span data-stu-id="0a0ee-124">id</span></span>|<span data-ttu-id="0a0ee-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a0ee-125">String</span></span>|<span data-ttu-id="0a0ee-126">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="0a0ee-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="0a0ee-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="0a0ee-127">appleIdentifier</span></span>|<span data-ttu-id="0a0ee-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a0ee-128">String</span></span>|<span data-ttu-id="0a0ee-129">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="0a0ee-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="0a0ee-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="0a0ee-130">topicIdentifier</span></span>|<span data-ttu-id="0a0ee-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a0ee-131">String</span></span>|<span data-ttu-id="0a0ee-132">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="0a0ee-132">Topic Id.</span></span>|
|<span data-ttu-id="0a0ee-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a0ee-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0a0ee-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a0ee-134">DateTimeOffset</span></span>|<span data-ttu-id="0a0ee-135">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="0a0ee-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="0a0ee-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0a0ee-136">expirationDateTime</span></span>|<span data-ttu-id="0a0ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a0ee-137">DateTimeOffset</span></span>|<span data-ttu-id="0a0ee-138">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="0a0ee-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="0a0ee-139">certificado</span><span class="sxs-lookup"><span data-stu-id="0a0ee-139">certificate</span></span>|<span data-ttu-id="0a0ee-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a0ee-140">String</span></span>|<span data-ttu-id="0a0ee-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0a0ee-141">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a0ee-142">Relações</span><span class="sxs-lookup"><span data-stu-id="0a0ee-142">Relationships</span></span>
<span data-ttu-id="0a0ee-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a0ee-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a0ee-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a0ee-144">JSON Representation</span></span>
<span data-ttu-id="0a0ee-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a0ee-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```









