---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 438b1cf075aa1e1cedafc8340b33186965691424
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760026"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="3e52d-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="3e52d-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="3e52d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e52d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e52d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e52d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e52d-106">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="3e52d-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="3e52d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e52d-107">Properties</span></span>
|<span data-ttu-id="3e52d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e52d-108">Property</span></span>|<span data-ttu-id="3e52d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e52d-109">Type</span></span>|<span data-ttu-id="3e52d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e52d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e52d-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="3e52d-111">bundleID</span></span>|<span data-ttu-id="3e52d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e52d-112">String</span></span>|<span data-ttu-id="3e52d-113">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="3e52d-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="3e52d-114">appName</span><span class="sxs-lookup"><span data-stu-id="3e52d-114">appName</span></span>|<span data-ttu-id="3e52d-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e52d-115">String</span></span>|<span data-ttu-id="3e52d-116">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="3e52d-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="3e52d-117">publicador</span><span class="sxs-lookup"><span data-stu-id="3e52d-117">publisher</span></span>|<span data-ttu-id="3e52d-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3e52d-118">String</span></span>|<span data-ttu-id="3e52d-119">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="3e52d-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="3e52d-120">enabled</span><span class="sxs-lookup"><span data-stu-id="3e52d-120">enabled</span></span>|<span data-ttu-id="3e52d-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e52d-121">Boolean</span></span>|<span data-ttu-id="3e52d-122">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3e52d-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="3e52d-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="3e52d-123">showInNotificationCenter</span></span>|<span data-ttu-id="3e52d-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e52d-124">Boolean</span></span>|<span data-ttu-id="3e52d-125">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="3e52d-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="3e52d-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="3e52d-126">showOnLockScreen</span></span>|<span data-ttu-id="3e52d-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e52d-127">Boolean</span></span>|<span data-ttu-id="3e52d-128">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="3e52d-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="3e52d-129">alertType</span><span class="sxs-lookup"><span data-stu-id="3e52d-129">alertType</span></span>|[<span data-ttu-id="3e52d-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="3e52d-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="3e52d-131">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3e52d-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="3e52d-132">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="3e52d-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="3e52d-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="3e52d-133">badgesEnabled</span></span>|<span data-ttu-id="3e52d-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e52d-134">Boolean</span></span>|<span data-ttu-id="3e52d-135">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3e52d-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="3e52d-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="3e52d-136">soundsEnabled</span></span>|<span data-ttu-id="3e52d-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="3e52d-137">Boolean</span></span>|<span data-ttu-id="3e52d-138">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3e52d-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e52d-139">Relações</span><span class="sxs-lookup"><span data-stu-id="3e52d-139">Relationships</span></span>
<span data-ttu-id="3e52d-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e52d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e52d-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e52d-141">JSON Representation</span></span>
<span data-ttu-id="3e52d-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e52d-142">Here is a JSON representation of the resource.</span></span>
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




