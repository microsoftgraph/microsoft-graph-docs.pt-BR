---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f07561029d35d945eca118f095496891c73a25a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941734"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="bc406-103">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="bc406-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="bc406-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc406-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc406-105">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="bc406-105">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="bc406-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="bc406-106">Methods</span></span>
|<span data-ttu-id="bc406-107">Método</span><span class="sxs-lookup"><span data-stu-id="bc406-107">Method</span></span>|<span data-ttu-id="bc406-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc406-108">Return Type</span></span>|<span data-ttu-id="bc406-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc406-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc406-110">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="bc406-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="bc406-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="bc406-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="bc406-112">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="bc406-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="bc406-113">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="bc406-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="bc406-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="bc406-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="bc406-115">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="bc406-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="bc406-116">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="bc406-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="bc406-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc406-117">String</span></span>|<span data-ttu-id="bc406-118">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="bc406-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="bc406-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc406-119">Properties</span></span>
|<span data-ttu-id="bc406-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc406-120">Property</span></span>|<span data-ttu-id="bc406-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc406-121">Type</span></span>|<span data-ttu-id="bc406-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc406-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc406-123">id</span><span class="sxs-lookup"><span data-stu-id="bc406-123">id</span></span>|<span data-ttu-id="bc406-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc406-124">String</span></span>|<span data-ttu-id="bc406-125">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="bc406-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="bc406-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc406-126">appleIdentifier</span></span>|<span data-ttu-id="bc406-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc406-127">String</span></span>|<span data-ttu-id="bc406-128">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="bc406-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="bc406-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="bc406-129">topicIdentifier</span></span>|<span data-ttu-id="bc406-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc406-130">String</span></span>|<span data-ttu-id="bc406-131">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="bc406-131">Topic Id.</span></span>|
|<span data-ttu-id="bc406-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc406-132">lastModifiedDateTime</span></span>|<span data-ttu-id="bc406-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc406-133">DateTimeOffset</span></span>|<span data-ttu-id="bc406-134">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="bc406-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="bc406-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bc406-135">expirationDateTime</span></span>|<span data-ttu-id="bc406-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc406-136">DateTimeOffset</span></span>|<span data-ttu-id="bc406-137">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="bc406-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="bc406-138">certificado</span><span class="sxs-lookup"><span data-stu-id="bc406-138">certificate</span></span>|<span data-ttu-id="bc406-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc406-139">String</span></span>|<span data-ttu-id="bc406-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bc406-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc406-141">Relações</span><span class="sxs-lookup"><span data-stu-id="bc406-141">Relationships</span></span>
<span data-ttu-id="bc406-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc406-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc406-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc406-143">JSON Representation</span></span>
<span data-ttu-id="bc406-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc406-144">Here is a JSON representation of the resource.</span></span>
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



