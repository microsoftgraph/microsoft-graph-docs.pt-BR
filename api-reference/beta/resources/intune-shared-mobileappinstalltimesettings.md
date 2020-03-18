---
title: tipo de recurso mobileAppInstallTimeSettings
description: Contém propriedades usadas para determinar quando oferecer um aplicativo a dispositivos e quando instalar o aplicativo em dispositivos.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 413d37ef0f672289e68e7dd8d8e2d0b6bc7d17ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768503"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="f3a92-103">tipo de recurso mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="f3a92-103">mobileAppInstallTimeSettings resource type</span></span>

> <span data-ttu-id="f3a92-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3a92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a92-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3a92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a92-106">Contém propriedades usadas para determinar quando oferecer um aplicativo a dispositivos e quando instalar o aplicativo em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f3a92-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="f3a92-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3a92-107">Properties</span></span>
|<span data-ttu-id="f3a92-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3a92-108">Property</span></span>|<span data-ttu-id="f3a92-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3a92-109">Type</span></span>|<span data-ttu-id="f3a92-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3a92-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3a92-111">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="f3a92-111">useLocalTime</span></span>|<span data-ttu-id="f3a92-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3a92-112">Boolean</span></span>|<span data-ttu-id="f3a92-113">Se a hora do dispositivo local ou a hora UTC deve ser usada ao determinar os horários disponíveis e prazos.</span><span class="sxs-lookup"><span data-stu-id="f3a92-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="f3a92-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f3a92-114">startDateTime</span></span>|<span data-ttu-id="f3a92-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3a92-115">DateTimeOffset</span></span>|<span data-ttu-id="f3a92-116">O horário em que o aplicativo deve estar disponível para instalação.</span><span class="sxs-lookup"><span data-stu-id="f3a92-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="f3a92-117">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="f3a92-117">deadlineDateTime</span></span>|<span data-ttu-id="f3a92-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3a92-118">DateTimeOffset</span></span>|<span data-ttu-id="f3a92-119">O horário em que o aplicativo deve ser instalado.</span><span class="sxs-lookup"><span data-stu-id="f3a92-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3a92-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f3a92-120">Relationships</span></span>
<span data-ttu-id="f3a92-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3a92-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3a92-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3a92-122">JSON Representation</span></span>
<span data-ttu-id="f3a92-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3a92-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallTimeSettings",
  "useLocalTime": true,
  "startDateTime": "String (timestamp)",
  "deadlineDateTime": "String (timestamp)"
}
```



