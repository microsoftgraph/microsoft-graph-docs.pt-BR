---
title: tipo de recurso mobileAppIntentAndStateDetail
description: Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 598cacd35ba5416c51388ef6ecb101d302ad9864
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523328"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="ebb3d-103">tipo de recurso mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="ebb3d-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="ebb3d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ebb3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebb3d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebb3d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebb3d-107">Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="ebb3d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebb3d-108">Properties</span></span>
|<span data-ttu-id="ebb3d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebb3d-109">Property</span></span>|<span data-ttu-id="ebb3d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebb3d-110">Type</span></span>|<span data-ttu-id="ebb3d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebb3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebb3d-112">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="ebb3d-112">applicationId</span></span>|<span data-ttu-id="ebb3d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ebb3d-113">String</span></span>|<span data-ttu-id="ebb3d-114">Identificador MobieApp.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="ebb3d-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ebb3d-115">displayName</span></span>|<span data-ttu-id="ebb3d-116">String</span><span class="sxs-lookup"><span data-stu-id="ebb3d-116">String</span></span>|<span data-ttu-id="ebb3d-117">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="ebb3d-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="ebb3d-118">mobileAppIntent</span></span>|[<span data-ttu-id="ebb3d-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="ebb3d-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="ebb3d-120">Tentativa de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-120">Mobile App Intent.</span></span> <span data-ttu-id="ebb3d-121">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="ebb3d-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="ebb3d-122">displayVersion</span></span>|<span data-ttu-id="ebb3d-123">String</span><span class="sxs-lookup"><span data-stu-id="ebb3d-123">String</span></span>|<span data-ttu-id="ebb3d-124">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebb3d-124">Human readable version of the application</span></span>|
|<span data-ttu-id="ebb3d-125">installState</span><span class="sxs-lookup"><span data-stu-id="ebb3d-125">installState</span></span>|[<span data-ttu-id="ebb3d-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="ebb3d-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="ebb3d-127">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-127">The install state of the app.</span></span> <span data-ttu-id="ebb3d-128">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="ebb3d-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="ebb3d-129">supportedDeviceTypes</span></span>|<span data-ttu-id="ebb3d-130">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="ebb3d-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="ebb3d-131">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebb3d-132">Relações</span><span class="sxs-lookup"><span data-stu-id="ebb3d-132">Relationships</span></span>
<span data-ttu-id="ebb3d-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ebb3d-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebb3d-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebb3d-134">JSON Representation</span></span>
<span data-ttu-id="ebb3d-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebb3d-135">Here is a JSON representation of the resource.</span></span>
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



