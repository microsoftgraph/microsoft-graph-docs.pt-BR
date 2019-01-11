---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2105d5641583f0d8216bd8f2241f40e5fbeea01d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810098"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="f1f5e-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="f1f5e-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="f1f5e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1f5e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1f5e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1f5e-107">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="f1f5e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1f5e-108">Properties</span></span>
|<span data-ttu-id="f1f5e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1f5e-109">Property</span></span>|<span data-ttu-id="f1f5e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1f5e-110">Type</span></span>|<span data-ttu-id="f1f5e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1f5e-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="f1f5e-112">bundleID</span></span>|<span data-ttu-id="f1f5e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f5e-113">String</span></span>|<span data-ttu-id="f1f5e-114">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="f1f5e-115">appName</span><span class="sxs-lookup"><span data-stu-id="f1f5e-115">appName</span></span>|<span data-ttu-id="f1f5e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f5e-116">String</span></span>|<span data-ttu-id="f1f5e-117">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="f1f5e-118">publicador</span><span class="sxs-lookup"><span data-stu-id="f1f5e-118">publisher</span></span>|<span data-ttu-id="f1f5e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f5e-119">String</span></span>|<span data-ttu-id="f1f5e-120">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="f1f5e-121">enabled</span><span class="sxs-lookup"><span data-stu-id="f1f5e-121">enabled</span></span>|<span data-ttu-id="f1f5e-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1f5e-122">Boolean</span></span>|<span data-ttu-id="f1f5e-123">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="f1f5e-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="f1f5e-124">showInNotificationCenter</span></span>|<span data-ttu-id="f1f5e-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1f5e-125">Boolean</span></span>|<span data-ttu-id="f1f5e-126">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="f1f5e-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f1f5e-127">showOnLockScreen</span></span>|<span data-ttu-id="f1f5e-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1f5e-128">Boolean</span></span>|<span data-ttu-id="f1f5e-129">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="f1f5e-130">alertType</span><span class="sxs-lookup"><span data-stu-id="f1f5e-130">alertType</span></span>|[<span data-ttu-id="f1f5e-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="f1f5e-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="f1f5e-132">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="f1f5e-133">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="f1f5e-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="f1f5e-134">badgesEnabled</span></span>|<span data-ttu-id="f1f5e-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1f5e-135">Boolean</span></span>|<span data-ttu-id="f1f5e-136">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="f1f5e-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="f1f5e-137">soundsEnabled</span></span>|<span data-ttu-id="f1f5e-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1f5e-138">Boolean</span></span>|<span data-ttu-id="f1f5e-139">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1f5e-140">Relações</span><span class="sxs-lookup"><span data-stu-id="f1f5e-140">Relationships</span></span>
<span data-ttu-id="f1f5e-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f1f5e-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1f5e-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1f5e-142">JSON Representation</span></span>
<span data-ttu-id="f1f5e-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1f5e-143">Here is a JSON representation of the resource.</span></span>
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





