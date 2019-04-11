---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d2fbc197f858b595bfe8572badddef9dadf6b3c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779640"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="6c161-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="6c161-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="6c161-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c161-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c161-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c161-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c161-106">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="6c161-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="6c161-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c161-107">Properties</span></span>
|<span data-ttu-id="6c161-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c161-108">Property</span></span>|<span data-ttu-id="6c161-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c161-109">Type</span></span>|<span data-ttu-id="6c161-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c161-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c161-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="6c161-111">bundleID</span></span>|<span data-ttu-id="6c161-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c161-112">String</span></span>|<span data-ttu-id="6c161-113">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="6c161-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="6c161-114">appName</span><span class="sxs-lookup"><span data-stu-id="6c161-114">appName</span></span>|<span data-ttu-id="6c161-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c161-115">String</span></span>|<span data-ttu-id="6c161-116">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="6c161-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="6c161-117">publicador</span><span class="sxs-lookup"><span data-stu-id="6c161-117">publisher</span></span>|<span data-ttu-id="6c161-118">String</span><span class="sxs-lookup"><span data-stu-id="6c161-118">String</span></span>|<span data-ttu-id="6c161-119">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="6c161-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="6c161-120">enabled</span><span class="sxs-lookup"><span data-stu-id="6c161-120">enabled</span></span>|<span data-ttu-id="6c161-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c161-121">Boolean</span></span>|<span data-ttu-id="6c161-122">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c161-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="6c161-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="6c161-123">showInNotificationCenter</span></span>|<span data-ttu-id="6c161-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c161-124">Boolean</span></span>|<span data-ttu-id="6c161-125">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="6c161-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="6c161-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="6c161-126">showOnLockScreen</span></span>|<span data-ttu-id="6c161-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c161-127">Boolean</span></span>|<span data-ttu-id="6c161-128">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="6c161-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="6c161-129">alertType</span><span class="sxs-lookup"><span data-stu-id="6c161-129">alertType</span></span>|[<span data-ttu-id="6c161-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="6c161-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="6c161-131">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c161-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="6c161-132">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="6c161-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="6c161-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="6c161-133">badgesEnabled</span></span>|<span data-ttu-id="6c161-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c161-134">Boolean</span></span>|<span data-ttu-id="6c161-135">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c161-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="6c161-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="6c161-136">soundsEnabled</span></span>|<span data-ttu-id="6c161-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c161-137">Boolean</span></span>|<span data-ttu-id="6c161-138">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c161-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c161-139">Relações</span><span class="sxs-lookup"><span data-stu-id="6c161-139">Relationships</span></span>
<span data-ttu-id="6c161-140">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6c161-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c161-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c161-141">JSON Representation</span></span>
<span data-ttu-id="6c161-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c161-142">Here is a JSON representation of the resource.</span></span>
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





