---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ce016579729353f69f2e7671ff67b5da0004536
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464586"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="03f99-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="03f99-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="03f99-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03f99-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03f99-105">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="03f99-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="03f99-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03f99-106">Properties</span></span>
|<span data-ttu-id="03f99-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03f99-107">Property</span></span>|<span data-ttu-id="03f99-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="03f99-108">Type</span></span>|<span data-ttu-id="03f99-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="03f99-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03f99-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="03f99-110">bundleID</span></span>|<span data-ttu-id="03f99-111">String</span><span class="sxs-lookup"><span data-stu-id="03f99-111">String</span></span>|<span data-ttu-id="03f99-112">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="03f99-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="03f99-113">appName</span><span class="sxs-lookup"><span data-stu-id="03f99-113">appName</span></span>|<span data-ttu-id="03f99-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03f99-114">String</span></span>|<span data-ttu-id="03f99-115">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="03f99-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="03f99-116">publicador</span><span class="sxs-lookup"><span data-stu-id="03f99-116">publisher</span></span>|<span data-ttu-id="03f99-117">String</span><span class="sxs-lookup"><span data-stu-id="03f99-117">String</span></span>|<span data-ttu-id="03f99-118">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="03f99-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="03f99-119">enabled</span><span class="sxs-lookup"><span data-stu-id="03f99-119">enabled</span></span>|<span data-ttu-id="03f99-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="03f99-120">Boolean</span></span>|<span data-ttu-id="03f99-121">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="03f99-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="03f99-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="03f99-122">showInNotificationCenter</span></span>|<span data-ttu-id="03f99-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="03f99-123">Boolean</span></span>|<span data-ttu-id="03f99-124">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="03f99-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="03f99-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="03f99-125">showOnLockScreen</span></span>|<span data-ttu-id="03f99-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="03f99-126">Boolean</span></span>|<span data-ttu-id="03f99-127">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="03f99-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="03f99-128">alertType</span><span class="sxs-lookup"><span data-stu-id="03f99-128">alertType</span></span>|[<span data-ttu-id="03f99-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="03f99-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="03f99-130">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="03f99-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="03f99-131">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="03f99-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="03f99-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="03f99-132">badgesEnabled</span></span>|<span data-ttu-id="03f99-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="03f99-133">Boolean</span></span>|<span data-ttu-id="03f99-134">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="03f99-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="03f99-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="03f99-135">soundsEnabled</span></span>|<span data-ttu-id="03f99-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="03f99-136">Boolean</span></span>|<span data-ttu-id="03f99-137">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="03f99-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03f99-138">Relações</span><span class="sxs-lookup"><span data-stu-id="03f99-138">Relationships</span></span>
<span data-ttu-id="03f99-139">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="03f99-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03f99-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03f99-140">JSON Representation</span></span>
<span data-ttu-id="03f99-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03f99-141">Here is a JSON representation of the resource.</span></span>
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



