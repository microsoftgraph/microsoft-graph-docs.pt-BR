---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 63e4b858404242d84597a7f650bae6c0870f5b76
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162502"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="3b20a-103">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3b20a-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="3b20a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b20a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b20a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b20a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b20a-106">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="3b20a-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="3b20a-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3b20a-107">Methods</span></span>
|<span data-ttu-id="3b20a-108">Método</span><span class="sxs-lookup"><span data-stu-id="3b20a-108">Method</span></span>|<span data-ttu-id="3b20a-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3b20a-109">Return Type</span></span>|<span data-ttu-id="3b20a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b20a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b20a-111">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3b20a-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="3b20a-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3b20a-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="3b20a-113">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="3b20a-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="3b20a-114">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3b20a-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="3b20a-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="3b20a-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="3b20a-116">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="3b20a-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="3b20a-117">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="3b20a-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="3b20a-118">String</span><span class="sxs-lookup"><span data-stu-id="3b20a-118">String</span></span>|<span data-ttu-id="3b20a-119">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="3b20a-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="3b20a-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b20a-120">Properties</span></span>
|<span data-ttu-id="3b20a-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b20a-121">Property</span></span>|<span data-ttu-id="3b20a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b20a-122">Type</span></span>|<span data-ttu-id="3b20a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b20a-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b20a-124">id</span><span class="sxs-lookup"><span data-stu-id="3b20a-124">id</span></span>|<span data-ttu-id="3b20a-125">String</span><span class="sxs-lookup"><span data-stu-id="3b20a-125">String</span></span>|<span data-ttu-id="3b20a-126">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="3b20a-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="3b20a-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="3b20a-127">appleIdentifier</span></span>|<span data-ttu-id="3b20a-128">String</span><span class="sxs-lookup"><span data-stu-id="3b20a-128">String</span></span>|<span data-ttu-id="3b20a-129">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="3b20a-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="3b20a-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="3b20a-130">topicIdentifier</span></span>|<span data-ttu-id="3b20a-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b20a-131">String</span></span>|<span data-ttu-id="3b20a-132">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="3b20a-132">Topic Id.</span></span>|
|<span data-ttu-id="3b20a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b20a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="3b20a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b20a-134">DateTimeOffset</span></span>|<span data-ttu-id="3b20a-135">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="3b20a-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="3b20a-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3b20a-136">expirationDateTime</span></span>|<span data-ttu-id="3b20a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b20a-137">DateTimeOffset</span></span>|<span data-ttu-id="3b20a-138">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="3b20a-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="3b20a-139">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="3b20a-139">certificateUploadStatus</span></span>|<span data-ttu-id="3b20a-140">String</span><span class="sxs-lookup"><span data-stu-id="3b20a-140">String</span></span>|<span data-ttu-id="3b20a-141">O status do carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="3b20a-141">The certificate upload status.</span></span>|
|<span data-ttu-id="3b20a-142">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="3b20a-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="3b20a-143">String</span><span class="sxs-lookup"><span data-stu-id="3b20a-143">String</span></span>|<span data-ttu-id="3b20a-144">O motivo da falha no carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="3b20a-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="3b20a-145">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="3b20a-145">certificateSerialNumber</span></span>|<span data-ttu-id="3b20a-146">String</span><span class="sxs-lookup"><span data-stu-id="3b20a-146">String</span></span>|<span data-ttu-id="3b20a-147">Número de série do certificado.</span><span class="sxs-lookup"><span data-stu-id="3b20a-147">Certificate serial number.</span></span> <span data-ttu-id="3b20a-148">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b20a-148">This property is read-only.</span></span>|
|<span data-ttu-id="3b20a-149">certificado</span><span class="sxs-lookup"><span data-stu-id="3b20a-149">certificate</span></span>|<span data-ttu-id="3b20a-150">String</span><span class="sxs-lookup"><span data-stu-id="3b20a-150">String</span></span>|<span data-ttu-id="3b20a-151">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b20a-151">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b20a-152">Relações</span><span class="sxs-lookup"><span data-stu-id="3b20a-152">Relationships</span></span>
<span data-ttu-id="3b20a-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b20a-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b20a-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b20a-154">JSON Representation</span></span>
<span data-ttu-id="3b20a-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b20a-155">Here is a JSON representation of the resource.</span></span>
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
  "certificateUploadStatus": "String",
  "certificateUploadFailureReason": "String",
  "certificateSerialNumber": "String",
  "certificate": "String"
}
```



