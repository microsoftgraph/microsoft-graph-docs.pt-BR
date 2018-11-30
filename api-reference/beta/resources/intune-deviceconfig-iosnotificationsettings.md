---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
ms.openlocfilehash: 515bf103c32694a16650986c91a3b719fad93236
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034836"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="c648d-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="c648d-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="c648d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c648d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c648d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c648d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c648d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c648d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c648d-107">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="c648d-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="c648d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c648d-108">Properties</span></span>
|<span data-ttu-id="c648d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c648d-109">Property</span></span>|<span data-ttu-id="c648d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c648d-110">Type</span></span>|<span data-ttu-id="c648d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c648d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c648d-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="c648d-112">bundleID</span></span>|<span data-ttu-id="c648d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c648d-113">String</span></span>|<span data-ttu-id="c648d-114">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="c648d-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="c648d-115">appName</span><span class="sxs-lookup"><span data-stu-id="c648d-115">appName</span></span>|<span data-ttu-id="c648d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c648d-116">String</span></span>|<span data-ttu-id="c648d-117">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="c648d-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="c648d-118">publicador</span><span class="sxs-lookup"><span data-stu-id="c648d-118">publisher</span></span>|<span data-ttu-id="c648d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c648d-119">String</span></span>|<span data-ttu-id="c648d-120">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="c648d-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="c648d-121">enabled</span><span class="sxs-lookup"><span data-stu-id="c648d-121">enabled</span></span>|<span data-ttu-id="c648d-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="c648d-122">Boolean</span></span>|<span data-ttu-id="c648d-123">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c648d-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="c648d-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="c648d-124">showInNotificationCenter</span></span>|<span data-ttu-id="c648d-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="c648d-125">Boolean</span></span>|<span data-ttu-id="c648d-126">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="c648d-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="c648d-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="c648d-127">showOnLockScreen</span></span>|<span data-ttu-id="c648d-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="c648d-128">Boolean</span></span>|<span data-ttu-id="c648d-129">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="c648d-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="c648d-130">alertType</span><span class="sxs-lookup"><span data-stu-id="c648d-130">alertType</span></span>|[<span data-ttu-id="c648d-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="c648d-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="c648d-132">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c648d-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="c648d-133">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="c648d-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="c648d-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="c648d-134">badgesEnabled</span></span>|<span data-ttu-id="c648d-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="c648d-135">Boolean</span></span>|<span data-ttu-id="c648d-136">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c648d-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="c648d-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="c648d-137">soundsEnabled</span></span>|<span data-ttu-id="c648d-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="c648d-138">Boolean</span></span>|<span data-ttu-id="c648d-139">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c648d-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c648d-140">Relações</span><span class="sxs-lookup"><span data-stu-id="c648d-140">Relationships</span></span>
<span data-ttu-id="c648d-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c648d-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c648d-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c648d-142">JSON Representation</span></span>
<span data-ttu-id="c648d-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c648d-143">Here is a JSON representation of the resource.</span></span>
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





