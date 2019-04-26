---
title: Tipo de recurso applePushNotificationCertificate
description: Certificado de notificação por push da Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41d5161f1e9344f187329bf795219151c91f29ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555882"
---
# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="08c72-103">Tipo de recurso applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="08c72-103">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="08c72-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08c72-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08c72-105">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="08c72-105">Apple push notification certificate.</span></span>

## <a name="methods"></a><span data-ttu-id="08c72-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="08c72-106">Methods</span></span>
|<span data-ttu-id="08c72-107">Método</span><span class="sxs-lookup"><span data-stu-id="08c72-107">Method</span></span>|<span data-ttu-id="08c72-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="08c72-108">Return Type</span></span>|<span data-ttu-id="08c72-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="08c72-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08c72-110">Obter applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="08c72-110">Get applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-get.md)|[<span data-ttu-id="08c72-111">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="08c72-111">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="08c72-112">Ler propriedades e relações de objetos de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="08c72-112">Read properties and relationships of the [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="08c72-113">Atualizar applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="08c72-113">Update applePushNotificationCertificate</span></span>](../api/intune-devices-applepushnotificationcertificate-update.md)|[<span data-ttu-id="08c72-114">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="08c72-114">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="08c72-115">Atualizar as propriedades de um objeto de [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="08c72-115">Update the properties of a [applePushNotificationCertificate](../resources/intune-devices-applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="08c72-116">Função downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="08c72-116">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="08c72-117">String</span><span class="sxs-lookup"><span data-stu-id="08c72-117">String</span></span>|<span data-ttu-id="08c72-118">Baixa a solicitação de assinatura de certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="08c72-118">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="08c72-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08c72-119">Properties</span></span>
|<span data-ttu-id="08c72-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08c72-120">Property</span></span>|<span data-ttu-id="08c72-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="08c72-121">Type</span></span>|<span data-ttu-id="08c72-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="08c72-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08c72-123">id</span><span class="sxs-lookup"><span data-stu-id="08c72-123">id</span></span>|<span data-ttu-id="08c72-124">String</span><span class="sxs-lookup"><span data-stu-id="08c72-124">String</span></span>|<span data-ttu-id="08c72-125">O identificador exclusivo do certificado.</span><span class="sxs-lookup"><span data-stu-id="08c72-125">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="08c72-126">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="08c72-126">appleIdentifier</span></span>|<span data-ttu-id="08c72-127">String</span><span class="sxs-lookup"><span data-stu-id="08c72-127">String</span></span>|<span data-ttu-id="08c72-128">Id da Apple da conta usada para criar o certificado de push do MDM.</span><span class="sxs-lookup"><span data-stu-id="08c72-128">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="08c72-129">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="08c72-129">topicIdentifier</span></span>|<span data-ttu-id="08c72-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08c72-130">String</span></span>|<span data-ttu-id="08c72-131">ID do tópico.</span><span class="sxs-lookup"><span data-stu-id="08c72-131">Topic Id.</span></span>|
|<span data-ttu-id="08c72-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08c72-132">lastModifiedDateTime</span></span>|<span data-ttu-id="08c72-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08c72-133">DateTimeOffset</span></span>|<span data-ttu-id="08c72-134">Data e hora da última modificação de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="08c72-134">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="08c72-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="08c72-135">expirationDateTime</span></span>|<span data-ttu-id="08c72-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08c72-136">DateTimeOffset</span></span>|<span data-ttu-id="08c72-137">Data e hora do vencimento de certificado de notificações por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="08c72-137">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="08c72-138">certificado</span><span class="sxs-lookup"><span data-stu-id="08c72-138">certificate</span></span>|<span data-ttu-id="08c72-139">String</span><span class="sxs-lookup"><span data-stu-id="08c72-139">String</span></span>|<span data-ttu-id="08c72-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="08c72-140">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="08c72-141">Relações</span><span class="sxs-lookup"><span data-stu-id="08c72-141">Relationships</span></span>
<span data-ttu-id="08c72-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08c72-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08c72-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08c72-143">JSON Representation</span></span>
<span data-ttu-id="08c72-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08c72-144">Here is a JSON representation of the resource.</span></span>
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



