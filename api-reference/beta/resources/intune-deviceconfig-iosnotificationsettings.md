---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 242a15d4b636cf73f0e9a9f29a3f53ce17f2fd00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972975"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="4405b-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="4405b-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="4405b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4405b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4405b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4405b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4405b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4405b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4405b-107">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="4405b-107">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="4405b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4405b-108">Properties</span></span>
|<span data-ttu-id="4405b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4405b-109">Property</span></span>|<span data-ttu-id="4405b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4405b-110">Type</span></span>|<span data-ttu-id="4405b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4405b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4405b-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="4405b-112">bundleID</span></span>|<span data-ttu-id="4405b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4405b-113">String</span></span>|<span data-ttu-id="4405b-114">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="4405b-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="4405b-115">appName</span><span class="sxs-lookup"><span data-stu-id="4405b-115">appName</span></span>|<span data-ttu-id="4405b-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4405b-116">String</span></span>|<span data-ttu-id="4405b-117">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="4405b-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="4405b-118">publicador</span><span class="sxs-lookup"><span data-stu-id="4405b-118">publisher</span></span>|<span data-ttu-id="4405b-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4405b-119">String</span></span>|<span data-ttu-id="4405b-120">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="4405b-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="4405b-121">enabled</span><span class="sxs-lookup"><span data-stu-id="4405b-121">enabled</span></span>|<span data-ttu-id="4405b-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="4405b-122">Boolean</span></span>|<span data-ttu-id="4405b-123">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4405b-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="4405b-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="4405b-124">showInNotificationCenter</span></span>|<span data-ttu-id="4405b-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="4405b-125">Boolean</span></span>|<span data-ttu-id="4405b-126">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="4405b-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="4405b-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="4405b-127">showOnLockScreen</span></span>|<span data-ttu-id="4405b-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="4405b-128">Boolean</span></span>|<span data-ttu-id="4405b-129">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="4405b-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="4405b-130">alertType</span><span class="sxs-lookup"><span data-stu-id="4405b-130">alertType</span></span>|[<span data-ttu-id="4405b-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="4405b-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="4405b-132">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4405b-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="4405b-133">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="4405b-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="4405b-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="4405b-134">badgesEnabled</span></span>|<span data-ttu-id="4405b-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="4405b-135">Boolean</span></span>|<span data-ttu-id="4405b-136">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4405b-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="4405b-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="4405b-137">soundsEnabled</span></span>|<span data-ttu-id="4405b-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="4405b-138">Boolean</span></span>|<span data-ttu-id="4405b-139">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4405b-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4405b-140">Relações</span><span class="sxs-lookup"><span data-stu-id="4405b-140">Relationships</span></span>
<span data-ttu-id="4405b-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4405b-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4405b-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4405b-142">JSON Representation</span></span>
<span data-ttu-id="4405b-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4405b-143">Here is a JSON representation of the resource.</span></span>
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





