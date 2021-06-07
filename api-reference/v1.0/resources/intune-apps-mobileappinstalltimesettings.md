---
title: Tipo de recurso mobileAppInstallTimeSettings
description: Contém propriedades usadas para determinar quando oferecer um aplicativo para dispositivos e quando instalar o aplicativo em dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bb768938ffa2e167f13a267451041b65f39011c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755116"
---
# <a name="mobileappinstalltimesettings-resource-type"></a><span data-ttu-id="56325-103">Tipo de recurso mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="56325-103">mobileAppInstallTimeSettings resource type</span></span>

<span data-ttu-id="56325-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56325-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56325-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56325-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56325-106">Contém propriedades usadas para determinar quando oferecer um aplicativo para dispositivos e quando instalar o aplicativo em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="56325-106">Contains properties used to determine when to offer an app to devices and when to install the app on devices.</span></span>

## <a name="properties"></a><span data-ttu-id="56325-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56325-107">Properties</span></span>
|<span data-ttu-id="56325-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56325-108">Property</span></span>|<span data-ttu-id="56325-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="56325-109">Type</span></span>|<span data-ttu-id="56325-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="56325-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56325-111">useLocalTime</span><span class="sxs-lookup"><span data-stu-id="56325-111">useLocalTime</span></span>|<span data-ttu-id="56325-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="56325-112">Boolean</span></span>|<span data-ttu-id="56325-113">Se a hora do dispositivo local ou utc deve ser usada ao determinar os tempos disponíveis e de prazo.</span><span class="sxs-lookup"><span data-stu-id="56325-113">Whether the local device time or UTC time should be used when determining the available and deadline times.</span></span>|
|<span data-ttu-id="56325-114">startDateTime</span><span class="sxs-lookup"><span data-stu-id="56325-114">startDateTime</span></span>|<span data-ttu-id="56325-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56325-115">DateTimeOffset</span></span>|<span data-ttu-id="56325-116">O momento em que o aplicativo deve estar disponível para instalação.</span><span class="sxs-lookup"><span data-stu-id="56325-116">The time at which the app should be available for installation.</span></span>|
|<span data-ttu-id="56325-117">deadlineDateTime</span><span class="sxs-lookup"><span data-stu-id="56325-117">deadlineDateTime</span></span>|<span data-ttu-id="56325-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56325-118">DateTimeOffset</span></span>|<span data-ttu-id="56325-119">O momento em que o aplicativo deve ser instalado.</span><span class="sxs-lookup"><span data-stu-id="56325-119">The time at which the app should be installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56325-120">Relações</span><span class="sxs-lookup"><span data-stu-id="56325-120">Relationships</span></span>
<span data-ttu-id="56325-121">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="56325-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56325-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56325-122">JSON Representation</span></span>
<span data-ttu-id="56325-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56325-123">Here is a JSON representation of the resource.</span></span>
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




