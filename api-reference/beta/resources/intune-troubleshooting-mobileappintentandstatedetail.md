---
title: tipo de recurso mobileAppIntentAndStateDetail
description: Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9511053bf11771bc3c766ab47672864b92d08cad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460577"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="04985-103">tipo de recurso mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="04985-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="04985-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04985-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04985-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04985-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04985-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04985-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04985-107">Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="04985-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="04985-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04985-108">Properties</span></span>
|<span data-ttu-id="04985-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04985-109">Property</span></span>|<span data-ttu-id="04985-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04985-110">Type</span></span>|<span data-ttu-id="04985-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04985-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04985-112">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="04985-112">applicationId</span></span>|<span data-ttu-id="04985-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04985-113">String</span></span>|<span data-ttu-id="04985-114">Identificador MobieApp.</span><span class="sxs-lookup"><span data-stu-id="04985-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="04985-115">displayName</span><span class="sxs-lookup"><span data-stu-id="04985-115">displayName</span></span>|<span data-ttu-id="04985-116">String</span><span class="sxs-lookup"><span data-stu-id="04985-116">String</span></span>|<span data-ttu-id="04985-117">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="04985-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="04985-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="04985-118">mobileAppIntent</span></span>|[<span data-ttu-id="04985-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="04985-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="04985-120">Tentativa de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="04985-120">Mobile App Intent.</span></span> <span data-ttu-id="04985-121">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="04985-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="04985-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="04985-122">displayVersion</span></span>|<span data-ttu-id="04985-123">String</span><span class="sxs-lookup"><span data-stu-id="04985-123">String</span></span>|<span data-ttu-id="04985-124">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="04985-124">Human readable version of the application</span></span>|
|<span data-ttu-id="04985-125">installState</span><span class="sxs-lookup"><span data-stu-id="04985-125">installState</span></span>|[<span data-ttu-id="04985-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="04985-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="04985-127">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04985-127">The install state of the app.</span></span> <span data-ttu-id="04985-128">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="04985-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="04985-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="04985-129">supportedDeviceTypes</span></span>|<span data-ttu-id="04985-130">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="04985-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="04985-131">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04985-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04985-132">Relações</span><span class="sxs-lookup"><span data-stu-id="04985-132">Relationships</span></span>
<span data-ttu-id="04985-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04985-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04985-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04985-134">JSON Representation</span></span>
<span data-ttu-id="04985-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04985-135">Here is a JSON representation of the resource.</span></span>
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



