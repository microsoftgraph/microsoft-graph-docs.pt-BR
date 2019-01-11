---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3cc0b4a3e35027f79dd79ab065de9632e9585873
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810861"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="df645-103">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df645-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="df645-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df645-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df645-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df645-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df645-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="df645-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df645-107">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="df645-107">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="df645-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="df645-108">Methods</span></span>
|<span data-ttu-id="df645-109">Método</span><span class="sxs-lookup"><span data-stu-id="df645-109">Method</span></span>|<span data-ttu-id="df645-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="df645-110">Return Type</span></span>|<span data-ttu-id="df645-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="df645-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="df645-112">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df645-112">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="df645-113">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df645-113">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="df645-114">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="df645-114">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="df645-115">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df645-115">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="df645-116">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="df645-116">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="df645-117">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="df645-117">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="df645-118">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="df645-118">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="df645-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df645-119">String</span></span>|<span data-ttu-id="df645-120">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="df645-120">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="df645-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df645-121">Properties</span></span>
|<span data-ttu-id="df645-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df645-122">Property</span></span>|<span data-ttu-id="df645-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="df645-123">Type</span></span>|<span data-ttu-id="df645-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="df645-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df645-125">id</span><span class="sxs-lookup"><span data-stu-id="df645-125">id</span></span>|<span data-ttu-id="df645-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df645-126">String</span></span>|<span data-ttu-id="df645-127">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="df645-127">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="df645-128">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="df645-128">appleIdentifier</span></span>|<span data-ttu-id="df645-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df645-129">String</span></span>|<span data-ttu-id="df645-130">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="df645-130">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="df645-131">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="df645-131">topicIdentifier</span></span>|<span data-ttu-id="df645-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df645-132">String</span></span>|<span data-ttu-id="df645-133">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="df645-133">Topic Id.</span></span>|
|<span data-ttu-id="df645-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df645-134">lastModifiedDateTime</span></span>|<span data-ttu-id="df645-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df645-135">DateTimeOffset</span></span>|<span data-ttu-id="df645-136">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="df645-136">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="df645-137">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="df645-137">expirationDateTime</span></span>|<span data-ttu-id="df645-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df645-138">DateTimeOffset</span></span>|<span data-ttu-id="df645-139">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="df645-139">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="df645-140">certificateUploadStatus</span><span class="sxs-lookup"><span data-stu-id="df645-140">certificateUploadStatus</span></span>|<span data-ttu-id="df645-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df645-141">String</span></span>|<span data-ttu-id="df645-142">O status de carregamento de certificado.</span><span class="sxs-lookup"><span data-stu-id="df645-142">The certificate upload status.</span></span>|
|<span data-ttu-id="df645-143">certificateUploadFailureReason</span><span class="sxs-lookup"><span data-stu-id="df645-143">certificateUploadFailureReason</span></span>|<span data-ttu-id="df645-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df645-144">String</span></span>|<span data-ttu-id="df645-145">O motivo pelo qual o carregamento do certificado falhou.</span><span class="sxs-lookup"><span data-stu-id="df645-145">The reason the certificate upload failed.</span></span>|
|<span data-ttu-id="df645-146">certificado</span><span class="sxs-lookup"><span data-stu-id="df645-146">certificate</span></span>|<span data-ttu-id="df645-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df645-147">String</span></span>|<span data-ttu-id="df645-148">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="df645-148">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="df645-149">Relações</span><span class="sxs-lookup"><span data-stu-id="df645-149">Relationships</span></span>
<span data-ttu-id="df645-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df645-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df645-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df645-151">JSON Representation</span></span>
<span data-ttu-id="df645-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df645-152">Here is a JSON representation of the resource.</span></span>
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





