---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c748c0ba5d21674438af0c7a60883ab8c9832e09
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790570"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="0f382-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="0f382-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="0f382-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f382-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f382-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f382-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f382-106">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="0f382-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="0f382-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f382-107">Properties</span></span>
|<span data-ttu-id="0f382-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f382-108">Property</span></span>|<span data-ttu-id="0f382-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f382-109">Type</span></span>|<span data-ttu-id="0f382-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f382-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f382-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="0f382-111">bundleID</span></span>|<span data-ttu-id="0f382-112">String</span><span class="sxs-lookup"><span data-stu-id="0f382-112">String</span></span>|<span data-ttu-id="0f382-113">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="0f382-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="0f382-114">appName</span><span class="sxs-lookup"><span data-stu-id="0f382-114">appName</span></span>|<span data-ttu-id="0f382-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f382-115">String</span></span>|<span data-ttu-id="0f382-116">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="0f382-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="0f382-117">publicador</span><span class="sxs-lookup"><span data-stu-id="0f382-117">publisher</span></span>|<span data-ttu-id="0f382-118">String</span><span class="sxs-lookup"><span data-stu-id="0f382-118">String</span></span>|<span data-ttu-id="0f382-119">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="0f382-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="0f382-120">enabled</span><span class="sxs-lookup"><span data-stu-id="0f382-120">enabled</span></span>|<span data-ttu-id="0f382-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f382-121">Boolean</span></span>|<span data-ttu-id="0f382-122">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f382-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="0f382-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="0f382-123">showInNotificationCenter</span></span>|<span data-ttu-id="0f382-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f382-124">Boolean</span></span>|<span data-ttu-id="0f382-125">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="0f382-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="0f382-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="0f382-126">showOnLockScreen</span></span>|<span data-ttu-id="0f382-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f382-127">Boolean</span></span>|<span data-ttu-id="0f382-128">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="0f382-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="0f382-129">alertType</span><span class="sxs-lookup"><span data-stu-id="0f382-129">alertType</span></span>|[<span data-ttu-id="0f382-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="0f382-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="0f382-131">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f382-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="0f382-132">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="0f382-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="0f382-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="0f382-133">badgesEnabled</span></span>|<span data-ttu-id="0f382-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f382-134">Boolean</span></span>|<span data-ttu-id="0f382-135">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f382-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="0f382-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="0f382-136">soundsEnabled</span></span>|<span data-ttu-id="0f382-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="0f382-137">Boolean</span></span>|<span data-ttu-id="0f382-138">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f382-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f382-139">Relações</span><span class="sxs-lookup"><span data-stu-id="0f382-139">Relationships</span></span>
<span data-ttu-id="0f382-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f382-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f382-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f382-141">JSON Representation</span></span>
<span data-ttu-id="0f382-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f382-142">Here is a JSON representation of the resource.</span></span>
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



