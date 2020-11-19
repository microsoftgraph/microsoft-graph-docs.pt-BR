---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ca6c5cf968897d701870bc695dcce909c74f1fc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280134"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="5636a-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="5636a-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="5636a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5636a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5636a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5636a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5636a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5636a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5636a-107">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="5636a-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="5636a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5636a-108">Properties</span></span>
|<span data-ttu-id="5636a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5636a-109">Property</span></span>|<span data-ttu-id="5636a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5636a-110">Type</span></span>|<span data-ttu-id="5636a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5636a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5636a-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="5636a-112">bundleID</span></span>|<span data-ttu-id="5636a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5636a-113">String</span></span>|<span data-ttu-id="5636a-114">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="5636a-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="5636a-115">appName</span><span class="sxs-lookup"><span data-stu-id="5636a-115">appName</span></span>|<span data-ttu-id="5636a-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5636a-116">String</span></span>|<span data-ttu-id="5636a-117">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="5636a-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="5636a-118">publicador</span><span class="sxs-lookup"><span data-stu-id="5636a-118">publisher</span></span>|<span data-ttu-id="5636a-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5636a-119">String</span></span>|<span data-ttu-id="5636a-120">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="5636a-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="5636a-121">enabled</span><span class="sxs-lookup"><span data-stu-id="5636a-121">enabled</span></span>|<span data-ttu-id="5636a-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="5636a-122">Boolean</span></span>|<span data-ttu-id="5636a-123">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5636a-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="5636a-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="5636a-124">showInNotificationCenter</span></span>|<span data-ttu-id="5636a-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="5636a-125">Boolean</span></span>|<span data-ttu-id="5636a-126">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="5636a-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="5636a-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="5636a-127">showOnLockScreen</span></span>|<span data-ttu-id="5636a-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="5636a-128">Boolean</span></span>|<span data-ttu-id="5636a-129">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="5636a-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="5636a-130">alertType</span><span class="sxs-lookup"><span data-stu-id="5636a-130">alertType</span></span>|[<span data-ttu-id="5636a-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="5636a-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="5636a-132">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5636a-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="5636a-133">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="5636a-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="5636a-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="5636a-134">badgesEnabled</span></span>|<span data-ttu-id="5636a-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="5636a-135">Boolean</span></span>|<span data-ttu-id="5636a-136">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5636a-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="5636a-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="5636a-137">soundsEnabled</span></span>|<span data-ttu-id="5636a-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="5636a-138">Boolean</span></span>|<span data-ttu-id="5636a-139">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5636a-139">Indicates whether sounds are allowed for this app.</span></span>|
|<span data-ttu-id="5636a-140">previewVisibility</span><span class="sxs-lookup"><span data-stu-id="5636a-140">previewVisibility</span></span>|[<span data-ttu-id="5636a-141">iosNotificationPreviewVisibility</span><span class="sxs-lookup"><span data-stu-id="5636a-141">iosNotificationPreviewVisibility</span></span>](../resources/intune-deviceconfig-iosnotificationpreviewvisibility.md)|<span data-ttu-id="5636a-142">Substitui a política de visualização de notificação definida pelo usuário em um dispositivo iOS.</span><span class="sxs-lookup"><span data-stu-id="5636a-142">Overrides the notification preview policy set by the user on an iOS device.</span></span> <span data-ttu-id="5636a-143">Os valores possíveis são: `notConfigured`, `alwaysShow`, `hideWhenLocked`, `neverShow`.</span><span class="sxs-lookup"><span data-stu-id="5636a-143">Possible values are: `notConfigured`, `alwaysShow`, `hideWhenLocked`, `neverShow`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5636a-144">Relações</span><span class="sxs-lookup"><span data-stu-id="5636a-144">Relationships</span></span>
<span data-ttu-id="5636a-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5636a-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5636a-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5636a-146">JSON Representation</span></span>
<span data-ttu-id="5636a-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5636a-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true,
  "previewVisibility": "String"
}
```




