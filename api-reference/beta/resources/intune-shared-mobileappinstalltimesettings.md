---
title: tipo de recurso mobileAppInstallTimeSettings
description: Contém propriedades usadas para determinar quando oferecer um aplicativo a dispositivos e quando instalar o aplicativo em dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 835a7f2f9a104b855a54de699dab83df744af5f3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084181"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="8cbb6-103">tipo de recurso mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="8cbb6-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="8cbb6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cbb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cbb6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cbb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cbb6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cbb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cbb6-107">Contém propriedades usadas para determinar quando oferecer um aplicativo a dispositivos e quando instalar o aplicativo em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="8cbb6-107">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="8cbb6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cbb6-108">Properties</span></span>
|<span data-ttu-id="8cbb6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cbb6-109">Property</span></span>|<span data-ttu-id="8cbb6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cbb6-110">Type</span></span>|<span data-ttu-id="8cbb6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cbb6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cbb6-112">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="8cbb6-112">useLocalTime</span></span>|<span data-ttu-id="8cbb6-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cbb6-113">Boolean</span></span>|<span data-ttu-id="8cbb6-114">Se a hora do dispositivo local ou a hora UTC deve ser usada ao determinar os horários disponíveis e prazos.</span><span class="sxs-lookup"><span data-stu-id="8cbb6-114">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="8cbb6-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8cbb6-115">startDateTime</span></span>|<span data-ttu-id="8cbb6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cbb6-116">DateTimeOffset</span></span>|<span data-ttu-id="8cbb6-117">O horário em que o aplicativo deve estar disponível para instalação.</span><span class="sxs-lookup"><span data-stu-id="8cbb6-117">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="8cbb6-118">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="8cbb6-118">deadlineDateTime</span></span>|<span data-ttu-id="8cbb6-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cbb6-119">DateTimeOffset</span></span>|<span data-ttu-id="8cbb6-120">O horário em que o aplicativo deve ser instalado.</span><span class="sxs-lookup"><span data-stu-id="8cbb6-120">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cbb6-121">Relações</span><span class="sxs-lookup"><span data-stu-id="8cbb6-121">Relationships</span></span>
<span data-ttu-id="8cbb6-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cbb6-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cbb6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cbb6-123">JSON Representation</span></span>
<span data-ttu-id="8cbb6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cbb6-124">Here is a JSON representation of the resource.</span></span>
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






