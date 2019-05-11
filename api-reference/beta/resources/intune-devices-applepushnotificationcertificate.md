---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9adcc496943118f268b8977a4134c4e434130bad
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943204"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="509fa-103">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="509fa-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="509fa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="509fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="509fa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="509fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="509fa-106">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="509fa-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="509fa-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="509fa-107">Methods</span></span>
|<span data-ttu-id="509fa-108">Método</span><span class="sxs-lookup"><span data-stu-id="509fa-108">Method</span></span>|<span data-ttu-id="509fa-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="509fa-109">Return Type</span></span>|<span data-ttu-id="509fa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="509fa-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="509fa-111">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="509fa-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="509fa-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="509fa-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="509fa-113">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="509fa-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="509fa-114">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="509fa-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="509fa-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="509fa-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="509fa-116">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="509fa-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="509fa-117">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="509fa-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="509fa-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509fa-118">String</span></span>|<span data-ttu-id="509fa-119">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="509fa-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="509fa-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="509fa-120">Properties</span></span>
|<span data-ttu-id="509fa-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="509fa-121">Property</span></span>|<span data-ttu-id="509fa-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="509fa-122">Type</span></span>|<span data-ttu-id="509fa-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="509fa-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="509fa-124">id</span><span class="sxs-lookup"><span data-stu-id="509fa-124">id</span></span>|<span data-ttu-id="509fa-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509fa-125">String</span></span>|<span data-ttu-id="509fa-126">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="509fa-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="509fa-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="509fa-127">appleIdentifier</span></span>|<span data-ttu-id="509fa-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509fa-128">String</span></span>|<span data-ttu-id="509fa-129">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="509fa-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="509fa-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="509fa-130">topicIdentifier</span></span>|<span data-ttu-id="509fa-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509fa-131">String</span></span>|<span data-ttu-id="509fa-132">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="509fa-132">Topic Id.</span></span>|
|<span data-ttu-id="509fa-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="509fa-133">lastModifiedDateTime</span></span>|<span data-ttu-id="509fa-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="509fa-134">DateTimeOffset</span></span>|<span data-ttu-id="509fa-135">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="509fa-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="509fa-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="509fa-136">expirationDateTime</span></span>|<span data-ttu-id="509fa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="509fa-137">DateTimeOffset</span></span>|<span data-ttu-id="509fa-138">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="509fa-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="509fa-139">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="509fa-139">certificateUploadStatus</span></span>|<span data-ttu-id="509fa-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509fa-140">String</span></span>|<span data-ttu-id="509fa-141">O status do carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="509fa-141">The certificate upload status.</span></span>|
|<span data-ttu-id="509fa-142">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="509fa-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="509fa-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="509fa-143">String</span></span>|<span data-ttu-id="509fa-144">O motivo da falha no carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="509fa-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="509fa-145">certificado</span><span class="sxs-lookup"><span data-stu-id="509fa-145">certificate</span></span>|<span data-ttu-id="509fa-146">String</span><span class="sxs-lookup"><span data-stu-id="509fa-146">String</span></span>|<span data-ttu-id="509fa-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="509fa-147">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="509fa-148">Relações</span><span class="sxs-lookup"><span data-stu-id="509fa-148">Relationships</span></span>
<span data-ttu-id="509fa-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="509fa-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="509fa-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="509fa-150">JSON Representation</span></span>
<span data-ttu-id="509fa-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="509fa-151">Here is a JSON representation of the resource.</span></span>
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
  "certificate": "String"
}
```




