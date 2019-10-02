---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 993266d2a96946bf9f22b2c66c26db48e9915837
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359933"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="8c908-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="8c908-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="8c908-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c908-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c908-105">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="8c908-105">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="8c908-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c908-106">Properties</span></span>
|<span data-ttu-id="8c908-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c908-107">Property</span></span>|<span data-ttu-id="8c908-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c908-108">Type</span></span>|<span data-ttu-id="8c908-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c908-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c908-110">bundleID</span><span class="sxs-lookup"><span data-stu-id="8c908-110">bundleID</span></span>|<span data-ttu-id="8c908-111">String</span><span class="sxs-lookup"><span data-stu-id="8c908-111">String</span></span>|<span data-ttu-id="8c908-112">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="8c908-112">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="8c908-113">appName</span><span class="sxs-lookup"><span data-stu-id="8c908-113">appName</span></span>|<span data-ttu-id="8c908-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c908-114">String</span></span>|<span data-ttu-id="8c908-115">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="8c908-115">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="8c908-116">publicador</span><span class="sxs-lookup"><span data-stu-id="8c908-116">publisher</span></span>|<span data-ttu-id="8c908-117">String</span><span class="sxs-lookup"><span data-stu-id="8c908-117">String</span></span>|<span data-ttu-id="8c908-118">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="8c908-118">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="8c908-119">enabled</span><span class="sxs-lookup"><span data-stu-id="8c908-119">enabled</span></span>|<span data-ttu-id="8c908-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c908-120">Boolean</span></span>|<span data-ttu-id="8c908-121">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c908-121">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="8c908-122">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="8c908-122">showInNotificationCenter</span></span>|<span data-ttu-id="8c908-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c908-123">Boolean</span></span>|<span data-ttu-id="8c908-124">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="8c908-124">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="8c908-125">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="8c908-125">showOnLockScreen</span></span>|<span data-ttu-id="8c908-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c908-126">Boolean</span></span>|<span data-ttu-id="8c908-127">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="8c908-127">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="8c908-128">alertType</span><span class="sxs-lookup"><span data-stu-id="8c908-128">alertType</span></span>|[<span data-ttu-id="8c908-129">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="8c908-129">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="8c908-130">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c908-130">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="8c908-131">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="8c908-131">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="8c908-132">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="8c908-132">badgesEnabled</span></span>|<span data-ttu-id="8c908-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c908-133">Boolean</span></span>|<span data-ttu-id="8c908-134">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c908-134">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="8c908-135">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="8c908-135">soundsEnabled</span></span>|<span data-ttu-id="8c908-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c908-136">Boolean</span></span>|<span data-ttu-id="8c908-137">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8c908-137">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c908-138">Relações</span><span class="sxs-lookup"><span data-stu-id="8c908-138">Relationships</span></span>
<span data-ttu-id="8c908-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c908-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c908-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c908-140">JSON Representation</span></span>
<span data-ttu-id="8c908-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c908-141">Here is a JSON representation of the resource.</span></span>
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




