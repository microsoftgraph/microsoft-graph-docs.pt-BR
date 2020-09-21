---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bfe71a68abd7ca55da6bb92654d8af0750a1ef22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003714"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="6ddcc-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="6ddcc-103">iosNotificationSettings resource type</span></span>

<span data-ttu-id="6ddcc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ddcc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ddcc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ddcc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ddcc-107">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-107">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="6ddcc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ddcc-108">Properties</span></span>
|<span data-ttu-id="6ddcc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ddcc-109">Property</span></span>|<span data-ttu-id="6ddcc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ddcc-110">Type</span></span>|<span data-ttu-id="6ddcc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ddcc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ddcc-112">bundleID</span><span class="sxs-lookup"><span data-stu-id="6ddcc-112">bundleID</span></span>|<span data-ttu-id="6ddcc-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ddcc-113">String</span></span>|<span data-ttu-id="6ddcc-114">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-114">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="6ddcc-115">appName</span><span class="sxs-lookup"><span data-stu-id="6ddcc-115">appName</span></span>|<span data-ttu-id="6ddcc-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ddcc-116">String</span></span>|<span data-ttu-id="6ddcc-117">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-117">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="6ddcc-118">publicador</span><span class="sxs-lookup"><span data-stu-id="6ddcc-118">publisher</span></span>|<span data-ttu-id="6ddcc-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ddcc-119">String</span></span>|<span data-ttu-id="6ddcc-120">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-120">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="6ddcc-121">enabled</span><span class="sxs-lookup"><span data-stu-id="6ddcc-121">enabled</span></span>|<span data-ttu-id="6ddcc-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ddcc-122">Boolean</span></span>|<span data-ttu-id="6ddcc-123">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-123">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="6ddcc-124">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="6ddcc-124">showInNotificationCenter</span></span>|<span data-ttu-id="6ddcc-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ddcc-125">Boolean</span></span>|<span data-ttu-id="6ddcc-126">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-126">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="6ddcc-127">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="6ddcc-127">showOnLockScreen</span></span>|<span data-ttu-id="6ddcc-128">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ddcc-128">Boolean</span></span>|<span data-ttu-id="6ddcc-129">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-129">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="6ddcc-130">alertType</span><span class="sxs-lookup"><span data-stu-id="6ddcc-130">alertType</span></span>|[<span data-ttu-id="6ddcc-131">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="6ddcc-131">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="6ddcc-132">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-132">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="6ddcc-133">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-133">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="6ddcc-134">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="6ddcc-134">badgesEnabled</span></span>|<span data-ttu-id="6ddcc-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ddcc-135">Boolean</span></span>|<span data-ttu-id="6ddcc-136">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-136">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="6ddcc-137">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="6ddcc-137">soundsEnabled</span></span>|<span data-ttu-id="6ddcc-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="6ddcc-138">Boolean</span></span>|<span data-ttu-id="6ddcc-139">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-139">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ddcc-140">Relações</span><span class="sxs-lookup"><span data-stu-id="6ddcc-140">Relationships</span></span>
<span data-ttu-id="6ddcc-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ddcc-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ddcc-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ddcc-142">JSON Representation</span></span>
<span data-ttu-id="6ddcc-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ddcc-143">Here is a JSON representation of the resource.</span></span>
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






