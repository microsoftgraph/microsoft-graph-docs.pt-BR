---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ceffa61669b9601e85e354e856c80a85d025f8b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410439"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="0232b-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="0232b-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="0232b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0232b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0232b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0232b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0232b-106">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="0232b-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="0232b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0232b-107">Properties</span></span>
|<span data-ttu-id="0232b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0232b-108">Property</span></span>|<span data-ttu-id="0232b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0232b-109">Type</span></span>|<span data-ttu-id="0232b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0232b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0232b-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="0232b-111">bundleID</span></span>|<span data-ttu-id="0232b-112">String</span><span class="sxs-lookup"><span data-stu-id="0232b-112">String</span></span>|<span data-ttu-id="0232b-113">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="0232b-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="0232b-114">appName</span><span class="sxs-lookup"><span data-stu-id="0232b-114">appName</span></span>|<span data-ttu-id="0232b-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0232b-115">String</span></span>|<span data-ttu-id="0232b-116">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="0232b-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="0232b-117">publicador</span><span class="sxs-lookup"><span data-stu-id="0232b-117">publisher</span></span>|<span data-ttu-id="0232b-118">String</span><span class="sxs-lookup"><span data-stu-id="0232b-118">String</span></span>|<span data-ttu-id="0232b-119">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="0232b-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="0232b-120">enabled</span><span class="sxs-lookup"><span data-stu-id="0232b-120">enabled</span></span>|<span data-ttu-id="0232b-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="0232b-121">Boolean</span></span>|<span data-ttu-id="0232b-122">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0232b-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="0232b-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="0232b-123">showInNotificationCenter</span></span>|<span data-ttu-id="0232b-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="0232b-124">Boolean</span></span>|<span data-ttu-id="0232b-125">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="0232b-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="0232b-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="0232b-126">showOnLockScreen</span></span>|<span data-ttu-id="0232b-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="0232b-127">Boolean</span></span>|<span data-ttu-id="0232b-128">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="0232b-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="0232b-129">alertType</span><span class="sxs-lookup"><span data-stu-id="0232b-129">alertType</span></span>|[<span data-ttu-id="0232b-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="0232b-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="0232b-131">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0232b-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="0232b-132">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="0232b-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="0232b-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="0232b-133">badgesEnabled</span></span>|<span data-ttu-id="0232b-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="0232b-134">Boolean</span></span>|<span data-ttu-id="0232b-135">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0232b-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="0232b-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="0232b-136">soundsEnabled</span></span>|<span data-ttu-id="0232b-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="0232b-137">Boolean</span></span>|<span data-ttu-id="0232b-138">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0232b-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0232b-139">Relações</span><span class="sxs-lookup"><span data-stu-id="0232b-139">Relationships</span></span>
<span data-ttu-id="0232b-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0232b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0232b-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0232b-141">JSON Representation</span></span>
<span data-ttu-id="0232b-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0232b-142">Here is a JSON representation of the resource.</span></span>
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
  "soundsEnabled": true
}
```







