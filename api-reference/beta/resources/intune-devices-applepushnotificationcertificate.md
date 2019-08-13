---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 90e7ede759d9df4197aa193495d8aea26996766e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319276"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="ed698-103">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ed698-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="ed698-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed698-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed698-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed698-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed698-106">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="ed698-106">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="ed698-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed698-107">Methods</span></span>
|<span data-ttu-id="ed698-108">Método</span><span class="sxs-lookup"><span data-stu-id="ed698-108">Method</span></span>|<span data-ttu-id="ed698-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed698-109">Return Type</span></span>|<span data-ttu-id="ed698-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed698-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed698-111">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ed698-111">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="ed698-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ed698-112">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="ed698-113">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="ed698-113">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="ed698-114">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ed698-114">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="ed698-115">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="ed698-115">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="ed698-116">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="ed698-116">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="ed698-117">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="ed698-117">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="ed698-118">String</span><span class="sxs-lookup"><span data-stu-id="ed698-118">String</span></span>|<span data-ttu-id="ed698-119">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="ed698-119">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="ed698-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed698-120">Properties</span></span>
|<span data-ttu-id="ed698-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed698-121">Property</span></span>|<span data-ttu-id="ed698-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed698-122">Type</span></span>|<span data-ttu-id="ed698-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed698-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed698-124">id</span><span class="sxs-lookup"><span data-stu-id="ed698-124">id</span></span>|<span data-ttu-id="ed698-125">String</span><span class="sxs-lookup"><span data-stu-id="ed698-125">String</span></span>|<span data-ttu-id="ed698-126">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="ed698-126">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="ed698-127">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed698-127">appleIdentifier</span></span>|<span data-ttu-id="ed698-128">String</span><span class="sxs-lookup"><span data-stu-id="ed698-128">String</span></span>|<span data-ttu-id="ed698-129">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="ed698-129">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="ed698-130">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="ed698-130">topicIdentifier</span></span>|<span data-ttu-id="ed698-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed698-131">String</span></span>|<span data-ttu-id="ed698-132">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="ed698-132">Topic Id.</span></span>|
|<span data-ttu-id="ed698-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed698-133">lastModifiedDateTime</span></span>|<span data-ttu-id="ed698-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed698-134">DateTimeOffset</span></span>|<span data-ttu-id="ed698-135">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="ed698-135">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="ed698-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ed698-136">expirationDateTime</span></span>|<span data-ttu-id="ed698-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed698-137">DateTimeOffset</span></span>|<span data-ttu-id="ed698-138">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="ed698-138">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="ed698-139">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="ed698-139">certificateUploadStatus</span></span>|<span data-ttu-id="ed698-140">String</span><span class="sxs-lookup"><span data-stu-id="ed698-140">String</span></span>|<span data-ttu-id="ed698-141">O status do carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="ed698-141">The certificate upload status.</span></span>|
|<span data-ttu-id="ed698-142">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="ed698-142">certificateUploadFailureReason</span></span>|<span data-ttu-id="ed698-143">String</span><span class="sxs-lookup"><span data-stu-id="ed698-143">String</span></span>|<span data-ttu-id="ed698-144">O motivo da falha no carregamento do certificado.</span><span class="sxs-lookup"><span data-stu-id="ed698-144">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="ed698-145">certificado</span><span class="sxs-lookup"><span data-stu-id="ed698-145">certificate</span></span>|<span data-ttu-id="ed698-146">String</span><span class="sxs-lookup"><span data-stu-id="ed698-146">String</span></span>|<span data-ttu-id="ed698-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ed698-147">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed698-148">Relações</span><span class="sxs-lookup"><span data-stu-id="ed698-148">Relationships</span></span>
<span data-ttu-id="ed698-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed698-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed698-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed698-150">JSON Representation</span></span>
<span data-ttu-id="ed698-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed698-151">Here is a JSON representation of the resource.</span></span>
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



