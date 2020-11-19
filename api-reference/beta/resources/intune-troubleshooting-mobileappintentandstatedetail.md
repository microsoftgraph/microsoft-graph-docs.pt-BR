---
title: tipo de recurso mobileAppIntentAndStateDetail
description: Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca3645c5af594e5352e0fcd0dae70516e0548fba
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271594"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="071ae-103">tipo de recurso mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="071ae-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="071ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="071ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="071ae-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="071ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="071ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="071ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="071ae-107">Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="071ae-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="071ae-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="071ae-108">Properties</span></span>
|<span data-ttu-id="071ae-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="071ae-109">Property</span></span>|<span data-ttu-id="071ae-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="071ae-110">Type</span></span>|<span data-ttu-id="071ae-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="071ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="071ae-112">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="071ae-112">applicationId</span></span>|<span data-ttu-id="071ae-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="071ae-113">String</span></span>|<span data-ttu-id="071ae-114">Identificador MobieApp.</span><span class="sxs-lookup"><span data-stu-id="071ae-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="071ae-115">displayName</span><span class="sxs-lookup"><span data-stu-id="071ae-115">displayName</span></span>|<span data-ttu-id="071ae-116">String</span><span class="sxs-lookup"><span data-stu-id="071ae-116">String</span></span>|<span data-ttu-id="071ae-117">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="071ae-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="071ae-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="071ae-118">mobileAppIntent</span></span>|[<span data-ttu-id="071ae-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="071ae-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="071ae-120">Tentativa de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="071ae-120">Mobile App Intent.</span></span> <span data-ttu-id="071ae-121">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="071ae-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="071ae-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="071ae-122">displayVersion</span></span>|<span data-ttu-id="071ae-123">String</span><span class="sxs-lookup"><span data-stu-id="071ae-123">String</span></span>|<span data-ttu-id="071ae-124">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="071ae-124">Human readable version of the application</span></span>|
|<span data-ttu-id="071ae-125">installState</span><span class="sxs-lookup"><span data-stu-id="071ae-125">installState</span></span>|[<span data-ttu-id="071ae-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="071ae-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="071ae-127">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="071ae-127">The install state of the app.</span></span> <span data-ttu-id="071ae-128">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="071ae-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="071ae-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="071ae-129">supportedDeviceTypes</span></span>|<span data-ttu-id="071ae-130">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="071ae-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="071ae-131">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="071ae-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="071ae-132">Relações</span><span class="sxs-lookup"><span data-stu-id="071ae-132">Relationships</span></span>
<span data-ttu-id="071ae-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="071ae-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="071ae-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="071ae-134">JSON Representation</span></span>
<span data-ttu-id="071ae-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="071ae-135">Here is a JSON representation of the resource.</span></span>
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




