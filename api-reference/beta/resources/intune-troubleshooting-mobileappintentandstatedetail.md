---
title: tipo de recurso mobileAppIntentAndStateDetail
description: Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2392d9bc83fda65832cb123115ba1285c823174a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939018"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="8b25e-103">tipo de recurso mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="8b25e-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="8b25e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b25e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b25e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b25e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b25e-106">Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b25e-106">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="8b25e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b25e-107">Properties</span></span>
|<span data-ttu-id="8b25e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b25e-108">Property</span></span>|<span data-ttu-id="8b25e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b25e-109">Type</span></span>|<span data-ttu-id="8b25e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b25e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b25e-111">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="8b25e-111">applicationId</span></span>|<span data-ttu-id="8b25e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b25e-112">String</span></span>|<span data-ttu-id="8b25e-113">Identificador MobieApp.</span><span class="sxs-lookup"><span data-stu-id="8b25e-113">MobieApp identifier.</span></span>|
|<span data-ttu-id="8b25e-114">displayName</span><span class="sxs-lookup"><span data-stu-id="8b25e-114">displayName</span></span>|<span data-ttu-id="8b25e-115">String</span><span class="sxs-lookup"><span data-stu-id="8b25e-115">String</span></span>|<span data-ttu-id="8b25e-116">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8b25e-116">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="8b25e-117">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="8b25e-117">mobileAppIntent</span></span>|[<span data-ttu-id="8b25e-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="8b25e-118">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="8b25e-119">Tentativa de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8b25e-119">Mobile App Intent.</span></span> <span data-ttu-id="8b25e-120">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="8b25e-120">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="8b25e-121">displayVersion</span><span class="sxs-lookup"><span data-stu-id="8b25e-121">displayVersion</span></span>|<span data-ttu-id="8b25e-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8b25e-122">String</span></span>|<span data-ttu-id="8b25e-123">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b25e-123">Human readable version of the application</span></span>|
|<span data-ttu-id="8b25e-124">installState</span><span class="sxs-lookup"><span data-stu-id="8b25e-124">installState</span></span>|[<span data-ttu-id="8b25e-125">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="8b25e-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="8b25e-126">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b25e-126">The install state of the app.</span></span> <span data-ttu-id="8b25e-127">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="8b25e-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="8b25e-128">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="8b25e-128">supportedDeviceTypes</span></span>|<span data-ttu-id="8b25e-129">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="8b25e-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="8b25e-130">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b25e-130">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b25e-131">Relações</span><span class="sxs-lookup"><span data-stu-id="8b25e-131">Relationships</span></span>
<span data-ttu-id="8b25e-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8b25e-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b25e-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b25e-133">JSON Representation</span></span>
<span data-ttu-id="8b25e-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b25e-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```




