---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0d53407d5ec380e7bfe11d50f6871eb6bbfb87aa
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760206"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="7164e-103">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7164e-103">applePushNotificationCertificate resource type</span></span>

<span data-ttu-id="7164e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7164e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7164e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7164e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7164e-106">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="7164e-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="7164e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="7164e-107">Methods</span></span>
|<span data-ttu-id="7164e-108">Método</span><span class="sxs-lookup"><span data-stu-id="7164e-108">Method</span></span>|<span data-ttu-id="7164e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7164e-109">Return Type</span></span>|<span data-ttu-id="7164e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7164e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7164e-111">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7164e-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="7164e-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7164e-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="7164e-113">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7164e-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="7164e-114">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7164e-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="7164e-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="7164e-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="7164e-116">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="7164e-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="7164e-117">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="7164e-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="7164e-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7164e-118">String</span></span>|<span data-ttu-id="7164e-119">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="7164e-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="7164e-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7164e-120">Properties</span></span>
|<span data-ttu-id="7164e-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7164e-121">Property</span></span>|<span data-ttu-id="7164e-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="7164e-122">Type</span></span>|<span data-ttu-id="7164e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7164e-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7164e-124">id</span><span class="sxs-lookup"><span data-stu-id="7164e-124">id</span></span>|<span data-ttu-id="7164e-125">String</span><span class="sxs-lookup"><span data-stu-id="7164e-125">String</span></span>|<span data-ttu-id="7164e-126">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="7164e-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="7164e-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="7164e-127">appleIdentifier</span></span>|<span data-ttu-id="7164e-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7164e-128">String</span></span>|<span data-ttu-id="7164e-129">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="7164e-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="7164e-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="7164e-130">topicIdentifier</span></span>|<span data-ttu-id="7164e-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7164e-131">String</span></span>|<span data-ttu-id="7164e-132">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="7164e-132">Topic Id.</span></span>|
|<span data-ttu-id="7164e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7164e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="7164e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7164e-134">DateTimeOffset</span></span>|<span data-ttu-id="7164e-135">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="7164e-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="7164e-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7164e-136">expirationDateTime</span></span>|<span data-ttu-id="7164e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7164e-137">DateTimeOffset</span></span>|<span data-ttu-id="7164e-138">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="7164e-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="7164e-139">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="7164e-139">certificateSerialNumber</span></span>|<span data-ttu-id="7164e-140">String</span><span class="sxs-lookup"><span data-stu-id="7164e-140">String</span></span>|<span data-ttu-id="7164e-141">Número de série do certificado.</span><span class="sxs-lookup"><span data-stu-id="7164e-141">Certificate serial number.</span></span> <span data-ttu-id="7164e-142">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7164e-142">This property is read-only.</span></span>|
|<span data-ttu-id="7164e-143">certificado</span><span class="sxs-lookup"><span data-stu-id="7164e-143">certificate</span></span>|<span data-ttu-id="7164e-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7164e-144">String</span></span>|<span data-ttu-id="7164e-145">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7164e-145">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="7164e-146">Relações</span><span class="sxs-lookup"><span data-stu-id="7164e-146">Relationships</span></span>
<span data-ttu-id="7164e-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7164e-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7164e-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7164e-148">JSON Representation</span></span>
<span data-ttu-id="7164e-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7164e-149">Here is a JSON representation of the resource.</span></span>
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
  "certificateSerialNumber": "String",
  "certificate": "String"
}
```




