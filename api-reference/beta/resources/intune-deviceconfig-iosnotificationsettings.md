---
title: Tipo de recurso iosNotificationSettings
description: Um item que descreve a configuração de notificação.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0503d938860798408fa5eb2af20ac51dc988f8a7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946445"
---
# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="f4e9a-103">Tipo de recurso iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="f4e9a-103">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="f4e9a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4e9a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4e9a-106">Um item que descreve a configuração de notificação.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-106">An item describing notification setting.</span></span>

## <a name="properties"></a><span data-ttu-id="f4e9a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4e9a-107">Properties</span></span>
|<span data-ttu-id="f4e9a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4e9a-108">Property</span></span>|<span data-ttu-id="f4e9a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4e9a-109">Type</span></span>|<span data-ttu-id="f4e9a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4e9a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4e9a-111">bundleID</span><span class="sxs-lookup"><span data-stu-id="f4e9a-111">bundleID</span></span>|<span data-ttu-id="f4e9a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4e9a-112">String</span></span>|<span data-ttu-id="f4e9a-113">Id de pacote do aplicativo ao qual aplicar essas configurações de notificação.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-113">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="f4e9a-114">appName</span><span class="sxs-lookup"><span data-stu-id="f4e9a-114">appName</span></span>|<span data-ttu-id="f4e9a-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4e9a-115">String</span></span>|<span data-ttu-id="f4e9a-116">Nome do aplicativo a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-116">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="f4e9a-117">publicador</span><span class="sxs-lookup"><span data-stu-id="f4e9a-117">publisher</span></span>|<span data-ttu-id="f4e9a-118">String</span><span class="sxs-lookup"><span data-stu-id="f4e9a-118">String</span></span>|<span data-ttu-id="f4e9a-119">Publicador a ser associado à bundleID.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-119">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="f4e9a-120">enabled</span><span class="sxs-lookup"><span data-stu-id="f4e9a-120">enabled</span></span>|<span data-ttu-id="f4e9a-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4e9a-121">Boolean</span></span>|<span data-ttu-id="f4e9a-122">Indica se são permitidas notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-122">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="f4e9a-123">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="f4e9a-123">showInNotificationCenter</span></span>|<span data-ttu-id="f4e9a-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4e9a-124">Boolean</span></span>|<span data-ttu-id="f4e9a-125">Indica se as notificações podem ser exibidas no centro de notificações.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-125">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="f4e9a-126">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="f4e9a-126">showOnLockScreen</span></span>|<span data-ttu-id="f4e9a-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4e9a-127">Boolean</span></span>|<span data-ttu-id="f4e9a-128">Indica se as notificações podem ser exibidas na tela de bloqueio.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-128">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="f4e9a-129">alertType</span><span class="sxs-lookup"><span data-stu-id="f4e9a-129">alertType</span></span>|[<span data-ttu-id="f4e9a-130">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="f4e9a-130">iosNotificationAlertType</span></span>](../resources/intune-deviceconfig-iosnotificationalerttype.md)|<span data-ttu-id="f4e9a-131">Indica o tipo de alerta para notificações neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-131">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="f4e9a-132">Os valores possíveis são: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-132">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="f4e9a-133">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="f4e9a-133">badgesEnabled</span></span>|<span data-ttu-id="f4e9a-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4e9a-134">Boolean</span></span>|<span data-ttu-id="f4e9a-135">Indica se serão permitidos selos neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-135">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="f4e9a-136">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="f4e9a-136">soundsEnabled</span></span>|<span data-ttu-id="f4e9a-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4e9a-137">Boolean</span></span>|<span data-ttu-id="f4e9a-138">Indica se são permitidos sons neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-138">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4e9a-139">Relações</span><span class="sxs-lookup"><span data-stu-id="f4e9a-139">Relationships</span></span>
<span data-ttu-id="f4e9a-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4e9a-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4e9a-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4e9a-141">JSON Representation</span></span>
<span data-ttu-id="f4e9a-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4e9a-142">Here is a JSON representation of the resource.</span></span>
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




