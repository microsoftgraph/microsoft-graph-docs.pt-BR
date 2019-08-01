---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 38ebee60ad5e4de642103a4cd72ae4f6cea0d9c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031476"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="0ee0d-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="0ee0d-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="0ee0d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ee0d-105">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="0ee0d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ee0d-106">Properties</span></span>
|<span data-ttu-id="0ee0d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ee0d-107">Property</span></span>|<span data-ttu-id="0ee0d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ee0d-108">Type</span></span>|<span data-ttu-id="0ee0d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ee0d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ee0d-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="0ee0d-110">bundleID</span></span>|<span data-ttu-id="0ee0d-111">String</span><span class="sxs-lookup"><span data-stu-id="0ee0d-111">String</span></span>|<span data-ttu-id="0ee0d-112">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="0ee0d-113">appName</span><span class="sxs-lookup"><span data-stu-id="0ee0d-113">appName</span></span>|<span data-ttu-id="0ee0d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0ee0d-114">String</span></span>|<span data-ttu-id="0ee0d-115">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="0ee0d-116">publicador</span><span class="sxs-lookup"><span data-stu-id="0ee0d-116">publisher</span></span>|<span data-ttu-id="0ee0d-117">String</span><span class="sxs-lookup"><span data-stu-id="0ee0d-117">String</span></span>|<span data-ttu-id="0ee0d-118">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="0ee0d-119">enabled</span><span class="sxs-lookup"><span data-stu-id="0ee0d-119">enabled</span></span>|<span data-ttu-id="0ee0d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ee0d-120">Boolean</span></span>|<span data-ttu-id="0ee0d-121">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="0ee0d-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="0ee0d-122">showInNotificationCenter</span></span>|<span data-ttu-id="0ee0d-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ee0d-123">Boolean</span></span>|<span data-ttu-id="0ee0d-124">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="0ee0d-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="0ee0d-125">showOnLockScreen</span></span>|<span data-ttu-id="0ee0d-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ee0d-126">Boolean</span></span>|<span data-ttu-id="0ee0d-127">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="0ee0d-128">alertType</span><span class="sxs-lookup"><span data-stu-id="0ee0d-128">alertType</span></span>|[<span data-ttu-id="0ee0d-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="0ee0d-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="0ee0d-130">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="0ee0d-131">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="0ee0d-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="0ee0d-132">badgesEnabled</span></span>|<span data-ttu-id="0ee0d-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ee0d-133">Boolean</span></span>|<span data-ttu-id="0ee0d-134">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="0ee0d-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="0ee0d-135">soundsEnabled</span></span>|<span data-ttu-id="0ee0d-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ee0d-136">Boolean</span></span>|<span data-ttu-id="0ee0d-137">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ee0d-138">Relações</span><span class="sxs-lookup"><span data-stu-id="0ee0d-138">Relationships</span></span>
<span data-ttu-id="0ee0d-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ee0d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ee0d-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ee0d-140">JSON Representation</span></span>
<span data-ttu-id="0ee0d-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ee0d-141">Here is a JSON representation of the resource.</span></span>
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



