---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f7e94d9db5c649329476b3df9a1489f9ffcfbba3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829985"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="de660-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="de660-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="de660-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="de660-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de660-105">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="de660-105">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="de660-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de660-106">Properties</span></span>
|<span data-ttu-id="de660-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de660-107">Property</span></span>|<span data-ttu-id="de660-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="de660-108">Type</span></span>|<span data-ttu-id="de660-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="de660-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de660-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="de660-110">bundleID</span></span>|<span data-ttu-id="de660-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de660-111">String</span></span>|<span data-ttu-id="de660-112">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="de660-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="de660-113">appName</span><span class="sxs-lookup"><span data-stu-id="de660-113">appName</span></span>|<span data-ttu-id="de660-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de660-114">String</span></span>|<span data-ttu-id="de660-115">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="de660-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="de660-116">publicador</span><span class="sxs-lookup"><span data-stu-id="de660-116">publisher</span></span>|<span data-ttu-id="de660-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de660-117">String</span></span>|<span data-ttu-id="de660-118">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="de660-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="de660-119">enabled</span><span class="sxs-lookup"><span data-stu-id="de660-119">enabled</span></span>|<span data-ttu-id="de660-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="de660-120">Boolean</span></span>|<span data-ttu-id="de660-121">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de660-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="de660-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="de660-122">showInNotificationCenter</span></span>|<span data-ttu-id="de660-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="de660-123">Boolean</span></span>|<span data-ttu-id="de660-124">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="de660-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="de660-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="de660-125">showOnLockScreen</span></span>|<span data-ttu-id="de660-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="de660-126">Boolean</span></span>|<span data-ttu-id="de660-127">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="de660-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="de660-128">alertType</span><span class="sxs-lookup"><span data-stu-id="de660-128">alertType</span></span>|[<span data-ttu-id="de660-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="de660-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="de660-130">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de660-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="de660-131">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="de660-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="de660-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="de660-132">badgesEnabled</span></span>|<span data-ttu-id="de660-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="de660-133">Boolean</span></span>|<span data-ttu-id="de660-134">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de660-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="de660-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="de660-135">soundsEnabled</span></span>|<span data-ttu-id="de660-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="de660-136">Boolean</span></span>|<span data-ttu-id="de660-137">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de660-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de660-138">Relações</span><span class="sxs-lookup"><span data-stu-id="de660-138">Relationships</span></span>
<span data-ttu-id="de660-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de660-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de660-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de660-140">JSON Representation</span></span>
<span data-ttu-id="de660-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de660-141">Here is a JSON representation of the resource.</span></span>
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



