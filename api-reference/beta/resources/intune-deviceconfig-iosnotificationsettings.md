---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7db0b6ba438522db0795f6897daba8b5c43258c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420497"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="aa957-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="aa957-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="aa957-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="aa957-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aa957-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="aa957-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa957-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="aa957-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa957-107">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="aa957-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="aa957-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa957-108">Properties</span></span>
|<span data-ttu-id="aa957-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa957-109">Property</span></span>|<span data-ttu-id="aa957-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa957-110">Type</span></span>|<span data-ttu-id="aa957-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa957-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa957-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="aa957-112">bundleID</span></span>|<span data-ttu-id="aa957-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa957-113">String</span></span>|<span data-ttu-id="aa957-114">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="aa957-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="aa957-115">appName</span><span class="sxs-lookup"><span data-stu-id="aa957-115">appName</span></span>|<span data-ttu-id="aa957-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa957-116">String</span></span>|<span data-ttu-id="aa957-117">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="aa957-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="aa957-118">publicador</span><span class="sxs-lookup"><span data-stu-id="aa957-118">publisher</span></span>|<span data-ttu-id="aa957-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa957-119">String</span></span>|<span data-ttu-id="aa957-120">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="aa957-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="aa957-121">enabled</span><span class="sxs-lookup"><span data-stu-id="aa957-121">enabled</span></span>|<span data-ttu-id="aa957-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa957-122">Boolean</span></span>|<span data-ttu-id="aa957-123">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aa957-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="aa957-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="aa957-124">showInNotificationCenter</span></span>|<span data-ttu-id="aa957-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa957-125">Boolean</span></span>|<span data-ttu-id="aa957-126">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="aa957-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="aa957-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="aa957-127">showOnLockScreen</span></span>|<span data-ttu-id="aa957-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa957-128">Boolean</span></span>|<span data-ttu-id="aa957-129">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="aa957-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="aa957-130">alertType</span><span class="sxs-lookup"><span data-stu-id="aa957-130">alertType</span></span>|[<span data-ttu-id="aa957-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="aa957-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="aa957-132">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aa957-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="aa957-133">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="aa957-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="aa957-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="aa957-134">badgesEnabled</span></span>|<span data-ttu-id="aa957-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa957-135">Boolean</span></span>|<span data-ttu-id="aa957-136">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aa957-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="aa957-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="aa957-137">soundsEnabled</span></span>|<span data-ttu-id="aa957-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="aa957-138">Boolean</span></span>|<span data-ttu-id="aa957-139">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aa957-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa957-140">Relações</span><span class="sxs-lookup"><span data-stu-id="aa957-140">Relationships</span></span>
<span data-ttu-id="aa957-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa957-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa957-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa957-142">JSON Representation</span></span>
<span data-ttu-id="aa957-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa957-143">Here is a JSON representation of the resource.</span></span>
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




